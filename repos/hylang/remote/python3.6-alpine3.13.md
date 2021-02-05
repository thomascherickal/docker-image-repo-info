## `hylang:python3.6-alpine3.13`

```console
$ docker pull hylang@sha256:2909fc7e1dbc583c22cc3f8ea6cf54f8ce2f67d3d7658a9e4f74bb841600d61c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:python3.6-alpine3.13` - linux; amd64

```console
$ docker pull hylang@sha256:0f7d7af6e97f5e68cd2c18c157ede7b673cd4e44c9e7edd8f7d72a64605bae9f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18258455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715c7716794e8cf9057dd0b114e94cdb93a5cdb956cca200388c7e166ad7c442`
-	Default Command: `["hy"]`

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
# Thu, 04 Feb 2021 01:42:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 01:56:30 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:06:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:06:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:06:43 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:06:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:06:43 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:06:54 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:06:54 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:20:55 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:21:01 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:21:01 GMT
CMD ["hy"]
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
	-	`sha256:1cf32de05765849edc829729a1a4d8c34cd621d4bccf3832bb809c1e1e6e1bd6`  
		Last Modified: Thu, 04 Feb 2021 02:10:26 GMT  
		Size: 10.2 MB (10189896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5818ae83b3016ae4364318131a365a4a2b69369cef68a0e3680b8cd785da93f3`  
		Last Modified: Thu, 04 Feb 2021 02:10:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4c65e1344cabd0af4b099ff1dc31de4dfc757f4699a1ab32c1af7c5d94f6b9`  
		Last Modified: Thu, 04 Feb 2021 02:10:25 GMT  
		Size: 2.2 MB (2163753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eda14737a5edd010366b14dc2b23353a35dd7930eef0dbb3bb35351085bfa6`  
		Last Modified: Fri, 05 Feb 2021 00:23:00 GMT  
		Size: 2.8 MB (2812051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.6-alpine3.13` - linux; arm variant v6

```console
$ docker pull hylang@sha256:dafb963aa8b1c434166e44b6977130a5c2c89f483b0bb607d2f096f782e09cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17681601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6260855f6d31d480e6a8b20281283dac9677edb4159c621577c612ec23d9ca8d`
-	Default Command: `["hy"]`

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
# Thu, 04 Feb 2021 01:55:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 02:11:48 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:20:46 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:20:49 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:20:50 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:20:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:20:51 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:21:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:21:08 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:01:56 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:02:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:02:09 GMT
CMD ["hy"]
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
	-	`sha256:ec23c15a3588b94c59dd36acaf40637f14b1c929b01ad39ab9c44bcb2f919203`  
		Last Modified: Thu, 04 Feb 2021 02:23:03 GMT  
		Size: 9.8 MB (9801484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6dfa2b64818cd407c56dd9aa09406a44b668c82f31c8935798c22f1a21ce84`  
		Last Modified: Thu, 04 Feb 2021 02:23:00 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4ba51cda564808b9898eb94a22895f291f48ee7fa0676c0cf53cdf1911a74`  
		Last Modified: Thu, 04 Feb 2021 02:23:01 GMT  
		Size: 2.2 MB (2164068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533340fd92996742c28168cd95903ae8247d8fe449b66069dfebefa4b2ed2387`  
		Last Modified: Fri, 05 Feb 2021 00:03:41 GMT  
		Size: 2.8 MB (2812663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.6-alpine3.13` - linux; arm variant v7

```console
$ docker pull hylang@sha256:ac8263a2699e4480c13e0148fa9d6bebee0b0833a0d6159c3b6242f8ecd0f35d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17035477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd71cbb78313254779fca2ee95da6ff23d1549c35b35e9b69054376878a8eea`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:48:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 02:12:09 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 02:20:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 02:36:43 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:44:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:44:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:44:38 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:44:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:44:39 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:44:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:44:53 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:02:09 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:02:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:02:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0855e8dcd0d27ddf9d5fa5df6cb906b256571a6ae0277cfc02d9d6368683786`  
		Last Modified: Thu, 04 Feb 2021 02:47:44 GMT  
		Size: 280.5 KB (280541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a17f4bdf44ffd0e0eaadc8f7e396809f66f23e9ad5aeb3262a33aac44f1741`  
		Last Modified: Thu, 04 Feb 2021 02:48:19 GMT  
		Size: 9.4 MB (9354591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c208ffebf6325a1d8383791ac1fec524a4b89393a2062166d53b7b8feea4e1`  
		Last Modified: Thu, 04 Feb 2021 02:48:17 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005ab9d97551a3ccc43a3f6c2a2f82867a4cb0f7daa01367d70bd331b10ef8f1`  
		Last Modified: Thu, 04 Feb 2021 02:48:17 GMT  
		Size: 2.2 MB (2164025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cf653dc577c27fc4ddce99aac58472ea418681de894a95e23d27b0d4e8db1a`  
		Last Modified: Fri, 05 Feb 2021 00:04:30 GMT  
		Size: 2.8 MB (2812530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.6-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:1f101f1bfe84ba300d90f1084c37c5ed17c8f051d42b00a7c8d99d1ddf18474e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.2 MB (18248787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba7f1e5260b4b2d086064e50f52542a440dbc55a8e6d79a083272976eba7c54`
-	Default Command: `["hy"]`

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
# Thu, 04 Feb 2021 01:59:19 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 02:15:04 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:23:03 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:23:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:23:06 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:23:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:23:08 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:23:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:23:20 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:41:26 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:41:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:41:37 GMT
CMD ["hy"]
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
	-	`sha256:2742b5205dcc793be598492bfb7f903cacd23620ff159a1fd86cdb37a7d264fd`  
		Last Modified: Thu, 04 Feb 2021 02:26:42 GMT  
		Size: 10.3 MB (10279126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04aa8bfb18afe6315bc4b0ff9aee32a784423fd8bec90eb0c891043e2de343c`  
		Last Modified: Thu, 04 Feb 2021 02:26:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e74b38902c1d009e813f58a8d883df390246935b5705d53527c56d0f2e7888`  
		Last Modified: Thu, 04 Feb 2021 02:26:40 GMT  
		Size: 2.2 MB (2164031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83bb5baab6d290ab6a7eee5077fddb5cbdf08e19e70aff73dffc18756da15b`  
		Last Modified: Fri, 05 Feb 2021 00:44:12 GMT  
		Size: 2.8 MB (2812566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.6-alpine3.13` - linux; 386

```console
$ docker pull hylang@sha256:1e12975f87d519b23bdad2ddba0b7511964ed80b24014fe6a200de78a4dfb9d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18440082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923117fb78ae1ce7fffa164a60db68ed90caeda07e68bdac82d5c79fdbb222d2`
-	Default Command: `["hy"]`

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
# Thu, 04 Feb 2021 02:23:22 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 02:34:52 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:43:59 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:43:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:44:00 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:44:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:44:00 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:44:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:44:08 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:39:27 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:39:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:39:33 GMT
CMD ["hy"]
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
	-	`sha256:8d558e1827fd6323d3cf041d31e1abc0738495f97e7000d35eee30407b5aa17d`  
		Last Modified: Thu, 04 Feb 2021 02:46:55 GMT  
		Size: 10.4 MB (10364565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6db73902b361deae19aed30840690ad5f63498ad5a3c5b281084d25c23a5c9`  
		Last Modified: Thu, 04 Feb 2021 02:46:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a624032e241b70c80b0c82a8b85a2de5252d8b55fc983435dd3c3d732a2ab867`  
		Last Modified: Thu, 04 Feb 2021 02:46:53 GMT  
		Size: 2.2 MB (2163670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b82956c08b2fe14060cd24550e4563542be158fc995d8eb24221a2fdd9f4ce`  
		Last Modified: Fri, 05 Feb 2021 00:41:36 GMT  
		Size: 2.8 MB (2812238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.6-alpine3.13` - linux; s390x

```console
$ docker pull hylang@sha256:6df33001cad5545c00e72ae25142c3d59b6b744733be0fd348d9150b336533dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18050072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bf6debcf745fcef936a99525e2c900e0dd5ea7da798e83db951ec202c951e2`
-	Default Command: `["hy"]`

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
# Thu, 04 Feb 2021 01:53:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 04 Feb 2021 02:01:20 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 04 Feb 2021 02:07:19 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:07:21 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:07:22 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:07:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:07:23 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:07:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:07:31 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 06:55:53 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 06:55:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 06:55:58 GMT
CMD ["hy"]
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
	-	`sha256:860a8f7683f40344f507a1935773252449aa77c6b4824385039dcdc594a5e1a4`  
		Last Modified: Thu, 04 Feb 2021 02:26:02 GMT  
		Size: 10.2 MB (10189682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201bc8458e218d7eae00c69706cacd72d4efedc61d6f388383ec448e5f6c4ac`  
		Last Modified: Thu, 04 Feb 2021 02:26:02 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c37b40ffda13b0cef2de0daf54be0e1db8e68ecc3f2dfe4d9c38299ed0633f3`  
		Last Modified: Thu, 04 Feb 2021 02:26:02 GMT  
		Size: 2.2 MB (2163911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403035b3b5f1f264d7e328e30a2ee4c47ecb607e08b040e97b207a2d7871a71f`  
		Last Modified: Fri, 05 Feb 2021 07:10:19 GMT  
		Size: 2.8 MB (2812484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
