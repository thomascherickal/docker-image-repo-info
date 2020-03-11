## `plone:alpine`

```console
$ docker pull plone@sha256:c8dc0c313bb90c1ea86d31758645c0b352053d9f1c316334580ee8faeb798e79
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
$ docker pull plone@sha256:0c096be1cf04c60572e92f6e048d48bc06b7aaf10ffc7603bc074339a2cd1202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167524259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d110dfe8b84924bb805ca859c08c3e31a8423095de96fdc510da999ba8f3cd`
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
# Sat, 18 Jan 2020 02:37:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:43:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:54:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:03:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:03:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:03:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:03:29 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:36:31 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:36:31 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:36:32 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:36:32 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:46:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:46:33 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:46:33 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:46:33 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:46:34 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:46:34 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:46:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5ad85d9abaadf23d5ae53c3f32e7ccb2df1956869980bfd2491ff396d348a`  
		Last Modified: Sat, 18 Jan 2020 03:11:07 GMT  
		Size: 301.3 KB (301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29edaae8dc30d7fc1e5c9c5a016e604e4b7cb4f6c5ecb9a3db52ebfc239db28e`  
		Last Modified: Wed, 11 Mar 2020 01:16:37 GMT  
		Size: 28.7 MB (28662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b1dc8253c8ff1738172bc5fdd061c70e30c965e11fd50436c2de192b80aaf`  
		Last Modified: Wed, 11 Mar 2020 01:16:31 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf370601a519cbf3f23c20bd5324374f3298a016e528911400bbaf2fc9d9fc`  
		Last Modified: Wed, 11 Mar 2020 01:16:32 GMT  
		Size: 1.9 MB (1890930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a4b668572d274ff9367bfbef67a9bc3019ea12fc2a58ea82a0eea5b285eff6`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d92a5515d89654fe39e14ae01a7ca45c43f3c384eda886f7cd4890a39aba4`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fedfc2f69a3a7fdcd3304d490f66dafb8a602d0237cc37115a420f3d0d1b39`  
		Last Modified: Wed, 11 Mar 2020 01:48:05 GMT  
		Size: 133.9 MB (133861603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432ae9ed707294c44ebb22b4ae0a84dc1cea08f048c5bc14c6624d4b2491501`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:733ded7baf5291bcb8705d08b37c71dcd350b1908fafcc31b17da63810642269
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164753015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ee5528cb767a9658228f1568269c7e9e1bd2c5988eed7626a141609dc784f`
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
# Sat, 18 Jan 2020 04:39:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:50:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Mar 2020 23:55:19 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:11:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:11:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:11:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:11:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:11:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:11:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:11:52 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 00:46:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 00:46:11 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 00:46:13 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 00:46:13 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:05:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:05:54 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:05:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:05:56 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:05:58 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:05:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:06:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a761fb3a5329492c5833bf26b25380ceb0c5243bea653014c9e329fd6901d4a`  
		Last Modified: Sat, 18 Jan 2020 05:43:45 GMT  
		Size: 301.6 KB (301623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff232bcbce1b952dce3fb1514e26139d4b21a75ef45ab03adf8b3cf16267d9`  
		Last Modified: Wed, 11 Mar 2020 00:28:17 GMT  
		Size: 26.6 MB (26631625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f767fb3cf30af8ed99f6d09de819fa937560cbb3a6d9d9f529b14e4fd273861`  
		Last Modified: Wed, 11 Mar 2020 00:28:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e981cab0ab9d602e6cda10e0ebe660effacb6568e23deaaf3762f291e3f091`  
		Last Modified: Wed, 11 Mar 2020 00:28:08 GMT  
		Size: 1.9 MB (1891153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b4e82b96c780400c428a78f8d81a94fc3ec626dd615eec7ce597bedae4662`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17fa2cd2cece0abc3cda884ab354878c14621bf6b8723908915cf6f1145771`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaf98029b25c2b64b2489034ee2b4f43ddcafb223027120dcaacd032c47194`  
		Last Modified: Wed, 11 Mar 2020 01:07:13 GMT  
		Size: 133.3 MB (133305793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ab1b02c65c97f665ba6c4ad2119f8425716d6fdc30f4eb946120536580252`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f3f037db79cf64c39db3d599890cbe45a8f8a7167b1634ea17f0a42d4c1b4105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166671522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a31999e3cdd98ef95738ba5a22ba6e22d5c94e959a3ed4eeb5907168d686e71`
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
# Sat, 18 Jan 2020 03:23:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:31:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:32:45 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:46:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:46:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:46:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:46:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:46:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:46:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:33:49 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:33:50 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:33:52 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:33:52 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:52:02 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:52:10 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:52:11 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:52:12 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:52:13 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:52:14 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:52:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:52:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323ef8020b66a82bff905b3b8da692d6daf69a17f2740337bd5dde99dfe6da5`  
		Last Modified: Sat, 18 Jan 2020 04:18:27 GMT  
		Size: 301.8 KB (301758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ae6db3fff2d501fd9a1588acc79b2d1979a2a85c0dcd74a319491a1a58b7c6`  
		Last Modified: Wed, 11 Mar 2020 02:04:08 GMT  
		Size: 28.2 MB (28152901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45080882b2e9e075b004193066447a213219648430fa7e4c55b2ab9c6b9a3826`  
		Last Modified: Wed, 11 Mar 2020 02:03:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e226b432b6eddbc490b8471084c95d5a59dae345fa3c2885fdb08d6a65433`  
		Last Modified: Wed, 11 Mar 2020 02:03:59 GMT  
		Size: 1.9 MB (1891200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e625dccbc4bcb58d7656906703e8e5f06d79429f7b81d2b96ff04cae9837732f`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c2281e9cd39ddddc9657eb2933dfe185eb25f55e43684895bd36e8a88c8583`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac109756fff8eaf85044f6b348e8b45a5eb69b8682427cdf4cca8964a289bb2a`  
		Last Modified: Wed, 11 Mar 2020 02:54:23 GMT  
		Size: 133.6 MB (133597324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc241cb3a360c66b800938870f75ca9a93ea857c9167f64be480e2dfc8b356`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; 386

```console
$ docker pull plone@sha256:96eee82b92d5510c4995f0407bfdbfd0cfe125081a0627717fc2ae1b18f38aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165403033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6692c859cb160cb2c7f275d367a860b482904d3b2513e66796ac164b57ec94`
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
# Sat, 18 Jan 2020 01:56:42 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:07:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:26:52 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:36:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:36:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:36:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:36:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:36:53 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:10:06 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:10:06 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:10:07 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:10:07 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:20:18 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:20:19 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:20:20 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:20:20 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:20:20 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:20:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:20:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:20:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb66073d5c36a76368a9927f9e38d96d7f925b38af3fb4396b94e6e7a3a309`  
		Last Modified: Sat, 18 Jan 2020 05:37:35 GMT  
		Size: 301.9 KB (301915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91978cf8e552dc424fe9c7a0e279d06d85b0d8cd8ecb407fcbf1d4e6a5dc743`  
		Last Modified: Wed, 11 Mar 2020 01:50:12 GMT  
		Size: 27.1 MB (27101747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07420e8869fa8e2b11ba9b9ab6a81c54856f9ed3b85f885ec3b9ecc919509da2`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c379d154581bc5f5429c792cb92f3a67c45bd027bf4130cb67a4e81ca90e7`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 1.9 MB (1890900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc3dc2bbf9b0e01f46c33752dbbf0861abd02214f0fa4c0f527d43d3185957d`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ae7fdbd0b57d5d5fc3571571121f23c7a72fe7bfa8ea007eea322e83e4792`  
		Last Modified: Wed, 11 Mar 2020 02:21:23 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca93f91c8cf90ee1468f466b73db05b55b09520a045b2843a4fdfd30710b93`  
		Last Modified: Wed, 11 Mar 2020 02:21:57 GMT  
		Size: 133.3 MB (133296714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47476cde9a33c03b602fee9920dfeeec484c0f4e36d7fe94421ec7bdfe33bec7`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:5091df027d694226adf6599fa2b46749049efb65c6d0f421c54ed692a134b881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168951697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50cb00ee5f8cd912f11c217ae2f432513342ed9c3d563ae94409789a384e5a2`
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
# Sat, 18 Jan 2020 04:57:48 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:06:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:22:59 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:35:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:35:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:35:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:35:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:35:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:35:43 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:35:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:35:39 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:35:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:35:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:53:22 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:53:31 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:53:34 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:53:37 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:53:41 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:53:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:53:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d4344e21f41e55783663900e987c11ef2a6b1168de19ae63f1e05009e4eae`  
		Last Modified: Sat, 18 Jan 2020 05:45:37 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997052e9d9d744aba0e068db207eeb61eaa721ae09904ce3c203df4e1088408`  
		Last Modified: Wed, 11 Mar 2020 01:52:37 GMT  
		Size: 29.6 MB (29601503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76109d56f0386d8030cb0e3532a1aba32698bda6498c8b8f0e47b733d34b54`  
		Last Modified: Wed, 11 Mar 2020 01:52:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027cf2e6261a311500aab624108c2403b01d6100404370e3b5cfa3e759597fd`  
		Last Modified: Wed, 11 Mar 2020 01:52:30 GMT  
		Size: 1.9 MB (1891099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a4297dc1e9435d804b5af7fc2cbac58ddc1af9eeab0b3cb1b94369e440f97`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951daf23dd61a7c9e21936160861cddcd504308e04a4ca81f9952abcc6814e3`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c9333a69e536301bd60e001f4e5b88c7fb88e7fa6bc624409395bb5a208fe4`  
		Last Modified: Wed, 11 Mar 2020 02:56:33 GMT  
		Size: 134.3 MB (134327723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eac9ab10fddc9dba9ec26c3cd340093aff28eac163a2cbe57067ebdbbabe`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; s390x

```console
$ docker pull plone@sha256:3589edb381d0570ac641b4a8d0a8cd0a493e7285eac9275e4e22a46da86ed2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167893238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc12fdb7579ed701d648ffc9ea4636149346b699cc98589581a2769ffbfcae12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:52:22 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:52:23 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 01:56:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 18 Jan 2020 01:56:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:02:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:02:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:52:22 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:26 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:31 GMT
CMD ["python3"]
# Fri, 06 Mar 2020 23:30:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 06 Mar 2020 23:30:07 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 06 Mar 2020 23:30:09 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 06 Mar 2020 23:30:10 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 06 Mar 2020 23:37:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 06 Mar 2020 23:38:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 23:38:23 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Fri, 06 Mar 2020 23:38:24 GMT
EXPOSE 8080
# Fri, 06 Mar 2020 23:38:25 GMT
WORKDIR /plone/instance
# Fri, 06 Mar 2020 23:38:25 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 06 Mar 2020 23:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Mar 2020 23:38:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2a03efad4a7a2934aa60870dd9847c7c02f10dcbbd1614ea32e83c78531ba2`  
		Last Modified: Sat, 18 Jan 2020 02:16:42 GMT  
		Size: 301.8 KB (301798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627e873630aec7205c7b8e4f1025c14b29c11134532107ac214bb0646e89ad`  
		Last Modified: Sat, 18 Jan 2020 02:17:03 GMT  
		Size: 28.9 MB (28940433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1052253c74f387f87f6ac8e43dc4e0dbc66ee4ea50dc26d9b6bb9bce0415d7`  
		Last Modified: Sat, 18 Jan 2020 02:16:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406603440045cdce1ff839ea8eb3f9ebf716cd7daa1977ac349b7c8cbfd3098`  
		Last Modified: Thu, 06 Feb 2020 00:55:22 GMT  
		Size: 1.9 MB (1892187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89906eb9051286a6f61393b0fdc29cbe1a319a8e92321e967e25f372742aae6`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ee2dd5709fd6ed2a54c89001cf1f401de53a1c1dd8b885a37d59faa24a14c`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f47382a3d80c83b2459b21f836eff7cbce5b520f1a972fbdf10d1bbf0f89f2`  
		Last Modified: Fri, 06 Mar 2020 23:58:42 GMT  
		Size: 134.2 MB (134171528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279fcc4ee668ab6054f985db3e9340958850e39f68c4384f63e86ce447df4a0b`  
		Last Modified: Fri, 06 Mar 2020 23:58:36 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
