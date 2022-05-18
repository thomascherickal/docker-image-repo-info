## `hylang:python3.7-alpine3.15`

```console
$ docker pull hylang@sha256:c939d577eecec51f78ce20c62727e140fe3fdd024ffe1150a52fc657bbcc827a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:python3.7-alpine3.15` - linux; amd64

```console
$ docker pull hylang@sha256:3f01126849dae6343380a3f4c54cdfdc04a8a7e95e2eba15507d58656bcfd30b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20439383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5668c0c0d6b35dc3f6bbdb1cb2aac26d76e49ba6622e887921a70e3c398d4b04`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:55:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:50:45 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 07:50:46 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 09:21:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 09:21:57 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 03:11:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:11:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:11:28 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:11:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 02:45:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:45:20 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:45:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:45:27 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:31:36 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:31:36 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:31:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:31:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ef3e6b7a02c0ce1d7d3ee96f273c2c5074b3f127082b4cd3f629f82097e1a8`  
		Last Modified: Tue, 05 Apr 2022 09:38:17 GMT  
		Size: 667.0 KB (667029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592c86358a0be3e5bea7de17e359984f3180e3e57aa18b5afb51cbffb6df7c71`  
		Last Modified: Wed, 20 Apr 2022 03:43:19 GMT  
		Size: 11.2 MB (11187621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb59fb21dd583d1d59b6815c76fb183a76fad49e34f19cb39a7f4b2d5310f8e9`  
		Last Modified: Wed, 20 Apr 2022 03:43:17 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f822da1bbc8ab19cc795ed92b43de6f1b8172ea157b1f7c50948907862f6f5`  
		Last Modified: Wed, 18 May 2022 02:53:26 GMT  
		Size: 2.9 MB (2874045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d496cc2ec25f6b950c0d34e46941e8d27fa9d307a9fd0ea0e595033b8028afb6`  
		Last Modified: Wed, 18 May 2022 04:36:26 GMT  
		Size: 2.9 MB (2895898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; arm variant v6

```console
$ docker pull hylang@sha256:05b7d9bb3c10fe3a7dda6a1df9fc1cfe57a21c5a00deead4213237ed686dd9c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19876583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe0e99fdcbd3a27677eb72e0f1fb9dda6642f7e733e7727fe558f67eef5ec57b`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:16:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:16:39 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 07:16:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 10:42:30 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 10:42:31 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 02:24:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 02:24:17 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 02:24:17 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 02:24:17 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 01:39:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 01:39:08 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 01:39:25 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 01:39:26 GMT
CMD ["python3"]
# Wed, 18 May 2022 02:42:56 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 02:42:56 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 02:43:04 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 02:43:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c148f0a21858ba6d892e5c2be6f7a4cdc7017f1eb8f0dfe07a2aa14cdcf6d2`  
		Last Modified: Tue, 05 Apr 2022 11:23:18 GMT  
		Size: 672.6 KB (672638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f09a1e40e800c344f5ecabb9bf8eb644ba792fe23855f582ea463cd67a1f7`  
		Last Modified: Wed, 20 Apr 2022 02:51:51 GMT  
		Size: 10.8 MB (10811640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202aa4bd8b580673b6efcef8722e0aad0aa358e9b99084a7a3eb2777a7942f80`  
		Last Modified: Wed, 20 Apr 2022 02:51:44 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadb642cf5b021fcf7092fcf81c7506cdd72491aa563aea6fe86adfa9c03eee1`  
		Last Modified: Wed, 18 May 2022 01:45:33 GMT  
		Size: 2.9 MB (2874069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b560dd8504cb5b324bfbfada50fc836a2e60e38f74c8af31cad20f33fda9ded`  
		Last Modified: Wed, 18 May 2022 02:47:59 GMT  
		Size: 2.9 MB (2896034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; arm variant v7

```console
$ docker pull hylang@sha256:83651e4157b223a45cf726304b713f9d19d0fda522471271e7da3cfa7206921f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19207655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad642ff93722cee41c25923634f3389c1556c41412cbb12ab08044ee21a86328`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:15:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 11:15:50 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:15:53 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 14:35:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 14:35:13 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 12:19:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 12:19:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 12:19:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 12:19:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 20 Apr 2022 12:19:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 12:19:53 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 12:20:07 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 12:20:08 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 19:27:54 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 19:27:54 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 19:28:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 19:28:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5594b60729afc7fdfa6de04dfddfc5560d7ca2510331911a8b6c27a5fd65f469`  
		Last Modified: Tue, 05 Apr 2022 15:18:31 GMT  
		Size: 664.5 KB (664505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66da00854c1e04d2bbf48b35b9887861ae1c28f55bbb4ce82e7a8bc5dd0a71b`  
		Last Modified: Wed, 20 Apr 2022 12:56:51 GMT  
		Size: 10.3 MB (10348937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ca92d0e8e711d848559deb0e5a99dc5b1d926e1643d5dcb664ddf872cb54c0`  
		Last Modified: Wed, 20 Apr 2022 12:56:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f958564d5b3b68efc21a69c30bd5e9c7e70f3352c83c6859e223a129c570520`  
		Last Modified: Wed, 20 Apr 2022 12:56:48 GMT  
		Size: 2.9 MB (2874073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145dde8205c352d54d8abd0c44a112b522aec9f311bd267c725b2e0e0965d2a7`  
		Last Modified: Wed, 20 Apr 2022 19:36:57 GMT  
		Size: 2.9 MB (2895587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:206c9c8d1b79d60f0bc75940025f208cf1befba6ad8aa57d9b2899a65b106124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20424539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18367ead591d1033f9b00e4db5f7aa72c1091bf18c9a6cea8b8b69533f517ba7`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:43:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:43:56 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:43:58 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 06:22:19 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 06:22:20 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 03:53:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:53:14 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:53:15 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:53:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 04:42:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 04:42:49 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 04:42:56 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 04:42:57 GMT
CMD ["python3"]
# Wed, 18 May 2022 05:45:43 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 05:45:43 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 05:45:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 05:45:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c8fe6b300068ece063b73d7ea69bef331e0698246ebbe2abe966cf6685e1ef`  
		Last Modified: Tue, 05 Apr 2022 06:41:57 GMT  
		Size: 668.4 KB (668392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb92912681d94b6426943674fb467c4e0cdac6bb51c376601eacbf2d077fa6c`  
		Last Modified: Wed, 20 Apr 2022 04:13:04 GMT  
		Size: 11.3 MB (11273875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5580f7d8d9399948904fcb4b8059417ac81165bc73529ce2bafcdb704df03c`  
		Last Modified: Wed, 20 Apr 2022 04:13:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b507acd5e10a78b32f77a73dca0fa6ee8da17ee657569086b078f450eeb147`  
		Last Modified: Wed, 18 May 2022 04:53:30 GMT  
		Size: 2.9 MB (2873507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed537904fd89a0d05d59605dbedeeda682417b9f810cf05597518e982c28f4f`  
		Last Modified: Wed, 18 May 2022 05:52:24 GMT  
		Size: 2.9 MB (2892058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; 386

```console
$ docker pull hylang@sha256:4dc816392f012e4a8f44e642a92c60bb3fd3cd4cb0f3d0ef19a000f17d35e648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20641819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b588599aa62a73f2d6b8ffaf4c37d76b58d127a73a17146e694d9d3c65612851`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:41:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:41:33 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:41:35 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 06:05:42 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 06:05:43 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 03:40:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:40:16 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:40:17 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:40:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:18:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:18:53 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:19:01 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:19:01 GMT
CMD ["python3"]
# Wed, 18 May 2022 03:49:10 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 03:49:11 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 03:49:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 03:49:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123e2fc95f4f26c5ef818012e9569da127091f4bda4bbd8d1b992ff1d9fca0f0`  
		Last Modified: Tue, 05 Apr 2022 06:24:17 GMT  
		Size: 674.8 KB (674790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f0e4f2e4201d4eeab7662782a694157c12975024f44783b09af5ea8fd25f0e`  
		Last Modified: Wed, 20 Apr 2022 05:39:33 GMT  
		Size: 11.4 MB (11382272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb9ff0c5a1b33ba979cbf208e7f5d6c9ab1f6572b446564d28f89f32e86fc5`  
		Last Modified: Wed, 20 Apr 2022 05:39:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c963600076a370a9046251cd3df617d7a008bce5643c913e24924f9fe8422`  
		Last Modified: Wed, 18 May 2022 03:30:01 GMT  
		Size: 2.9 MB (2873512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f5f0acd857409e805a3b80d51b412909295c5615616238a501a3cde54238da`  
		Last Modified: Wed, 18 May 2022 03:56:13 GMT  
		Size: 2.9 MB (2892040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; ppc64le

```console
$ docker pull hylang@sha256:dfa1f3fa7743dcb9c8f83194d4f044b6146c1fd389e16d43b3d41635de8ff74a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20724219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69f7c52d230d475208f575dc5ae97640035cb9920fe9decdaabed9d0ce59879`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:00:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 16:00:44 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:00:54 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 18:34:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 18:34:11 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 08:44:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 08:44:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 08:44:58 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 08:45:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 20 Apr 2022 08:45:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 08:45:07 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 08:45:24 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 08:45:27 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 16:07:16 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 16:07:24 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 16:08:01 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 16:08:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383b0511332251ebc07b3b84ac239f2c956371bd46dbe7229965dd10db503224`  
		Last Modified: Tue, 05 Apr 2022 19:05:19 GMT  
		Size: 676.5 KB (676534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ed11f14d4cdff58a3ef30ce0755c14c6e867ad5fb1d4738e1fc1ed1fce3a8`  
		Last Modified: Wed, 20 Apr 2022 09:12:35 GMT  
		Size: 11.5 MB (11466139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de93b3b78cc575fc0c2589154af5c1947aa3e8ab24af58884a9c89c76a4d826`  
		Last Modified: Wed, 20 Apr 2022 09:12:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18b884b979580bf22576675ff21a36203dfd644bc681b75c86a7a2a36f458ec`  
		Last Modified: Wed, 20 Apr 2022 09:12:34 GMT  
		Size: 2.9 MB (2874095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65ce36595fc1ad8dba67b8666dcfef62d6b9ba45a808c21d3944531af008f3`  
		Last Modified: Wed, 20 Apr 2022 16:16:37 GMT  
		Size: 2.9 MB (2896033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.15` - linux; s390x

```console
$ docker pull hylang@sha256:99ad52b29cc07029ee1fc33ce9533dbd7ee53eab0f57a4fc83a7265c0f3d72d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20247812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ec0023482a7f529b7cc575d8052e3001eee1c75a57d83c620f5cd0c24e328f`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:24:38 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:24:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 05:42:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 05 Apr 2022 05:42:14 GMT
ENV PYTHON_VERSION=3.7.13
# Wed, 20 Apr 2022 03:04:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:04:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:04:28 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:04:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:05:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:05:34 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:05:43 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:05:44 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:53:13 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:53:13 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:53:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:53:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e008f4836aadf966085bfc88ab008beb623e1f799da4ac849b1532735dc5b`  
		Last Modified: Tue, 05 Apr 2022 05:59:03 GMT  
		Size: 672.6 KB (672601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ed67ec8420fd6df7e63ae685fff5f6d929a95c97937240c122b2493aa4c693`  
		Last Modified: Wed, 20 Apr 2022 05:01:18 GMT  
		Size: 11.2 MB (11204866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e164502e34886bf3f8f7617c66395edcb5e4c8e1294b007859780f9ea542292`  
		Last Modified: Wed, 20 Apr 2022 05:01:17 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902c2e55800c57aad45b455fe26545008d378130d01b62f57dae0e0ac904d3da`  
		Last Modified: Wed, 18 May 2022 03:14:44 GMT  
		Size: 2.9 MB (2873967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba96b2d48e10dcb642db222854fc07e155bb773184c4f46b983c4bc0965b4772`  
		Last Modified: Wed, 18 May 2022 04:58:11 GMT  
		Size: 2.9 MB (2895773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
