## `hylang:0-python3.7-stretch`

```console
$ docker pull hylang@sha256:351cb201a440e83ea0a3a9bde57a17ea5072f56dd1bb61336a9f45ba23de27b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-python3.7-stretch` - linux; amd64

```console
$ docker pull hylang@sha256:cda00f9ad5c88286deded374f422eb9d4367a8bbe705206f0ab456d8bd83ef0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88224af32798f638a645a13047d06e39aa5cd2566f1acb9e0204a4ba03112176`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 17:51:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 17:51:33 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 17:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:51:46 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 12 Jan 2021 17:51:46 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 12 Jan 2021 18:02:54 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Jan 2021 18:02:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Jan 2021 18:02:55 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 18:02:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 18:02:55 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 18:03:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 18:03:09 GMT
CMD ["python3"]
# Tue, 12 Jan 2021 23:05:34 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 23:05:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 23:05:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e650750de57ddba73f7898085b2cdf2eabdaad6b2fc9a1cff60b6f764aeb84aa`  
		Last Modified: Tue, 12 Jan 2021 18:46:18 GMT  
		Size: 2.5 MB (2485746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdb855f7fed1ac9d545d2ceac650e072f935868699feb0edb982d9f5430fa56`  
		Last Modified: Tue, 12 Jan 2021 18:46:20 GMT  
		Size: 10.0 MB (10005097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48945d8ebc04e34f680034dcbd904430d1ef448563fc7917c87f451351db49bb`  
		Last Modified: Tue, 12 Jan 2021 18:46:17 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f405b5ed74dfb14a2dec0ef3ad05591f7cadad41b295c10d5030bcc5b140c9`  
		Last Modified: Tue, 12 Jan 2021 18:46:17 GMT  
		Size: 2.4 MB (2421843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0d7391f094d46b5fb4365f88e8cfa23b16aaf45802f6d91aa27b95e389451f`  
		Last Modified: Tue, 12 Jan 2021 23:09:01 GMT  
		Size: 2.8 MB (2824115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm variant v5

```console
$ docker pull hylang@sha256:b14458faf027215417817c714187441cc39f4f18e3887a409a9e4f1a877c322e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38016979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808d401b17f0ad14d06b78d69e7aa0b57a7ea8b2ba966e0978bc4586a7793eeb`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:55:36 GMT
ADD file:a1aaab9dbc905b25a99c43eb7b0b67fd535a69525aa1041074f121a1a3d4e0fd in / 
# Tue, 12 Jan 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 07:25:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 07:26:00 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 07:26:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 07:26:20 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 12 Jan 2021 07:26:21 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 12 Jan 2021 07:36:57 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Jan 2021 07:37:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Jan 2021 07:37:03 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 07:37:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 07:37:05 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 07:37:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 07:37:40 GMT
CMD ["python3"]
# Tue, 12 Jan 2021 13:32:15 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 13:32:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 13:32:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:aebd341c255b2e9649416ee98a58dcb2bfe03c3254dad00ab693687f1a9c8af5`  
		Last Modified: Tue, 12 Jan 2021 01:05:10 GMT  
		Size: 21.2 MB (21204237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ab6f8ce38a94c2dd3c766bd795a5a9f04434900030b1db9b1a289106f7d5a5`  
		Last Modified: Tue, 12 Jan 2021 08:14:46 GMT  
		Size: 2.2 MB (2216381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a17a7644b6b4b1e78f93c038e9a3f99e4eb1650049dec54fa52e02584825e`  
		Last Modified: Tue, 12 Jan 2021 08:14:50 GMT  
		Size: 9.3 MB (9349550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477fab67b3899c1e43e841ed6bed0b7febd997c3d8cbda767bd687e0bda39c73`  
		Last Modified: Tue, 12 Jan 2021 08:14:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb291e09fde5e7c1c3602ae3b623441b1feb76e3fedb6abbdfc4f25843e754ab`  
		Last Modified: Tue, 12 Jan 2021 08:14:47 GMT  
		Size: 2.4 MB (2421975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a86adedc1c7d73fb34232633d9b8a46914ad923c355c0007517fbacfb8059e`  
		Last Modified: Tue, 12 Jan 2021 13:34:40 GMT  
		Size: 2.8 MB (2824594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm variant v7

```console
$ docker pull hylang@sha256:246e48e0af2db5be15c87f69dc6744e92241d2476b68f4ff851bef6e5f5331d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (35995196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5041fce6cf0affe30d39ec0a7cb87645575b6111ce875a779d49175ad162cd3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 13:32:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 13:32:02 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 13:32:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:32:20 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 12 Jan 2021 13:32:21 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 12 Jan 2021 13:45:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Jan 2021 13:45:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Jan 2021 13:45:32 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 13:45:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 13:45:34 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 13:46:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 13:46:05 GMT
CMD ["python3"]
# Tue, 12 Jan 2021 22:13:37 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 22:13:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 22:13:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f1264eb6beafdd4b22533e7ac7a181f8b6f03156059f170cac02aab4ad7cc`  
		Last Modified: Tue, 12 Jan 2021 14:30:49 GMT  
		Size: 2.1 MB (2137670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25202b0264ad846d06ace91e2dd1d14d126dc6ab3de0ac2339099e6f50db527`  
		Last Modified: Tue, 12 Jan 2021 14:30:49 GMT  
		Size: 9.3 MB (9295083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecee618637d1eff3ae13ef0c5ebf8f46ea16116bd6e7f0cbaeb5f9a4e7402d`  
		Last Modified: Tue, 12 Jan 2021 14:30:49 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df659ef9e5451b2cfae15fa1549aa42e30bba7974e73e9cddf98f737ced0d1`  
		Last Modified: Tue, 12 Jan 2021 14:30:49 GMT  
		Size: 2.4 MB (2421696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e573c5d3241479d8b2eb1cbb17901b1c61c37d3fac36108c1deeced7df241be3`  
		Last Modified: Tue, 12 Jan 2021 22:17:03 GMT  
		Size: 2.8 MB (2824515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:ac8e352eca888dde255e6d169358f14e512978fd53a1ca24502ccaa21a6d6579
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37557094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ef483e3688be9f5b732f43bfd7d2132d1a12bb5de7ad22b9ecf2c2f6490cc2`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 13:28:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 13:28:20 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 13:28:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:28:53 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 11 Dec 2020 13:28:55 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 11 Dec 2020 13:41:15 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 11 Dec 2020 13:41:21 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Dec 2020 23:02:23 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 23:02:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 23:02:29 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 23:03:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 23:03:11 GMT
CMD ["python3"]
# Tue, 15 Dec 2020 23:15:04 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:15:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:15:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c841ad12709b1a4912be95d9fdbf1e4fa98472ca8acc54dc57ad51f0effb066`  
		Last Modified: Fri, 11 Dec 2020 14:32:30 GMT  
		Size: 2.2 MB (2199177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98b893e0e5000d683c54d17527dfd3f8606fd31277beb97795e6c08046c230a`  
		Last Modified: Fri, 11 Dec 2020 14:32:33 GMT  
		Size: 9.7 MB (9723427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17239b5f207899d566542531f143e0d8ec333245629b2a6b1240adff581bf4c`  
		Last Modified: Fri, 11 Dec 2020 14:32:30 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67d256a6cd300c9bd4093f206f45b6ada419ae16f16753d3cee7023e03714c9`  
		Last Modified: Tue, 15 Dec 2020 23:11:37 GMT  
		Size: 2.4 MB (2421733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b70ecf8f75bc7888641b141d365280425a84f85b41eb533a02a1081f26767`  
		Last Modified: Tue, 15 Dec 2020 23:20:50 GMT  
		Size: 2.8 MB (2824635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; 386

```console
$ docker pull hylang@sha256:8aff1cab73c4bb5c9e99dd0ef6812e20f75d7915ef6bd946c9040949302abf1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40981938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a2d950e7858aad57330fb053cdfc3a5b78d62ff177dfe6b344437a9e5e67d8`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:15 GMT
ADD file:063139004c73cb6604fea25bb3b6e525aec0ae9e058a80019983c4d829bc5284 in / 
# Tue, 12 Jan 2021 00:42:15 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 14:35:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 14:35:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 14:36:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 14:36:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 12 Jan 2021 14:36:06 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 12 Jan 2021 14:48:26 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Jan 2021 14:48:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Jan 2021 14:48:28 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 14:48:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 14:48:29 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 14:48:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 14:48:49 GMT
CMD ["python3"]
# Tue, 12 Jan 2021 21:48:20 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 21:48:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 21:48:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f2e04963ccccb40a42f69475cc128575f57db677f5a2fa0ce980baa2a1ade883`  
		Last Modified: Tue, 12 Jan 2021 00:50:59 GMT  
		Size: 23.2 MB (23156510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af144c801b5a08b17a711ea03d330a54aad3dab989946ff70a4a32b0a016e1a`  
		Last Modified: Tue, 12 Jan 2021 15:44:10 GMT  
		Size: 2.5 MB (2490232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54313e565213d0f3ac64aabd061bd7f65fcb61f804b017e35b00e2870ec517c8`  
		Last Modified: Tue, 12 Jan 2021 15:44:13 GMT  
		Size: 10.1 MB (10089048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55caee30d8a04d71acc14322391852330c6d26e4f9a01801c0be2b7d16c530c4`  
		Last Modified: Tue, 12 Jan 2021 15:44:07 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0220560b1ea592c580c80d8b7ba1137c8158ea8218d4ff91e79e5a1f5b017`  
		Last Modified: Tue, 12 Jan 2021 15:44:11 GMT  
		Size: 2.4 MB (2421616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea00b8296b7d93d0e6b440dad71d07e22f77aec0b83c4521e3205df1b7ff1f0`  
		Last Modified: Tue, 12 Jan 2021 21:52:22 GMT  
		Size: 2.8 MB (2824292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
