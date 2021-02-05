## `hylang:python3.7-alpine`

```console
$ docker pull hylang@sha256:7128482529e986d39fd3a806d145d0b903013d1944eb55daf6402c600bdf44aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:python3.7-alpine` - linux; amd64

```console
$ docker pull hylang@sha256:83cd74c416756ed413061480c1b2f8d0ca632af5d01ae5e4d91d2686cdde8377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18649636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee265b055e56a4b530db0f3107474982f2dc6c721a7aa5150f18124c7222f15`
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
# Thu, 04 Feb 2021 01:42:57 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 01:55:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 01:55:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 01:55:44 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 01:55:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 01:55:44 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 01:55:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 01:55:51 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:20:32 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:20:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:20:38 GMT
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
	-	`sha256:5c0d1f839dbc3575d2a08ab3fb2fb3329cb5462ffc4861ae3d93c8cd1deb935a`  
		Last Modified: Thu, 04 Feb 2021 02:10:14 GMT  
		Size: 10.6 MB (10566142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c078d76f332bb5be6620b85b7c37cf240de86015c45c4f95e5587a81fe25cfb`  
		Last Modified: Thu, 04 Feb 2021 02:10:12 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb33935d71661812e92aea087c722736df4e164558f6a6427b58671cc372ea0a`  
		Last Modified: Thu, 04 Feb 2021 02:10:12 GMT  
		Size: 2.2 MB (2163656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc78854cc12088aa4db33212715e7907dfce21dc238ca04ba396da7c97fb7b`  
		Last Modified: Fri, 05 Feb 2021 00:22:47 GMT  
		Size: 2.8 MB (2827083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; arm variant v6

```console
$ docker pull hylang@sha256:a6ea35f94eabd098336e0a2c76e0752516d23dec0eea9dc73704a2106abd7cb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18081935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22671fa8961c1218881b0f4174cd4ddd63dbbbbe7f5976f7a82465289cd791a`
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
# Thu, 04 Feb 2021 01:55:07 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 02:11:09 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:11:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:11:14 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:11:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:11:16 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:11:31 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:11:33 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:01:32 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:01:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:01:45 GMT
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
	-	`sha256:9ab4a019543ca8b96e7ff27e5fe4343fa3463455a46241c138022e51421c9a78`  
		Last Modified: Thu, 04 Feb 2021 02:22:51 GMT  
		Size: 10.2 MB (10186775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd206978566b23fdfa3aa04d799904d222a06fc1d3277fdc00395048c8685a1`  
		Last Modified: Thu, 04 Feb 2021 02:22:48 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172f30b5bc870788e06a34afb0d5f89e5e8912231303e6cc0bb1d874d56cc856`  
		Last Modified: Thu, 04 Feb 2021 02:22:49 GMT  
		Size: 2.2 MB (2164057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a454ceca59fc4d146a95bd3b5f600b4366a833d1e0d1389308391d43e60b2db`  
		Last Modified: Fri, 05 Feb 2021 00:03:25 GMT  
		Size: 2.8 MB (2827716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; arm variant v7

```console
$ docker pull hylang@sha256:ed6e5d2191beaf36b02203e4399399a7d16d4c16c26e339f39f84c74f37939e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17419980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5d1fb3b88d4d42a90850a87ea60759bc078c4fc2ce5f0bce5e0c1c21692813`
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
# Thu, 04 Feb 2021 02:20:58 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 02:35:44 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:35:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:35:47 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:35:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:35:49 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:36:01 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:36:03 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:01:31 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:01:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:01:44 GMT
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
	-	`sha256:e5f78a4ee2518167da97f6bf2344350a2a1921cf881ce1693b97a52b3521d4e5`  
		Last Modified: Thu, 04 Feb 2021 02:48:04 GMT  
		Size: 9.7 MB (9724010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64f6f15d172b462a690d93396c37c7d0d94cf7510e7c02b4dbac0e399e96d6`  
		Last Modified: Thu, 04 Feb 2021 02:48:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410420d503517f6a18376d21f6a2a9ddb98af5cc5894d173b8f1362a68dd0ad5`  
		Last Modified: Thu, 04 Feb 2021 02:48:02 GMT  
		Size: 2.2 MB (2163924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1189ad0c142e31f37374269ca583a98b702b4cced291047e52090fdb1905829e`  
		Last Modified: Fri, 05 Feb 2021 00:04:08 GMT  
		Size: 2.8 MB (2827713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:94aa630486b5fead0427b462d000f6aa48ff4f986d27968427f62e396355b010
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18653360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f60875d517e224da6bb1d85965e5b279c53559ed5523ff206d6c4a7a4fc935a`
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
# Thu, 04 Feb 2021 01:59:20 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 02:14:17 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:14:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:14:20 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:14:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:14:21 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:14:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:14:34 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:40:48 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:41:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:41:01 GMT
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
	-	`sha256:f3bcd368b0f75fcc09458edb6297fae542de4ecd2d21b01a7056bfc267fe7a42`  
		Last Modified: Thu, 04 Feb 2021 02:26:26 GMT  
		Size: 10.7 MB (10668640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e65c2cc717ad8d60c6d5d17039235a6d68922988e1452593f45b452c121a10`  
		Last Modified: Thu, 04 Feb 2021 02:26:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2255574d144994c236b05d3e8e58205ac4b98e45c03bb4dea1773fec27b8eb9`  
		Last Modified: Thu, 04 Feb 2021 02:26:24 GMT  
		Size: 2.2 MB (2163999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d848e2e77b74d878be781b5d04488d1088732e082a223ca12fb7610f6b5816`  
		Last Modified: Fri, 05 Feb 2021 00:43:53 GMT  
		Size: 2.8 MB (2827656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; 386

```console
$ docker pull hylang@sha256:25cd7f2c0c258e8347c354144f31f55677fc780dbcb9a43fcda5921a546f2880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18844419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b08d722892249828737a9ab5af5e15e1faf766a845c686a85652040cc67dcbf`
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
# Thu, 04 Feb 2021 02:23:22 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 02:34:19 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:34:20 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:34:20 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:34:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:34:21 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:34:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:34:28 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 00:39:05 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 00:39:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 00:39:10 GMT
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
	-	`sha256:0b7ded0d70ddf7a17e82c868506e9a857c2639d4d1898d773302223599ecf4b9`  
		Last Modified: Thu, 04 Feb 2021 02:46:42 GMT  
		Size: 10.8 MB (10753987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d270f07f9449788510b91a50eee3cc318377898e4988805d025463be2e836838`  
		Last Modified: Thu, 04 Feb 2021 02:46:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1490f7881cd10627af2ef81e79bf0dea8fe588150a6a49fd42758f537a849d11`  
		Last Modified: Thu, 04 Feb 2021 02:46:40 GMT  
		Size: 2.2 MB (2163680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8ce53cc7bb77810eca92f7d9e2a1ec61bd6ef1ae32bd47291d0bada5befeaa`  
		Last Modified: Fri, 05 Feb 2021 00:41:20 GMT  
		Size: 2.8 MB (2827142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; ppc64le

```console
$ docker pull hylang@sha256:c4d69a29a0c9de9bd2f8be0190a8e4b753ccb1563a65d144d707be0b5300e935
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19512984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31de8f7b3fc40ee08ca454f0aab43f5ed0bd438fd0705a9499e3e8384ea9059`
-	Default Command: `["hy"]`

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
# Thu, 17 Dec 2020 10:16:17 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 10:16:21 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 10:28:32 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 10:28:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 23:03:00 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 23:03:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 23:03:15 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 23:04:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 23:04:27 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 23:39:38 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 23:40:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 23:40:23 GMT
CMD ["hy"]
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
	-	`sha256:6af9699de8d75a93c512e5e9449eece88fb05cb734010ceddd9f2f2704ed64e7`  
		Last Modified: Thu, 17 Dec 2020 11:04:18 GMT  
		Size: 11.4 MB (11432316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949f5b60a22c994ff3dd3cb1ff0ececdc0d7c4ef5e711bd5ffdcd267eaa88d0`  
		Last Modified: Thu, 17 Dec 2020 11:04:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6d9300404a8aebebe6bd5b4ac6bc6cda17990b06b5cea47858daaf1d81953b`  
		Last Modified: Mon, 01 Feb 2021 23:18:39 GMT  
		Size: 2.2 MB (2164112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d22d04d4124a4dd8c2b31a98ad4917698fec2a6e2d93373a7f279fa14ac00`  
		Last Modified: Mon, 01 Feb 2021 23:46:46 GMT  
		Size: 2.8 MB (2827895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine` - linux; s390x

```console
$ docker pull hylang@sha256:b93320687976af4b8c56b6adce6b16f89b24e8f7052ed60cdfdeb9caab7cd64d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18466938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916a1e6cf9e30644d2c2a2f98245cbf84a942258e27173f6fe605020895f97ec`
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
# Thu, 04 Feb 2021 01:53:27 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 04 Feb 2021 02:00:47 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:00:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:00:50 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:00:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:00:51 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:00:57 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:00:58 GMT
CMD ["python3"]
# Fri, 05 Feb 2021 06:55:33 GMT
ENV HY_VERSION=0.20.0
# Fri, 05 Feb 2021 06:55:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 05 Feb 2021 06:55:38 GMT
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
	-	`sha256:f953b69f973f306628ad45131f55a29171e2c244f2b7edfcea6871582a5e192e`  
		Last Modified: Thu, 04 Feb 2021 02:24:01 GMT  
		Size: 10.6 MB (10591570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b4ec0667fa32a2a1b59de7991065781dd67d6eaae448c1043e0d07f3edd4c5`  
		Last Modified: Thu, 04 Feb 2021 02:23:57 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7665e792947b85cf0ab27e2266627941480997f9c656cb03d0bf580ddcbe471a`  
		Last Modified: Thu, 04 Feb 2021 02:24:01 GMT  
		Size: 2.2 MB (2163938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f417909c546b567a1ccadc216c11d3e0e8ee5ed258202c6a41c49c84769a76f1`  
		Last Modified: Fri, 05 Feb 2021 07:06:15 GMT  
		Size: 2.8 MB (2827435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
