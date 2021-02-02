## `hylang:python3.7-alpine3.11`

```console
$ docker pull hylang@sha256:23a1d1701c6fa407822d95928fb12d58fdf60ec8bdc47d9e54dbb152198cacb5
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

### `hylang:python3.7-alpine3.11` - linux; amd64

```console
$ docker pull hylang@sha256:03f1a4ac7c8bd1636c01c79c8c15be38269c3f2cd18ee66ef75026075958d0af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18818186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1783cb849c61f1decbf5da6daac1c5802b3d5ad75a4d94ff36c092abc61c01b7`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:11:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 02:11:02 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:11:04 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 05:22:03 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 05:22:03 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 18 Dec 2020 05:58:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 18 Dec 2020 05:58:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 25 Jan 2021 23:31:42 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:31:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:31:42 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:31:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 25 Jan 2021 23:31:48 GMT
CMD ["python3"]
# Mon, 25 Jan 2021 23:53:43 GMT
ENV HY_VERSION=0.20.0
# Mon, 25 Jan 2021 23:53:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 25 Jan 2021 23:53:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233d96b408279e8bd3bc2420e6b070d4af559b50d792ee416508669ba88d68f2`  
		Last Modified: Thu, 17 Dec 2020 08:40:03 GMT  
		Size: 299.6 KB (299552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ad073959edc68f72e9a6d32cb8f9439f19c45eb5c736466860ed166465d3d7`  
		Last Modified: Fri, 18 Dec 2020 06:14:34 GMT  
		Size: 10.7 MB (10715228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d21bc3309f3343f3acab6ddd607a668dc5f90ef0e79bf9ffb6ba875708ee440`  
		Last Modified: Fri, 18 Dec 2020 06:14:33 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce85c1471caf6f207884c198987f1dc1a0f6b5c13ab06e19589ebe985c717cf2`  
		Last Modified: Mon, 25 Jan 2021 23:36:28 GMT  
		Size: 2.2 MB (2162624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411ace6b8183820e747b0ff2a90247baeade8d9ca0c5bcd3c36566d890490af7`  
		Last Modified: Mon, 25 Jan 2021 23:57:30 GMT  
		Size: 2.8 MB (2825688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; arm variant v6

```console
$ docker pull hylang@sha256:09f0f6a74cd14cc88612b357df3ceeae5e95928b22f820d664797061cda6bbf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18298200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c25ced45ee0b0949f5c542379844967b89eb33926a6607f13744e3a229c35fdf`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:41:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:41:27 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:41:31 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 07:08:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 07:08:14 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 07:24:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 07:24:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:56:31 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:56:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:56:33 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:56:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:56:49 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 22:16:34 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 22:16:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 22:16:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f23ae38c65dbef0b3cc2ac2315aa2827f11bd8a88fb155443d02829807f61c`  
		Last Modified: Thu, 17 Dec 2020 07:45:24 GMT  
		Size: 299.9 KB (299908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4e32583c01930f4eca16719fff16b66caa734a4689b47a3dadb48e9d3e5954`  
		Last Modified: Thu, 17 Dec 2020 07:46:04 GMT  
		Size: 10.4 MB (10385869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381dfa0881bb647c04ee3567f500b3aa7018b9479784c406e1a14baa4f6c8063`  
		Last Modified: Thu, 17 Dec 2020 07:45:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9841c6bd7d3bc1025780fcdadb712409a32eab80a073fee2c4d68585b9ade`  
		Last Modified: Mon, 01 Feb 2021 21:59:41 GMT  
		Size: 2.2 MB (2164038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8ae83f3f8be958ce80adefa4bacbcaddd9b40693be80a87e24078d3b5de7d3`  
		Last Modified: Mon, 01 Feb 2021 22:18:56 GMT  
		Size: 2.8 MB (2827385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; arm variant v7

```console
$ docker pull hylang@sha256:f9cc10061c3c6458819ffec05691f359aa3ccfe738287bd136d4f79cab4d6567
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17296614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897e40d76dcfb3761e6fd437260488a3b7334a6a5c26993278e0dca43c74a0d0`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:28 GMT
ADD file:6757438ec5b22931a1c6a274c9c1eca94f0715a405d2ba91bd8b95704ba969ca in / 
# Wed, 16 Dec 2020 23:58:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:08:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 07:08:35 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 07:08:37 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 07:24:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 07:24:51 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 07:35:16 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 07:35:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 22:12:43 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 22:12:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 22:12:44 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 22:12:58 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 22:13:00 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 23:20:04 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 23:20:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 23:20:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:71728559ce1f58d5e0ef30be5b1d7628ff967d4038f9202818dd3d8c76feb8ab`  
		Last Modified: Wed, 16 Dec 2020 23:59:11 GMT  
		Size: 2.4 MB (2422964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508e3fb4c86f690902e4be263a6f51548be539bb932e2d1426e7c60f724e9678`  
		Last Modified: Thu, 17 Dec 2020 07:49:32 GMT  
		Size: 298.9 KB (298868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc378fea743532d1264b9a4d022eeed900bb62db8ea76a6013997f8bbb1e6d`  
		Last Modified: Thu, 17 Dec 2020 07:50:14 GMT  
		Size: 9.6 MB (9582843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae76f4ce41da69d7fa888e200dea3103f7ee91b6273fbfcab0c93526c213edf`  
		Last Modified: Thu, 17 Dec 2020 07:50:01 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37721841ba3859f28a6318d5a543f4387b9b0f53610e31a51be1e85cb8a2066`  
		Last Modified: Mon, 01 Feb 2021 22:20:01 GMT  
		Size: 2.2 MB (2164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62570f81a5af5fcd8dd8e97c9e48c16132d25091f594a45c3635bef84b2c5f9`  
		Last Modified: Mon, 01 Feb 2021 23:24:25 GMT  
		Size: 2.8 MB (2827590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:837bbec0946867275896f812c7bd266ed8e0a2c89f8d9f0f654c1111771400d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d183516ab9fb4c1a3a46d6635b1a967f168291f2949f7ef913831d5275952858`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:06:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 07:52:39 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 07:52:41 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 08:15:32 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 08:15:33 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 08:29:46 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 08:29:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 23:24:06 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 23:24:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 23:24:07 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 23:24:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 23:24:20 GMT
CMD ["python3"]
# Tue, 02 Feb 2021 00:59:25 GMT
ENV HY_VERSION=0.20.0
# Tue, 02 Feb 2021 00:59:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 02 Feb 2021 00:59:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b5f17f69216b30a243442af8849c15ecbff6a46a06cb002e9f03078ea87ace`  
		Last Modified: Thu, 17 Dec 2020 08:50:11 GMT  
		Size: 300.1 KB (300061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc6e226b868f5735c25e715f1bafec4cb2c0563556746b4e3a72ac13bdaa8d`  
		Last Modified: Thu, 17 Dec 2020 08:50:47 GMT  
		Size: 10.8 MB (10845600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad56faf1b2d40ee0010ac012bc8e1b881a030a6e77603687e5eb4dd4fbde5`  
		Last Modified: Thu, 17 Dec 2020 08:50:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee20da74c8f2ac296f61d1ff1a29f14f4d897098eddbf1eda906ac7ab230bcf4`  
		Last Modified: Mon, 01 Feb 2021 23:31:32 GMT  
		Size: 2.2 MB (2164060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2046b50b24c3346643cf56e3ac7a8287a647a0362158743b470ba9cd6be9fd5e`  
		Last Modified: Tue, 02 Feb 2021 01:04:20 GMT  
		Size: 2.8 MB (2827678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; 386

```console
$ docker pull hylang@sha256:442daf92f2a098ffc8e8eebb59d85cbb811c874644492cc40239dfb2e268e074
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (19035121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e2e0fc95183a744cfef03cb749fac445249ccd5c9b474db11e9e418f68fb761`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:39 GMT
ADD file:c8f5b26cfa9b90dfe6ca805f2101bd199c87b93faed2af74df0cbe54ea28fa6d in / 
# Thu, 17 Dec 2020 00:38:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:32:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:32:59 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:33:00 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 06:50:28 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 06:50:29 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 06:59:52 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 06:59:53 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:46:45 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:46:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:46:45 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:46:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:46:52 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 22:09:07 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 22:09:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 22:09:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:60519712d04c07db59906a2e14fa87c037b6504d612ba116ea1ef94ae08a650b`  
		Last Modified: Thu, 17 Dec 2020 00:39:32 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3a008c1853e538eeb067786c0c0e8bf4bbbb16d1061a9581d516516c0b927c`  
		Last Modified: Thu, 17 Dec 2020 07:17:08 GMT  
		Size: 300.3 KB (300253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb29592fa701fde387669204098bac6da81ff4bb037f6d00cac97737402f1b1`  
		Last Modified: Thu, 17 Dec 2020 07:17:35 GMT  
		Size: 10.9 MB (10933389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8833cf222ffdb897083bcf60edd8fa11421cc11bd5a65bbda77330f5b2b82b13`  
		Last Modified: Thu, 17 Dec 2020 07:17:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14202f2f552317d8a35652efaff8b0003d83a738f10586026518539a734f174`  
		Last Modified: Mon, 01 Feb 2021 21:51:40 GMT  
		Size: 2.2 MB (2163765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84735f1c0333f6afe5a4f5af6b65db4e4623ec0496a988ec7f7aad8812a414fd`  
		Last Modified: Mon, 01 Feb 2021 22:12:33 GMT  
		Size: 2.8 MB (2826971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; ppc64le

```console
$ docker pull hylang@sha256:085a0c8e04e5dcb56b3c086d3c8bb51b882650ce34a787a57484c7429f9c33ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19555172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bf310188810a94ecd25dc926080d24265e65219bdc81d8287dae4cc98a9eb8e`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Dec 2020 00:21:03 GMT
ADD file:4a7a7b8454234532546faed6d4d392f006f235e86744822034cb829a16205d11 in / 
# Thu, 17 Dec 2020 00:21:06 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 10:06:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 10:06:18 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 10:06:29 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 10:29:32 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 10:29:41 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 10:41:41 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 10:41:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 23:04:57 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 23:05:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 23:05:10 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 23:06:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 23:06:22 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 23:40:45 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 23:41:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 23:41:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2c090b1a59445fb94c5fb14edf51af12a8f8bc2259535b08191f26ea84a7bb05`  
		Last Modified: Thu, 17 Dec 2020 00:21:49 GMT  
		Size: 2.8 MB (2821993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722c5f720201e02b4b0bd8f3f88e7748788edba855ba946b75624a062ad0d51a`  
		Last Modified: Thu, 17 Dec 2020 11:03:52 GMT  
		Size: 302.4 KB (302427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d048dae347aea169ecd5e3ab59fa97b118d194e6e4ce10acc87dd30023efaae`  
		Last Modified: Thu, 17 Dec 2020 11:04:38 GMT  
		Size: 11.4 MB (11438546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f638af0fef64ece489310c77ddf8c5b0f1eaedc9379f427f4de046f06dbec0`  
		Last Modified: Thu, 17 Dec 2020 11:04:35 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b67924befdb9c5189227fdb04bf7f726b1524af6a07b1fa9efd20f84c10e84`  
		Last Modified: Mon, 01 Feb 2021 23:18:53 GMT  
		Size: 2.2 MB (2164096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f53dc57e35f46c68ad28110c5ccbc9b3de20fc5dc436d662fc2ad14607e048`  
		Last Modified: Mon, 01 Feb 2021 23:47:12 GMT  
		Size: 2.8 MB (2827879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.11` - linux; s390x

```console
$ docker pull hylang@sha256:4834dee11e09e8052e1c4a92655de6b1075dfd0ee183a260d9362eb6169af183
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18618738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc6a1a1a38fad2a87f0cee43523806cd6a9a90377602861743c3363488766c8d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:44 GMT
ADD file:9e0a7f4c5f520dabbf66a5d4312ceeb614fc5073fca7a248eb070cd99f4b75ff in / 
# Wed, 16 Dec 2020 23:41:44 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:41:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 08:41:57 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 08:42:00 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 09:01:59 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 17 Dec 2020 09:01:59 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 17 Dec 2020 09:12:19 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 09:12:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:50:50 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:50:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:50:51 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:50:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:51:00 GMT
CMD ["python3"]
# Mon, 01 Feb 2021 22:49:10 GMT
ENV HY_VERSION=0.20.0
# Mon, 01 Feb 2021 22:49:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 01 Feb 2021 22:49:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ae4c90d25da4580c1cd02a35a672d9113b17e063183b4148c463df4d33079192`  
		Last Modified: Wed, 16 Dec 2020 23:42:26 GMT  
		Size: 2.6 MB (2583287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf385f85cc27e1028f51bfcbffd968615b36b1a89bf0645688ccc820f958717`  
		Last Modified: Thu, 17 Dec 2020 09:30:04 GMT  
		Size: 300.1 KB (300135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f917d194f4f54a9f7a6718c97b2ed265bcdfcd01f0378b3cfb9af36fb1c01bed`  
		Last Modified: Thu, 17 Dec 2020 09:30:35 GMT  
		Size: 10.7 MB (10743990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f53631beabeae544dce1f594e7d541eec1da18e2d4422cbf454eb416f8deb48`  
		Last Modified: Thu, 17 Dec 2020 09:30:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2f08a24c54dadbd0ae45dc7ae6efecb3c065bed6d22703c6500a9ffe5a82cd`  
		Last Modified: Mon, 01 Feb 2021 21:55:27 GMT  
		Size: 2.2 MB (2163770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f0d4c56136e0a07930aa0bd4546322218142a1b448c7318d2d7bc4aa03b2`  
		Last Modified: Mon, 01 Feb 2021 22:53:13 GMT  
		Size: 2.8 MB (2827325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
