## `hylang:0-python3.5-alpine3.10`

```console
$ docker pull hylang@sha256:f217b044923f2c2d00bee0dc6dead61d841e11e69d4aff97050fb591b4e83191
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

### `hylang:0-python3.5-alpine3.10` - linux; amd64

```console
$ docker pull hylang@sha256:54ed48d2205376676ffc1adddda6acafa8a3e45cbcf487d596f392d54382f0d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32418487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98321d4eb07393bc4fb4b5133cfcdb590cfbc90f0eed8add43993c3fd15cfa`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 01:34:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 01:34:56 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 01:34:58 GMT
RUN apk add --no-cache ca-certificates
# Fri, 24 Apr 2020 11:05:43 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Fri, 24 Apr 2020 11:05:43 GMT
ENV PYTHON_VERSION=3.5.9
# Fri, 24 Apr 2020 11:12:04 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 11:12:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 11:12:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 11:12:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 11:12:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 11:12:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 11:12:12 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 11:21:09 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 11:21:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 11:21:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a80d14c35bdcf3182348df62dae02f393b19e47d873d74d008296c54b784602`  
		Last Modified: Fri, 24 Apr 2020 11:13:39 GMT  
		Size: 300.9 KB (300945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8888542c91391f74b7130d259654b212e13885e7c91493bf8e0e49f5c6e03780`  
		Last Modified: Fri, 24 Apr 2020 11:14:22 GMT  
		Size: 24.6 MB (24597901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5fa64dc693f68bd692079fd2df49843826e47731b98b44d078d865bb26f60d`  
		Last Modified: Fri, 24 Apr 2020 11:14:17 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59f6a8919b9187320013a432e29ade50b5f204a57675ae0343255d08c4c6d52`  
		Last Modified: Fri, 24 Apr 2020 11:14:17 GMT  
		Size: 1.9 MB (1891346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e8fa53440288c343d0ca3233b3a1a6284434ad5be9c499af91a6935863afcc`  
		Last Modified: Fri, 24 Apr 2020 11:23:20 GMT  
		Size: 2.8 MB (2832483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; arm variant v6

```console
$ docker pull hylang@sha256:f943241a6852cdabd2385547f7f357ce21b9007071e7c19b0beea53ebd3e0543
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30274971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffff27968a12254d52de10a1b041cc71b9c130ba3b1d7b09d8fbbd5f052e03e`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:38:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 20:38:45 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 20:38:48 GMT
RUN apk add --no-cache ca-certificates
# Thu, 23 Apr 2020 21:48:34 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Thu, 23 Apr 2020 21:48:34 GMT
ENV PYTHON_VERSION=3.5.9
# Thu, 23 Apr 2020 21:56:30 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 21:56:35 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 23 Apr 2020 21:56:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 23 Apr 2020 21:56:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 23 Apr 2020 21:56:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 23 Apr 2020 21:56:53 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Apr 2020 21:56:54 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 01:52:06 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 01:52:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 01:52:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57a40f256a36351da43ee93685238f00bc7c6b0457d57f43b6de40365dc27eb`  
		Last Modified: Thu, 23 Apr 2020 21:58:11 GMT  
		Size: 301.3 KB (301254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfaac61d6a94f1e1dd5c8dcad211aeaed39f87bd21de0b2b6452c023402c130`  
		Last Modified: Thu, 23 Apr 2020 22:00:11 GMT  
		Size: 22.7 MB (22675992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e932cade3dec134779778f5069f3ee36842a97f30ebbad464efb59dfdf553ce9`  
		Last Modified: Thu, 23 Apr 2020 22:00:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe045241b8cc0055fd53735f352331b342769d89453caa6ecf2a3d72d36d36e`  
		Last Modified: Thu, 23 Apr 2020 22:00:05 GMT  
		Size: 1.9 MB (1891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f5cc1d90825cdc0e01eb1cd016107bb49723830641db66d05c256b9d2dfcdf`  
		Last Modified: Fri, 24 Apr 2020 01:54:31 GMT  
		Size: 2.8 MB (2833373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; arm variant v7

```console
$ docker pull hylang@sha256:4e13475696725b9388de6cfd853f15c7ebfea8c1131941304511206cdb80a3f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29691602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f44f9a3de72496abd3ae36d3d516fcc2b3d9adefa13f24dec96e6db858543b`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:28:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 04:28:07 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 04:28:10 GMT
RUN apk add --no-cache ca-certificates
# Fri, 24 Apr 2020 08:20:34 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Fri, 24 Apr 2020 08:20:34 GMT
ENV PYTHON_VERSION=3.5.9
# Fri, 24 Apr 2020 08:27:58 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 08:28:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 08:28:01 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 08:28:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 08:28:02 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 08:28:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 08:28:15 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 17:38:08 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 17:38:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 17:38:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce92f9b10e33d2ac10e4a2982e1b92743ef36e12ec1e8ba8ef66ae7a125936a`  
		Last Modified: Fri, 24 Apr 2020 08:30:19 GMT  
		Size: 300.1 KB (300138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3b79d43eac93d3feadf9481ba34e25cbf97c97323391bdf3967d9dac643a8d`  
		Last Modified: Fri, 24 Apr 2020 08:32:10 GMT  
		Size: 22.3 MB (22287440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0190631f1ec388719d75b9ba1f4a629c7794eddbd2727b040222a46a0667f2a`  
		Last Modified: Fri, 24 Apr 2020 08:32:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8e1640cfac25d8a1eca1838a22bfb2746bc84da63198b581e4c1e7085e1fe8`  
		Last Modified: Fri, 24 Apr 2020 08:32:04 GMT  
		Size: 1.9 MB (1891606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8796a6defeb22117d8b544e202c7ed41fd39c9171de06f9068d31cae5a77c2a`  
		Last Modified: Fri, 24 Apr 2020 17:40:20 GMT  
		Size: 2.8 MB (2833549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:fc274d0133ab360b82ea801bc452ad10fe02cec9a06b1ca79e31118c54cfc5a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31818429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bc834d7104a2db055a860892696b15b3d333c195cfc32dc89b58ba19df55f7`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:16:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 07:16:39 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 07:16:41 GMT
RUN apk add --no-cache ca-certificates
# Fri, 24 Apr 2020 08:16:05 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Fri, 24 Apr 2020 08:16:06 GMT
ENV PYTHON_VERSION=3.5.9
# Fri, 24 Apr 2020 08:23:14 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 08:23:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 08:23:17 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 08:23:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 08:23:18 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 08:23:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 08:23:30 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 08:31:28 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 08:31:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 08:31:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00770a9e6c343f414a2bac6b7ff8cb12c89d6b8559f1cb74ed38ea04ff029cd`  
		Last Modified: Fri, 24 Apr 2020 08:25:29 GMT  
		Size: 301.6 KB (301579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a5e61d4a47631476959cf4832a5710d7b29d01fd3eeee2ea3a3a7cae9ca1c5`  
		Last Modified: Fri, 24 Apr 2020 08:27:56 GMT  
		Size: 24.1 MB (24073128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a251383a435cb6795f5465b40e81aa309b510b6cc01c13e990b9a5b8efd9258`  
		Last Modified: Fri, 24 Apr 2020 08:27:48 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f460837181d1d11c7061d07fb726c9bda298f1cc00d803835e4eb55434d10e`  
		Last Modified: Fri, 24 Apr 2020 08:27:48 GMT  
		Size: 1.9 MB (1891688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b8805ab5867f52a0db757c3d1c670ebb3f7be9e02cce039775156327ebb1b9`  
		Last Modified: Fri, 24 Apr 2020 08:35:37 GMT  
		Size: 2.8 MB (2833069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; 386

```console
$ docker pull hylang@sha256:aab58a1de9fc119fb66b6401bc2c766e4e52dfc160e484788c117afce26ec621
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31052884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6fe44ba73a145b13fc4ee97a8c3e5df95f5b4e8964347d8c1fc1ed150cc1078`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 21:38:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 21:38:22 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 21:38:24 GMT
RUN apk add --no-cache ca-certificates
# Thu, 23 Apr 2020 22:35:41 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Thu, 23 Apr 2020 22:35:42 GMT
ENV PYTHON_VERSION=3.5.9
# Thu, 23 Apr 2020 22:43:07 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 22:43:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 23 Apr 2020 22:43:08 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 23 Apr 2020 22:43:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 23 Apr 2020 22:43:08 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 23 Apr 2020 22:43:16 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Apr 2020 22:43:16 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 04:01:14 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 04:01:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 04:01:19 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61cc54eae371e15077a5272fb58cfef3e4a13587edf5fe05700b05ee682c5cd`  
		Last Modified: Thu, 23 Apr 2020 22:44:54 GMT  
		Size: 301.6 KB (301596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb82cfb2ff1d7974116d2479e901ede23b88d7dba449e809a982be324c30ea2`  
		Last Modified: Thu, 23 Apr 2020 22:46:11 GMT  
		Size: 23.2 MB (23240051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad241af7a16dbbcaf8583dc95d7ba53941eafd873df7c9b9ee0b4702acfd3bf`  
		Last Modified: Thu, 23 Apr 2020 22:46:05 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261e6dc1c01e586aea45caf3174cdb549f62f995fd01fe692958508fddde357a`  
		Last Modified: Thu, 23 Apr 2020 22:46:06 GMT  
		Size: 1.9 MB (1891284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486ed699024cf0250275228002ee28cdaded58615d35356f4783034787143898`  
		Last Modified: Fri, 24 Apr 2020 04:03:18 GMT  
		Size: 2.8 MB (2832595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; ppc64le

```console
$ docker pull hylang@sha256:1a0a50c59fd5eaaef04a5d99d03467c216a15ae18d6139196bea6326000c9273
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33294844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902ee993dde6d1c1524b10353cb44bb00cc53e92e114310da3c5ce01a3302fa1`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:56:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 09:56:06 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 09:56:16 GMT
RUN apk add --no-cache ca-certificates
# Fri, 24 Apr 2020 10:58:31 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Fri, 24 Apr 2020 10:58:38 GMT
ENV PYTHON_VERSION=3.5.9
# Fri, 24 Apr 2020 11:06:13 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 11:06:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 11:06:27 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 11:06:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 11:06:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 11:06:58 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 11:07:01 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 15:23:10 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 15:23:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 15:23:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36408d0fc6e8604a4840728f6b4d11631e84283c697404c6f7487c1b60518036`  
		Last Modified: Fri, 24 Apr 2020 11:09:27 GMT  
		Size: 303.7 KB (303693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb189008195fead5cbf07a1fea83e21027ee9fb6c6ace9844bb86f2cfa421cb`  
		Last Modified: Fri, 24 Apr 2020 11:11:42 GMT  
		Size: 25.5 MB (25455945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be3914be2618808eb6b234f0cf081e6b30f672dc1130ac9c146ea16b22016c`  
		Last Modified: Fri, 24 Apr 2020 11:11:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128c5089c17868b2f112807b949b388d7956a1a8ea5c584fde90edbb873101fd`  
		Last Modified: Fri, 24 Apr 2020 11:11:36 GMT  
		Size: 1.9 MB (1891606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c078704f4459494fc7e5b9ec3f507ba5e2fa5cd48a72044c93db8e0f3035ffc7`  
		Last Modified: Fri, 24 Apr 2020 15:27:12 GMT  
		Size: 2.8 MB (2833412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.5-alpine3.10` - linux; s390x

```console
$ docker pull hylang@sha256:7f5cbeb0cdfd3765c0a8d801461b5892cc0c7d2deb781ba95665b21a8d2dacf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32327085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a0a02ce9e620ae423fdbcd5ba276a3d8588086281a51f8d212c1be09ff9eee`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 00:08:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 00:08:22 GMT
ENV LANG=C.UTF-8
# Fri, 24 Apr 2020 00:08:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 24 Apr 2020 06:31:31 GMT
ENV GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D
# Fri, 24 Apr 2020 06:31:31 GMT
ENV PYTHON_VERSION=3.5.9
# Fri, 24 Apr 2020 06:35:39 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 06:35:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 06:35:41 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 06:35:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 06:35:42 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 06:35:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 06:35:47 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 10:11:20 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 10:11:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 10:11:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9effbbafa6dfb00bba9beef1c64dca1e9ac011970f2065747370e7774a9109a7`  
		Last Modified: Fri, 24 Apr 2020 06:43:43 GMT  
		Size: 301.7 KB (301709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e48a0e8ddacf17823e5f177e9da6727279f56e84ec768d17f9f45a917d060a`  
		Last Modified: Fri, 24 Apr 2020 06:44:57 GMT  
		Size: 24.7 MB (24726488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6dbb24b7eae21f96db001a75879b33bddb09b699b503de86314313f65e9fb0`  
		Last Modified: Fri, 24 Apr 2020 06:44:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f35abeb4e1491fad2385aefffa04a724cdba5b8e2a8c5689eb7102fd2a2173`  
		Last Modified: Fri, 24 Apr 2020 06:44:58 GMT  
		Size: 1.9 MB (1891376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa54396567aae0c092f4ed4143bb6aac8218524ceec2fefe4b7b936c3d5fd32`  
		Last Modified: Fri, 24 Apr 2020 10:13:24 GMT  
		Size: 2.8 MB (2832806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
