## `plone:4-alpine`

```console
$ docker pull plone@sha256:1a1c347f3bd762eeff74e6300bce9a4dd417f3144a5677134150cb229dc66278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:4-alpine` - linux; amd64

```console
$ docker pull plone@sha256:8b7825e710aae27c817e893f1f7b61f529925889bd17dbd016695c5e25a7cdf2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.9 MB (108893697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c5cdff24300bdce962c07f0618840091f2f50d3eb55912b12bdeed24e43dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:37:13 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:05:17 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Jan 2020 03:05:18 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:05:18 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 18 Jan 2020 03:05:18 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 18 Jan 2020 03:10:20 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sat, 18 Jan 2020 03:10:20 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Sat, 18 Jan 2020 03:10:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Sat, 18 Jan 2020 03:10:21 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Sat, 18 Jan 2020 03:10:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 18 Jan 2020 03:10:26 GMT
CMD ["python2"]
# Sat, 18 Jan 2020 05:10:11 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Sat, 18 Jan 2020 05:10:11 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Sat, 18 Jan 2020 05:10:12 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 18 Jan 2020 05:10:12 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Sat, 18 Jan 2020 05:19:31 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 18 Jan 2020 05:19:32 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 05:19:33 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Sat, 18 Jan 2020 05:19:33 GMT
EXPOSE 8080
# Sat, 18 Jan 2020 05:19:33 GMT
WORKDIR /plone/instance
# Sat, 18 Jan 2020 05:19:33 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 18 Jan 2020 05:19:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:19:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea5c17ab132115631f8ed013132367bade1bf4b9df91fe0e962bfbfc63336ac`  
		Last Modified: Sat, 18 Jan 2020 03:11:58 GMT  
		Size: 301.3 KB (301259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbe995357bf87b3689676cf8a89e250a99ba7fd60ab32e5eba2e83a20b4b215`  
		Last Modified: Sat, 18 Jan 2020 03:12:02 GMT  
		Size: 20.7 MB (20710099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afb78be294494b794b2f2c01c26730bff6457c34d5b6a13ba07546577e9498c`  
		Last Modified: Sat, 18 Jan 2020 03:11:59 GMT  
		Size: 1.9 MB (1866333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a82ad45119d5f52a1df44dff6cc6de735a04c6867e3e080fe21afe3729096a3`  
		Last Modified: Sat, 18 Jan 2020 05:20:55 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e26bc6dd24f9e6306eb30e8c5e9aa850cf167e8d9f465cd685fb501d04fc713`  
		Last Modified: Sat, 18 Jan 2020 05:20:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe74006605627051fdd0e073d7839cae6ffacd8a4b1197c04f3d43d541ba92b4`  
		Last Modified: Sat, 18 Jan 2020 05:21:18 GMT  
		Size: 83.2 MB (83207586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba557a7ce1308e9163d3d062b78f53321a03a33aba618587f786379f78f58015`  
		Last Modified: Sat, 18 Jan 2020 05:20:55 GMT  
		Size: 2.9 KB (2882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:4-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:bc6501060ac8cf6387f7cdfd48dc9a29e9e41bdfc64ddfa3aeab73c6ca475e76
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106965210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8389fe0e4b6f2f87f3e84b5462f152cd58220dd546fa21fe7e61e63c75238f2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:38:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:38:59 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:31:00 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Jan 2020 05:31:12 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:31:17 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 18 Jan 2020 05:31:21 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 18 Jan 2020 05:42:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Thu, 23 Jan 2020 23:11:13 GMT
ENV PYTHON_PIP_VERSION=20.0.1
# Thu, 23 Jan 2020 23:11:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 23 Jan 2020 23:11:15 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 23 Jan 2020 23:11:34 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Jan 2020 23:11:35 GMT
CMD ["python2"]
# Fri, 24 Jan 2020 01:06:44 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Fri, 24 Jan 2020 01:06:45 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 24 Jan 2020 01:06:51 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 24 Jan 2020 01:06:52 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Fri, 24 Jan 2020 01:28:13 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 24 Jan 2020 01:28:19 GMT
VOLUME [/data]
# Fri, 24 Jan 2020 01:28:19 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Fri, 24 Jan 2020 01:28:20 GMT
EXPOSE 8080
# Fri, 24 Jan 2020 01:28:21 GMT
WORKDIR /plone/instance
# Fri, 24 Jan 2020 01:28:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 24 Jan 2020 01:28:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Jan 2020 01:28:23 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9ee5cb431b6df66261c35037b6a83da0e40c73306a795eab69536be10dfe1`  
		Last Modified: Sat, 18 Jan 2020 05:45:09 GMT  
		Size: 301.6 KB (301617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d417f4578e06c92fe68969a793bf3852e440daea306071b5d92b5c502fd710c2`  
		Last Modified: Sat, 18 Jan 2020 05:45:17 GMT  
		Size: 19.4 MB (19402798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0ef8e91360347f31bf3ac03829825d6b6594d6bf64909656508acf3fd00fda`  
		Last Modified: Thu, 23 Jan 2020 23:14:12 GMT  
		Size: 1.9 MB (1942432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2591d6a2e5f2fdcc8580e92951983eb73bf3e127c87102dd40ac2d45d49fc6e`  
		Last Modified: Fri, 24 Jan 2020 01:31:00 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98e7610d34e8e4b8a125d7517e814f14a17b8b1351d9fa24a5b5a407af4e157`  
		Last Modified: Fri, 24 Jan 2020 01:31:00 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ec430f0aa65c6a5f08010405b93a0d1a6c3577f8c4683c7628ea2f19ae4df`  
		Last Modified: Fri, 24 Jan 2020 01:32:12 GMT  
		Size: 82.7 MB (82695272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1a026b53f5ec5b93d2f4bd8e73fb32e51cee165143b5d0e80339f5b6781c7f`  
		Last Modified: Fri, 24 Jan 2020 01:30:59 GMT  
		Size: 2.9 KB (2881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:4-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:c6a3b70d797b68e208c7f43c675526b59ee852d56e0f1a4e717ecdf43a91c680
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108215283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56945612a79dd83dbf00bec5364cf6973f959430f52c0a97640b24ab29dd056e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:23:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:23:12 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:06:50 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Jan 2020 04:06:57 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:06:58 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 18 Jan 2020 04:07:00 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 18 Jan 2020 04:16:17 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Fri, 24 Jan 2020 09:24:54 GMT
ENV PYTHON_PIP_VERSION=20.0.1
# Fri, 24 Jan 2020 09:24:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 24 Jan 2020 09:24:55 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 24 Jan 2020 09:25:07 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Jan 2020 09:25:08 GMT
CMD ["python2"]
# Fri, 24 Jan 2020 11:42:58 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Fri, 24 Jan 2020 11:42:59 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 24 Jan 2020 11:43:00 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 24 Jan 2020 11:43:01 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Fri, 24 Jan 2020 12:03:00 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 24 Jan 2020 12:03:08 GMT
VOLUME [/data]
# Fri, 24 Jan 2020 12:03:08 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Fri, 24 Jan 2020 12:03:09 GMT
EXPOSE 8080
# Fri, 24 Jan 2020 12:03:09 GMT
WORKDIR /plone/instance
# Fri, 24 Jan 2020 12:03:10 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 24 Jan 2020 12:03:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Jan 2020 12:03:11 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55aa4b23d1c945e644c16e0a10c13704ef3215b13d1752d03032a86786dc0a4`  
		Last Modified: Sat, 18 Jan 2020 04:19:56 GMT  
		Size: 301.8 KB (301760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec79a1c6d20ca237f366b092214e9eac3f82f49a431ddf5308b4815bfa96556`  
		Last Modified: Sat, 18 Jan 2020 04:20:03 GMT  
		Size: 20.4 MB (20364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05a0716544c76e300bb1765105d4903b47df93acae82f9fceb9a5677beb8bc5`  
		Last Modified: Fri, 24 Jan 2020 09:31:08 GMT  
		Size: 1.9 MB (1942417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c41304d1ef8f638f771a36eb7da2e7ec497523e2363b431413f9ef56994046`  
		Last Modified: Fri, 24 Jan 2020 12:09:49 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcfb9a410600237074ec04980bbe6fac8c29b54301d6937d95ec1831f867c9f`  
		Last Modified: Fri, 24 Jan 2020 12:09:50 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa07d74d5f4cb5925bfe3c67ebc4b2df1977e01ea004654d8eb6261a9523795`  
		Last Modified: Fri, 24 Jan 2020 12:10:59 GMT  
		Size: 82.9 MB (82877896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590918d0c537a83837ed58189938ecb4a146b829e37526eefef90521bf2ce236`  
		Last Modified: Fri, 24 Jan 2020 12:09:49 GMT  
		Size: 2.9 KB (2880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:4-alpine` - linux; 386

```console
$ docker pull plone@sha256:8e4f95a7b68a883219529e8be413d4e2243ce63921833f64830be09581186dba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107590402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20b8fe553f5bab6f0d378b239aad76a2a51d851963981ce5dab303f8ce0ed406`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:56:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:56:40 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:29:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Jan 2020 05:29:24 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:29:24 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 18 Jan 2020 05:29:24 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 18 Jan 2020 05:36:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Fri, 24 Jan 2020 03:34:05 GMT
ENV PYTHON_PIP_VERSION=20.0.1
# Fri, 24 Jan 2020 03:34:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 24 Jan 2020 03:34:05 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 24 Jan 2020 03:34:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Jan 2020 03:34:11 GMT
CMD ["python2"]
# Fri, 24 Jan 2020 11:22:38 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Fri, 24 Jan 2020 11:22:38 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 24 Jan 2020 11:22:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 24 Jan 2020 11:22:39 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Fri, 24 Jan 2020 11:34:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 24 Jan 2020 11:34:52 GMT
VOLUME [/data]
# Fri, 24 Jan 2020 11:34:52 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Fri, 24 Jan 2020 11:34:52 GMT
EXPOSE 8080
# Fri, 24 Jan 2020 11:34:52 GMT
WORKDIR /plone/instance
# Fri, 24 Jan 2020 11:34:52 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 24 Jan 2020 11:34:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Jan 2020 11:34:53 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a77ddb7ca1169962ea618a46a6b8b7816331fb8c59b33d94e8524f6ecc020f`  
		Last Modified: Sat, 18 Jan 2020 05:38:24 GMT  
		Size: 301.9 KB (301910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bfa87a42954e46ea1e13754708a50260e4fb4d30603c6c29cf3ae8919f246f`  
		Last Modified: Sat, 18 Jan 2020 05:38:30 GMT  
		Size: 19.9 MB (19861131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c07781d8dce1fdb37e76c179077b1ce268aa339504210e47998115a539567d`  
		Last Modified: Fri, 24 Jan 2020 03:44:45 GMT  
		Size: 1.9 MB (1942062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2823fea6e14b0c230c63dbf2b04d0b683d99ad52733aaa4c515c0e95772688`  
		Last Modified: Fri, 24 Jan 2020 11:42:55 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eeef59b136be2de2f5aa4d4cd3f735e05c678b56d160d6ca6e9f25d02800958`  
		Last Modified: Fri, 24 Jan 2020 11:42:55 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9221d49e50ac8b9db5657fcead354b17451e954d789e0cbcc0dd791ac53a91f`  
		Last Modified: Fri, 24 Jan 2020 11:43:26 GMT  
		Size: 82.7 MB (82673270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359dbd7ee7ef74d1b1f47413b43b124987fafa4b844bb517c995c1d453f65f`  
		Last Modified: Fri, 24 Jan 2020 11:42:55 GMT  
		Size: 2.9 KB (2880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:4-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:275a63dbfd33b3e4f8556457275683a0241ff598c0c987c4536e2defc265b86f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109892507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00752fab2f5d73bece17baa6c167d68f882ec7409db3b94c28f9eef20907f18`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:57:42 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:35:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Jan 2020 05:36:00 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:36:02 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 18 Jan 2020 05:36:04 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 18 Jan 2020 05:43:10 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Fri, 24 Jan 2020 05:27:58 GMT
ENV PYTHON_PIP_VERSION=20.0.1
# Fri, 24 Jan 2020 05:28:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 24 Jan 2020 05:28:01 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 24 Jan 2020 05:28:17 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Jan 2020 05:28:19 GMT
CMD ["python2"]
# Fri, 24 Jan 2020 13:23:33 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Fri, 24 Jan 2020 13:23:37 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 24 Jan 2020 13:23:50 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 24 Jan 2020 13:23:52 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Fri, 24 Jan 2020 13:41:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 24 Jan 2020 13:41:42 GMT
VOLUME [/data]
# Fri, 24 Jan 2020 13:41:43 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Fri, 24 Jan 2020 13:41:45 GMT
EXPOSE 8080
# Fri, 24 Jan 2020 13:41:48 GMT
WORKDIR /plone/instance
# Fri, 24 Jan 2020 13:41:52 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 24 Jan 2020 13:41:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Jan 2020 13:41:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71484225792d18482c4c33240e65f27532a437830baa8fe82a1152f9fd9a4bfb`  
		Last Modified: Sat, 18 Jan 2020 05:47:29 GMT  
		Size: 304.0 KB (303975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924299c31fe2afa16ccc2ec832adf989db449ec454ec43377dfaba3f3608c539`  
		Last Modified: Sat, 18 Jan 2020 05:47:35 GMT  
		Size: 21.3 MB (21301536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf3d6a7f1173839e787a872e41720af4cc84fc90390bc524cc0cd62e2c70d9f`  
		Last Modified: Fri, 24 Jan 2020 05:37:38 GMT  
		Size: 1.9 MB (1942354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81152a731aff9ca2638b9e61df2d8c5563889e5aa2d6fc28dc8d9edae60d567`  
		Last Modified: Fri, 24 Jan 2020 13:53:05 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1e4945800ff146b623482a39adb3da639c44f14dfaa45d57bf0262711f200a`  
		Last Modified: Fri, 24 Jan 2020 13:53:05 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e54e6a4ab5c0d4cb60c7d3254a3d75c7185b04be07746f622f7f34ca837d20a`  
		Last Modified: Fri, 24 Jan 2020 13:54:14 GMT  
		Size: 83.5 MB (83516983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af0638a52cc255eb0e6d89fc18ffcbe60b2e3854644bd4f7542165a81f9354`  
		Last Modified: Fri, 24 Jan 2020 13:53:06 GMT  
		Size: 2.9 KB (2883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:4-alpine` - linux; s390x

```console
$ docker pull plone@sha256:5deb0b3d8272529501e968d72a3d6f259938016a378c74303ba854bb6c4d9df5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105813789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f67df8d945e51112f46364d7f96ecc877ef28a2a22618c1f85b073bcdc4433`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:57:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 21 Oct 2019 18:57:49 GMT
ENV LANG=C.UTF-8
# Tue, 22 Oct 2019 01:16:25 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 22 Oct 2019 01:16:26 GMT
RUN apk add --no-cache ca-certificates
# Tue, 22 Oct 2019 01:16:26 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Thu, 24 Oct 2019 00:57:22 GMT
ENV PYTHON_VERSION=2.7.17
# Fri, 15 Nov 2019 03:54:46 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-shared 		--enable-unicode=ucs4 		--with-system-expat 		--with-system-ffi 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Fri, 15 Nov 2019 03:54:47 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 15 Nov 2019 03:54:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 15 Nov 2019 03:54:47 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 15 Nov 2019 03:54:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 Nov 2019 03:54:52 GMT
CMD ["python2"]
# Fri, 15 Nov 2019 05:41:29 GMT
ENV PIP=9.0.3 ZC_BUILDOUT=2.13.1 SETUPTOOLS=40.8.0 WHEEL=0.33.1 PLONE_MAJOR=4.3 PLONE_VERSION=4.3.19 PLONE_MD5=04ed5beac7fb8504f06a36d44e407b06
# Fri, 15 Nov 2019 05:41:29 GMT
LABEL plone=4.3.19 os=alpine os.version=3.10 name=Plone 4.3 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 15 Nov 2019 05:41:30 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 15 Nov 2019 05:41:30 GMT
COPY file:d2686f3dde22793e1cf870d3f997b1d6ff10a1bb2a2c48fe9a9f11b9824a86c1 in /plone/instance/ 
# Fri, 15 Nov 2019 05:49:38 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/Plone-$PLONE_VERSION-UnifiedInstaller.tgz  && echo "$PLONE_MD5  Plone.tgz" | md5sum -c -  && tar -zxvf Plone.tgz  && cp -rv ./Plone-$PLONE_VERSION-UnifiedInstaller/base_skeleton/* /plone/instance/  && cp -v ./Plone-$PLONE_VERSION-UnifiedInstaller/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && rm -rf bin/buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance//var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apk del .build-deps  && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 15 Nov 2019 05:49:39 GMT
VOLUME [/data]
# Fri, 15 Nov 2019 05:49:40 GMT
COPY multi:1923bbb6e3d76129ed8afd8e145516fb42d067a3323b0830ce09a51a5a3d629c in / 
# Fri, 15 Nov 2019 05:49:40 GMT
EXPOSE 8080
# Fri, 15 Nov 2019 05:49:40 GMT
WORKDIR /plone/instance
# Fri, 15 Nov 2019 05:49:41 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 15 Nov 2019 05:49:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 Nov 2019 05:49:41 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87da057bc7467c488226a0f5368a96c0eb396ff2684bd7a58d0dbb5c88ef6334`  
		Last Modified: Tue, 22 Oct 2019 01:19:36 GMT  
		Size: 302.4 KB (302376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b59e9c7ba879b7726965965c20aebe3c0d4b0d1032d472bfa698573429771b`  
		Last Modified: Fri, 15 Nov 2019 04:02:57 GMT  
		Size: 18.8 MB (18760145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9909268e4fa5a3831d4999d5a4f51fbe166535e2aa4f6a10ec849612450f3cd4`  
		Last Modified: Fri, 15 Nov 2019 04:02:41 GMT  
		Size: 1.9 MB (1865159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713d1701eacb2a15b19690ac4773c55641b5d1debba3f196cfc7990e6c774496`  
		Last Modified: Fri, 15 Nov 2019 05:50:57 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9774f4c2b30a6dd85f9aeb626f23f15158bf3b3875cf7ff0a8b43bb685ba2e6`  
		Last Modified: Fri, 15 Nov 2019 05:50:57 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb0532261992abf2ba66caecbfa821c01b3cf5a66cb39a4ec2e57587d94cd71`  
		Last Modified: Fri, 15 Nov 2019 05:51:14 GMT  
		Size: 82.3 MB (82307029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c29cf0a416f0efa34e9e523d60f254cbbf77def9f8b1b1141ebad83e803c55f`  
		Last Modified: Fri, 15 Nov 2019 05:50:57 GMT  
		Size: 2.9 KB (2881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
