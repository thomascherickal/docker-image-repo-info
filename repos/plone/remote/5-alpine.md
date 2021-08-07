## `plone:5-alpine`

```console
$ docker pull plone@sha256:379aa4145b6c2547f0920c3848e3436cdece4d0dee0a2ec964c04cdbe90191d6
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
$ docker pull plone@sha256:3aeea40fe61245846f3f9cfa379cbdfdd1336447f532279ca20ccacdd77461ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152158425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b998065c9da556386944f67394b68be87011d1eca6cbf39077c97ad02c0afe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:37:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 21:11:33 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 21:30:58 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 06 Aug 2021 21:30:58 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 06 Aug 2021 21:30:58 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 06 Aug 2021 21:37:04 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 06 Aug 2021 21:37:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 06 Aug 2021 21:37:05 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Fri, 06 Aug 2021 21:37:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 06 Aug 2021 21:37:05 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 06 Aug 2021 21:37:12 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 06 Aug 2021 21:37:12 GMT
CMD ["python3"]
# Sat, 07 Aug 2021 02:15:15 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 07 Aug 2021 02:15:16 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 07 Aug 2021 02:15:16 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 07 Aug 2021 02:27:48 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 07 Aug 2021 02:27:50 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 02:27:50 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 07 Aug 2021 02:27:50 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 02:27:51 GMT
WORKDIR /plone/instance
# Sat, 07 Aug 2021 02:27:51 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 07 Aug 2021 02:27:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 07 Aug 2021 02:27:51 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3626a090061d56f9d6eaa946c29f4a7600401e2bca3f7b517369d0da709bf6d3`  
		Last Modified: Fri, 06 Aug 2021 22:03:22 GMT  
		Size: 281.5 KB (281505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab7c3958d02c548f8a01137383d178a982079695cda15bda551d17fde69092`  
		Last Modified: Fri, 06 Aug 2021 22:03:25 GMT  
		Size: 11.2 MB (11244323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d9978a71b93404de628d3705cbf22d6b284b0264c244c84a0ba170ce640cb7`  
		Last Modified: Fri, 06 Aug 2021 22:03:22 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e93103535260c51fbb6da1174085bd794ca3be8324fa69cabebe1df938391e0`  
		Last Modified: Fri, 06 Aug 2021 22:03:23 GMT  
		Size: 2.4 MB (2355097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1cdeabe9d502043962ddcd4ef932f78a65b9aecef526bec6534700d90448a`  
		Last Modified: Sat, 07 Aug 2021 02:30:25 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823870d2f167978c0459db05c643e654dbd533508b1a1431917c0fd1d2b31f06`  
		Last Modified: Sat, 07 Aug 2021 02:30:25 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e06c1d1f4760d4c539d26c8474825431ba9afdef77fe46f9dbc50a5b74d7a1c`  
		Last Modified: Sat, 07 Aug 2021 02:30:50 GMT  
		Size: 135.5 MB (135457823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c833ab4510d43f8d137b7e03de5c0c49db55bcaf05236526a6fafb7c4d943`  
		Last Modified: Sat, 07 Aug 2021 02:30:25 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:4e434f653cd1652382d1a8ff41949e25eabfa8d7711c6d1fa5bfa3d66a60218b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.9 MB (150908702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e5be25cd662b2295227d819cf356c1aee78bc21eedcd770081d2ac6f328139`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:10:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:10:56 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 22:40:35 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 06 Aug 2021 22:40:36 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 06 Aug 2021 22:40:37 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 06 Aug 2021 22:53:28 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 06 Aug 2021 22:53:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 06 Aug 2021 22:53:30 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Fri, 06 Aug 2021 22:53:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 06 Aug 2021 22:53:31 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 06 Aug 2021 22:53:46 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 06 Aug 2021 22:53:47 GMT
CMD ["python3"]
# Sat, 07 Aug 2021 03:02:01 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 07 Aug 2021 03:02:02 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 07 Aug 2021 03:02:03 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 07 Aug 2021 03:27:19 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 07 Aug 2021 03:27:22 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 03:27:22 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 07 Aug 2021 03:27:23 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 03:27:23 GMT
WORKDIR /plone/instance
# Sat, 07 Aug 2021 03:27:24 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 07 Aug 2021 03:27:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 07 Aug 2021 03:27:25 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fce632e670bccbc0903da70add2d72568a9c2b703cbe9aa1a968f6d0bfb7673`  
		Last Modified: Fri, 06 Aug 2021 23:31:33 GMT  
		Size: 281.7 KB (281674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d4f66268ec3e17e61e9e6e91bcbacea5fc85d0ea6f77132eb749e238f75d71`  
		Last Modified: Fri, 06 Aug 2021 23:31:39 GMT  
		Size: 10.8 MB (10827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5d2f94b7fc6ae598dcf5b448ed7b645be05a981c081747beb52027deda0da9`  
		Last Modified: Fri, 06 Aug 2021 23:31:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2756aa4d1badba0e523c99e90593b3e57d35ad18df1796cd1835c70983b834e`  
		Last Modified: Fri, 06 Aug 2021 23:31:34 GMT  
		Size: 2.4 MB (2355217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c94b217afc89518cf45595b665b71533000ba42a0e627b02b58cf7b0afa357`  
		Last Modified: Sat, 07 Aug 2021 03:27:57 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e149bb51e805644fc433d0a7d1f17726f9309d6cb4618552260d4525de753b0`  
		Last Modified: Sat, 07 Aug 2021 03:27:56 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c342d70894ac11d77c9198e641d1f465d543ee9147919907d6b988c8f1a1b`  
		Last Modified: Sat, 07 Aug 2021 03:29:42 GMT  
		Size: 134.8 MB (134811306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32947ea45bcac5a582110d31456cbea8b940b6695ed5412a5cad2b00d96fb847`  
		Last Modified: Sat, 07 Aug 2021 03:27:56 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:3b659399773041e611f90006564cfbdf1a60105ce6ab11158bb95c7acd16bd1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (152036077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b66eff8bbdfeeb069212eafd98ef26b99c4cd657b472b808d8076f09eddcce09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:48:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 23:28:08 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 23:43:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 06 Aug 2021 23:43:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 06 Aug 2021 23:43:28 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 06 Aug 2021 23:49:18 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 06 Aug 2021 23:49:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 06 Aug 2021 23:49:19 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Fri, 06 Aug 2021 23:49:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 06 Aug 2021 23:49:20 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 06 Aug 2021 23:49:26 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 06 Aug 2021 23:49:26 GMT
CMD ["python3"]
# Sat, 07 Aug 2021 04:40:53 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 07 Aug 2021 04:40:54 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 07 Aug 2021 04:40:54 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 07 Aug 2021 04:54:30 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 07 Aug 2021 04:54:33 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 04:54:33 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 07 Aug 2021 04:54:33 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 04:54:33 GMT
WORKDIR /plone/instance
# Sat, 07 Aug 2021 04:54:33 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 07 Aug 2021 04:54:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 07 Aug 2021 04:54:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd496dba037efd04fc4937dd16b10cb87ae37d722c8751ef5f9adbfd57f4f116`  
		Last Modified: Sat, 07 Aug 2021 00:15:12 GMT  
		Size: 281.7 KB (281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda0ce65f112f2e6ab6630c071313b585c0847c3907a8ac344aa3805af1f73d8`  
		Last Modified: Sat, 07 Aug 2021 00:15:13 GMT  
		Size: 11.3 MB (11302197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac5d64d22c7436ce090e68d6c2d58d2f472c10188a57e2843380dbca3b55dc`  
		Last Modified: Sat, 07 Aug 2021 00:15:12 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a97cc82a5390d15e7e3d382e8c173027f342ab5d60a72aadf2b41b5642dd732`  
		Last Modified: Sat, 07 Aug 2021 00:15:12 GMT  
		Size: 2.4 MB (2355244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22edb08d8ce4a5772eedae3b4f6d5e730a8a24f027d23c3ea58319f4304f0a83`  
		Last Modified: Sat, 07 Aug 2021 04:54:52 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6578c3fe9ec3129b1d8722c5c4239cbee144533d9a4d1ff0fd4f1bf1dd14a860`  
		Last Modified: Sat, 07 Aug 2021 04:54:52 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbd23011a65dea8b60ec6cd19946dba9b234787484011198f560855bfa7c624`  
		Last Modified: Sat, 07 Aug 2021 04:55:15 GMT  
		Size: 135.4 MB (135379676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcb3674940c8ae03840aef04f433f6359a8cacb04bcd787fb41895d569b41c4`  
		Last Modified: Sat, 07 Aug 2021 04:54:52 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:ffa1254bdffa68592b206ec84a9528b80879da59a44c37a6dad8e9e736a6b475
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153364742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbfac97b63305cde4256d0cb5e8fe17d7acaef1c23d94193289d53ff7733ae7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:30:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:30:10 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 22:48:29 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 06 Aug 2021 22:48:29 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 06 Aug 2021 22:48:30 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 06 Aug 2021 22:58:09 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 06 Aug 2021 22:58:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 06 Aug 2021 22:58:12 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Fri, 06 Aug 2021 22:58:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 06 Aug 2021 22:58:12 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 06 Aug 2021 22:58:21 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 06 Aug 2021 22:58:21 GMT
CMD ["python3"]
# Sat, 07 Aug 2021 05:32:40 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 07 Aug 2021 05:32:41 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 07 Aug 2021 05:32:41 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 07 Aug 2021 05:47:31 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 07 Aug 2021 05:47:34 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 05:47:34 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 07 Aug 2021 05:47:34 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 05:47:35 GMT
WORKDIR /plone/instance
# Sat, 07 Aug 2021 05:47:35 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 07 Aug 2021 05:47:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 07 Aug 2021 05:47:35 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49056098fc643a84d25c508ba089cd7e0b0dbbfcb5fb20902d520bc82424d43b`  
		Last Modified: Sat, 07 Aug 2021 02:22:22 GMT  
		Size: 282.0 KB (282043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba53bcb7ed7e8855940dc034cfc02f9bd672a3cbed7e759c9ebfea98016a84c`  
		Last Modified: Sat, 07 Aug 2021 02:22:24 GMT  
		Size: 11.4 MB (11432483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d65d1e73f44b5f510b7f5e7f4bb8b3360cd6d04472f3784e602fc92941f89a7`  
		Last Modified: Sat, 07 Aug 2021 02:22:21 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ee0c3abcab86c730530fd901d755ab7fa8a336f969c7a81932c2d8cc4532c`  
		Last Modified: Sat, 07 Aug 2021 02:22:22 GMT  
		Size: 2.4 MB (2355097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed87678cd633a045a5376cd60d91193b6f9fc90480ffe4be3710abd105c46aa`  
		Last Modified: Sat, 07 Aug 2021 05:47:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df757a733370467a7746f0101e64f1f9032521de6ea3354ced8476463e41b71`  
		Last Modified: Sat, 07 Aug 2021 05:47:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12caa9a550fc931db3e25ff1c3352e31ab2cef3d59e4baa5758a84c6f1c11cc5`  
		Last Modified: Sat, 07 Aug 2021 05:48:22 GMT  
		Size: 136.5 MB (136466537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c60d12e559a76cd42d07154b16cfe5b6ea78335922943c5e1c94af123899f`  
		Last Modified: Sat, 07 Aug 2021 05:47:53 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:062d6811924de9a41f3c6b5ca13b7acb2a8cb6d558b52cebe4184ece2645eeab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153858370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faeaa9c2de5052822666a2d89be7aa448394740c28b94d7cb5a97049735b811d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:34:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:34:35 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 19:06:10 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 06 Aug 2021 19:06:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 06 Aug 2021 19:06:17 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 06 Aug 2021 19:14:23 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 06 Aug 2021 19:14:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 06 Aug 2021 19:14:41 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Fri, 06 Aug 2021 19:14:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 06 Aug 2021 19:14:47 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 06 Aug 2021 19:15:05 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 06 Aug 2021 19:15:10 GMT
CMD ["python3"]
# Sat, 07 Aug 2021 03:13:54 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 07 Aug 2021 03:14:01 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 07 Aug 2021 03:14:03 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 07 Aug 2021 03:35:16 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 07 Aug 2021 03:35:32 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 03:35:35 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 07 Aug 2021 03:35:39 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 03:35:45 GMT
WORKDIR /plone/instance
# Sat, 07 Aug 2021 03:35:48 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 07 Aug 2021 03:35:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 07 Aug 2021 03:35:56 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8479c3e0d7fec98095b4beac83f9d91b5eb0795b66b61644662edddb55f1ab7`  
		Last Modified: Fri, 06 Aug 2021 19:53:50 GMT  
		Size: 283.6 KB (283636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd00c6b7f8be2d488a85f3f400565c742712995e13465b5cd562e467e2297c1`  
		Last Modified: Fri, 06 Aug 2021 19:53:52 GMT  
		Size: 11.5 MB (11538309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cf673c9a800fb0c3a01c50e8e181475f75dc25e5b27631f04b218227151342`  
		Last Modified: Fri, 06 Aug 2021 19:53:49 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7670981af5066182c98bf431ebc83d7bad203971ee7f926722bcf4c6041323`  
		Last Modified: Fri, 06 Aug 2021 19:53:50 GMT  
		Size: 2.4 MB (2355249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e1a702fd29e39c687f515f8476a4080e8dbc3e0f17f442f72e7e98432a32d`  
		Last Modified: Sat, 07 Aug 2021 03:36:23 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651391b421d69724a0b8895737b286a731f036a3f9fcd921a45d896f2da7c2f1`  
		Last Modified: Sat, 07 Aug 2021 03:36:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecd421eba5d3aa089def38cfc9ad2c7bcfbc5395de92a5f3bdcc67dee422981`  
		Last Modified: Sat, 07 Aug 2021 03:36:49 GMT  
		Size: 136.9 MB (136863356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76b98c99d19a9b0e17abb7d8d1967e63c07ec51131a19f74b6c0a8c8d4ab8a`  
		Last Modified: Sat, 07 Aug 2021 03:36:23 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:41307f0ee610cf238ab99e08efde2c82c9c22813381be2cf9459c25decaaa437
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151971327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7024bf3e57c521d83b98de6cf420ece2fb9afee09440c23f97de9c6cf8cdd94a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 21:55:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 26 Jun 2021 21:55:22 GMT
ENV LANG=C.UTF-8
# Sun, 27 Jun 2021 04:34:32 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sun, 27 Jun 2021 04:34:32 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sun, 27 Jun 2021 04:34:33 GMT
ENV PYTHON_VERSION=3.8.10
# Sun, 27 Jun 2021 04:40:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sun, 27 Jun 2021 04:40:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sun, 27 Jun 2021 04:40:28 GMT
ENV PYTHON_PIP_VERSION=21.1.2
# Sun, 27 Jun 2021 04:40:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/936e08ce004d0b2fae8952c50f7ccce1bc578ce5/public/get-pip.py
# Sun, 27 Jun 2021 04:40:28 GMT
ENV PYTHON_GET_PIP_SHA256=8890955d56a8262348470a76dc432825f61a84a54e2985a86cd520f656a6e220
# Sun, 27 Jun 2021 04:40:36 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 27 Jun 2021 04:40:37 GMT
CMD ["python3"]
# Sun, 27 Jun 2021 16:26:36 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sun, 27 Jun 2021 16:26:36 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sun, 27 Jun 2021 16:26:37 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sun, 27 Jun 2021 16:37:44 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sun, 27 Jun 2021 16:37:56 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:37:56 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sun, 27 Jun 2021 16:37:56 GMT
EXPOSE 8080
# Sun, 27 Jun 2021 16:37:57 GMT
WORKDIR /plone/instance
# Sun, 27 Jun 2021 16:37:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sun, 27 Jun 2021 16:37:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 27 Jun 2021 16:37:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3458e7c8450afd4ac23016a210cff9430775463b81b2c791ca25a7e1fef4b0a`  
		Last Modified: Sun, 27 Jun 2021 11:33:44 GMT  
		Size: 281.7 KB (281714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df39682fa6c9282e8e73e918d8e4476e099947c62ecdc67921e2fe08d826541`  
		Last Modified: Sun, 27 Jun 2021 11:33:50 GMT  
		Size: 11.6 MB (11611528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6bbd28aa3f6bfd6f857e9a1744d7867fdf415582f7873b272c02c0837cee40`  
		Last Modified: Sun, 27 Jun 2021 11:33:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bd4b91269b927e104660934e80a54b9171e2f62bbfcd972b0638f61b3f79e`  
		Last Modified: Sun, 27 Jun 2021 11:33:44 GMT  
		Size: 2.3 MB (2348337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e76db18ddaca2cf7b8f4bb6938ee08d9dd6ea1b2bb22af08bd434c481eb1a1d`  
		Last Modified: Sun, 27 Jun 2021 16:38:18 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cbc57bd72a2f18a1d6d393fbeb553dfe02fb4481f05c3eedb54e1cc4eed243`  
		Last Modified: Sun, 27 Jun 2021 16:38:18 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057a6ab4459c106b0c47737635bbf8697fb993a6a8c427311a8634236606c2c7`  
		Last Modified: Sun, 27 Jun 2021 16:38:37 GMT  
		Size: 135.1 MB (135120440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b38b77b56f5c3b0b45785cef4127b06f8cbeed2f0715a183b0fefbffbce8d`  
		Last Modified: Sun, 27 Jun 2021 16:38:18 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
