## `hylang:0-python3.7-alpine3.10`

```console
$ docker pull hylang@sha256:1b2328e565021d6de277d897ef1f547bad1f8548178e94c3bb58d580e9e42206
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

### `hylang:0-python3.7-alpine3.10` - linux; amd64

```console
$ docker pull hylang@sha256:f32b5f3b93c02cd5890fac10f3297abe7e565d23f3424ae3ecb207a85521d3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36178023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c991e7845b2bc0dd3215ca34d36387cd59dfef93a4bc0fc4d1f9cf2cea3ed9`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:05:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 23:09:17 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jan 2020 23:09:19 GMT
RUN apk add --no-cache ca-certificates
# Thu, 23 Jan 2020 23:32:58 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:03:37 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:13:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:13:02 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:13:02 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:13:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:13:03 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:13:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:13:08 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:49:11 GMT
ENV HY_VERSION=0.18.0
# Wed, 11 Mar 2020 01:49:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 11 Mar 2020 01:49:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf8a687be7ffea0d5471a91e524515128c316739abda79ead8135ca464ea15`  
		Last Modified: Fri, 24 Jan 2020 05:53:56 GMT  
		Size: 301.7 KB (301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76509a1f14414b17442e11b1b9fa527335c81e5d04f96db8906f17735f05cf1`  
		Last Modified: Wed, 11 Mar 2020 01:16:48 GMT  
		Size: 28.5 MB (28474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d8543d55bde5650eea880dd753ea3c50f674818169d4a6f08debd616d3e71`  
		Last Modified: Wed, 11 Mar 2020 01:16:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b423a1c32f6e5bae675b63e9adc2d73e218ec3cad31dcac8b0b104a0367416`  
		Last Modified: Wed, 11 Mar 2020 01:16:43 GMT  
		Size: 1.9 MB (1890890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337385e6ac45c99f176c84875ec1a680f4e4c0b18916c6fa636706c6186a2eb`  
		Last Modified: Wed, 11 Mar 2020 01:50:45 GMT  
		Size: 2.7 MB (2723798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; arm variant v6

```console
$ docker pull hylang@sha256:b9d73626f44a5b2be739a714f2c11106cd015286ccd089126594848f6aca082a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33718939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1673b671a198fb2bc20dd8838bdb2d4e6848e0fd0100c5a0ed82b1264b78cab3`
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
# Thu, 23 Apr 2020 21:05:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Apr 2020 21:05:05 GMT
ENV PYTHON_VERSION=3.7.7
# Thu, 23 Apr 2020 21:20:02 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 21:20:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 23 Apr 2020 21:20:08 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 23 Apr 2020 21:20:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 23 Apr 2020 21:20:12 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 23 Apr 2020 21:20:24 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Apr 2020 21:20:25 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 01:50:32 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 01:50:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 01:50:50 GMT
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
	-	`sha256:51a4023b1b41dc35f65bd12ad8bd1b0cb0912cb402b235a060099096c2376acf`  
		Last Modified: Thu, 23 Apr 2020 21:59:00 GMT  
		Size: 26.2 MB (26228669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2786fd7c2cb3428ea81bc6b8dcd8f2c2c71bf8457f903a078a9163070504e46`  
		Last Modified: Thu, 23 Apr 2020 21:58:51 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b3ede5cbe9ab5f4821c531a244231f506e40dd490ea38d797e3036d77d03cc`  
		Last Modified: Thu, 23 Apr 2020 21:58:52 GMT  
		Size: 1.9 MB (1891500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d30ef23838a0090c91e6eef5245e0f88ec2961f0dd3646272f9ca1a2ff3a93`  
		Last Modified: Fri, 24 Apr 2020 01:53:39 GMT  
		Size: 2.7 MB (2724771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; arm variant v7

```console
$ docker pull hylang@sha256:3c31640a3cee650e39d7db2e2ce136129f6dbce27ac1fe15e5e3453ebb6e9059
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33012178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9777d32a32114f69a88764883cbd9d4d9920f4122ac58c240cb629e1a015933b`
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
# Fri, 24 Apr 2020 04:49:55 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Apr 2020 04:49:56 GMT
ENV PYTHON_VERSION=3.7.7
# Fri, 24 Apr 2020 05:04:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 05:04:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 05:04:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 05:04:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 05:04:47 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 05:05:04 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 05:05:05 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 17:36:30 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 17:36:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 17:36:46 GMT
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
	-	`sha256:0f03889ddd8102af7f3a45cb91db6d4ac83fd6356de4bc2fec3dc081883346ff`  
		Last Modified: Fri, 24 Apr 2020 08:31:13 GMT  
		Size: 25.7 MB (25716797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02802567f860f33e39bb97188e2bbf12cc23792ce98287dbdad64e29bf424397`  
		Last Modified: Fri, 24 Apr 2020 08:31:04 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93741ff23b265a2c85f0bb1684e28d4def6305f23f26598871a280a73be2c5db`  
		Last Modified: Fri, 24 Apr 2020 08:31:05 GMT  
		Size: 1.9 MB (1891522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8930595f6f59613d0cf2858fbbd7368a320180884733ae8ed3608359f3d5e5b1`  
		Last Modified: Fri, 24 Apr 2020 17:39:51 GMT  
		Size: 2.7 MB (2724849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b102d18e4ae1c75332f915c984a9bda57ca1e04d72a0bb84fd1fca5a42430308
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35526794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623eb51ead18309900c01fbc038ac72f5f7eb1921e12bcf88ad03c633d7e6317`
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
# Fri, 24 Apr 2020 07:38:45 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Apr 2020 07:38:46 GMT
ENV PYTHON_VERSION=3.7.7
# Fri, 24 Apr 2020 07:51:51 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 07:51:53 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 07:51:54 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 07:51:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 07:51:55 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 07:52:05 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 07:52:06 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 08:29:54 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 08:30:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 08:30:04 GMT
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
	-	`sha256:b7e9089bda2b56b996208b9c59243499d3cd3f34480db797211e0e74b9d84ed5`  
		Last Modified: Fri, 24 Apr 2020 08:26:31 GMT  
		Size: 27.9 MB (27890194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5971df9506575ee2d8a16fb4948e1ca894c113c9abeda2b3f42699d37d7956`  
		Last Modified: Fri, 24 Apr 2020 08:26:21 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffc044e08ebbc663e4d9af5b5765b8961e539f5a50b451451ea641fc45f3401`  
		Last Modified: Fri, 24 Apr 2020 08:26:22 GMT  
		Size: 1.9 MB (1891493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1e85af1030647daef067094d6cdb0ed285c22804907f91a50b04d82f876cb8`  
		Last Modified: Fri, 24 Apr 2020 08:34:31 GMT  
		Size: 2.7 MB (2724562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; 386

```console
$ docker pull hylang@sha256:574a6759e033574472a6d4fa03aed8149a2f1c3cc2754227684266f8c351a41b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34656475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d6d93ed0077df4d7039552d8aa964cd8325398c9639068c95362b25bb25be5`
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
# Thu, 23 Apr 2020 21:58:55 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Apr 2020 21:58:55 GMT
ENV PYTHON_VERSION=3.7.7
# Thu, 23 Apr 2020 22:09:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 22:09:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 23 Apr 2020 22:09:27 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 23 Apr 2020 22:09:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 23 Apr 2020 22:09:27 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 23 Apr 2020 22:09:34 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Apr 2020 22:09:34 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 04:00:20 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 04:00:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 04:00:25 GMT
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
	-	`sha256:75e7dbe901b41baa097a36df15cc550b1000fcaf4a534f505ee5c40fb75cc430`  
		Last Modified: Thu, 23 Apr 2020 22:45:26 GMT  
		Size: 27.0 MB (26952313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff715e3c4f09c1d3d71e707aa5f1acae1ca46c9c7605ec4e787d0d8a69ec046c`  
		Last Modified: Thu, 23 Apr 2020 22:45:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce263b996b8fcb6da94c12b67e7e5167bd3408aa2083a490499b2346539ac8f8`  
		Last Modified: Thu, 23 Apr 2020 22:45:20 GMT  
		Size: 1.9 MB (1890980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0187ada1a902c3e44d1b878de29393484209905f6ff5980fb555658e6e5462`  
		Last Modified: Fri, 24 Apr 2020 04:02:54 GMT  
		Size: 2.7 MB (2724227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; ppc64le

```console
$ docker pull hylang@sha256:2725578f98b3c75d10e104427dda57badbdd0a5951f4a93779944298d81f76bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37258165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f799e3c7b9245876166c86a875778c5d141bddeb84c800e653f1717efbbae50`
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
# Fri, 24 Apr 2020 10:19:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Apr 2020 10:19:28 GMT
ENV PYTHON_VERSION=3.7.7
# Fri, 24 Apr 2020 10:31:25 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 10:31:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 10:31:36 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 10:31:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 10:31:42 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 10:31:56 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 10:31:58 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 15:20:53 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 15:21:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 15:21:15 GMT
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
	-	`sha256:b356fe1206b623d24d38867931106fb1ca471d57620605f235384a42653a9cf4`  
		Last Modified: Fri, 24 Apr 2020 11:10:23 GMT  
		Size: 29.5 MB (29527874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0c340ac1b2ddd062053c0049673075f92da853bb2b39d8296aceabe91197b5`  
		Last Modified: Fri, 24 Apr 2020 11:10:15 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45936ee8dc9ae2f030b1934b2911c3641c10a3d7baf5d6bb5f002f1e4e3b229b`  
		Last Modified: Fri, 24 Apr 2020 11:10:16 GMT  
		Size: 1.9 MB (1891503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e406cf880631595b1e565ceb6a08563c3891493408d42dbbae034866702ae8`  
		Last Modified: Fri, 24 Apr 2020 15:25:53 GMT  
		Size: 2.7 MB (2724907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine3.10` - linux; s390x

```console
$ docker pull hylang@sha256:f515e377b5af95c9960f2045a4ec0974565594bea32eee3ad162bce0c2192238
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36090652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8526f94d5a05cf7181a6d72415417f56ab71f969f425b70a4d9e1793e8aad3`
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
# Fri, 24 Apr 2020 00:19:24 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Apr 2020 00:19:24 GMT
ENV PYTHON_VERSION=3.7.7
# Fri, 24 Apr 2020 00:25:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 24 Apr 2020 00:25:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 24 Apr 2020 00:25:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Fri, 24 Apr 2020 00:25:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Fri, 24 Apr 2020 00:25:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Fri, 24 Apr 2020 00:25:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 24 Apr 2020 00:25:30 GMT
CMD ["python3"]
# Fri, 24 Apr 2020 10:10:20 GMT
ENV HY_VERSION=0.18.0
# Fri, 24 Apr 2020 10:10:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 24 Apr 2020 10:10:24 GMT
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
	-	`sha256:40c80a10484b3b77d75fe55ab8e136068d0e3530419273685f5b5ce6a85fd861`  
		Last Modified: Fri, 24 Apr 2020 06:44:24 GMT  
		Size: 28.6 MB (28598536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1390e04adec7db82f8a26596d24257f935b9ff32e01e727b2caeb6144ba802be`  
		Last Modified: Fri, 24 Apr 2020 06:44:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353837efd0ed6a9c113c7a9cced968e036699807f7492fe3a5a0086e60c1b8bc`  
		Last Modified: Fri, 24 Apr 2020 06:44:19 GMT  
		Size: 1.9 MB (1891287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ab3caa36e6955a8d7a93067653067b4f63a4be9f1725ee849978daf56c0bd6`  
		Last Modified: Fri, 24 Apr 2020 10:12:47 GMT  
		Size: 2.7 MB (2724412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
