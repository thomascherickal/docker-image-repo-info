## `hylang:python3.7`

```console
$ docker pull hylang@sha256:f3adc0c9b58437a19f63e71a4872966ef6a441a540ade5a8a1b63e928dcc2e16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `hylang:python3.7` - linux; amd64

```console
$ docker pull hylang@sha256:6af085d446b1bc33920c7dd60692040a75db173fccf25eb9b0979ec0980182da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48229604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d16cf6933c780249c9a09ee34a154faee1c672a6afbed2c0f9bfe048fdc0113`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:54:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 01:54:38 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 02:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 03:14:19 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 03:14:19 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 03:22:59 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 03:23:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 03:23:00 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 03:23:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 03:23:00 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 03:23:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 03:23:12 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 00:20:42 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 00:20:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 00:20:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9202170ba44ed748bb05d5e0de4a8c1ed1de21c247bc5b55c8323424d28f411f`  
		Last Modified: Tue, 17 Aug 2021 03:59:26 GMT  
		Size: 1.1 MB (1075866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598c4c4defc8cbcd328f297ab874777e24b149e9de5572031a4dee8b849e7024`  
		Last Modified: Tue, 17 Aug 2021 04:00:14 GMT  
		Size: 10.1 MB (10100811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbb562cb68bb404321b95972ffa01d3ee543d346da283f7e8c9db56a42e2ff7`  
		Last Modified: Tue, 17 Aug 2021 04:00:12 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126703eb79854780394e049e9b8611b61c1c77c4456753cd21159845efdd8965`  
		Last Modified: Tue, 17 Aug 2021 04:00:12 GMT  
		Size: 2.6 MB (2640131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7469170126a6f554c9ba7326bf4f48250152cba172a6af719b14048f7b27d3`  
		Last Modified: Thu, 19 Aug 2021 00:23:46 GMT  
		Size: 3.1 MB (3051250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm variant v5

```console
$ docker pull hylang@sha256:5ca627ae191a27a688ccf640e003960eecf7e7f3ca44f5054356de3818894a0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45351103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573f25164833a8c732399228a6bfd4210348a5d529da3fc62673e49711f46548`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 03:45:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 03:45:04 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 05:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:07:30 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 06:07:30 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 06:25:38 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 06:25:40 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 06:25:40 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 06:25:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 06:25:41 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 06:26:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 06:26:13 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:50:11 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:50:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:50:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b24195f6fd5e811c9ab9c9b31acfb33744ca6febc1dd29cb92de07ef87c92e`  
		Last Modified: Tue, 17 Aug 2021 07:31:40 GMT  
		Size: 1.1 MB (1059058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa44b6be2c2c0dc0a6fce449134ade094b107749995229f6ede2a29ccefe153`  
		Last Modified: Tue, 17 Aug 2021 07:32:56 GMT  
		Size: 9.7 MB (9696396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f343ae1266402145d76a82b4d68601cee9baf270f82a1f26aaa2322c8a30b5`  
		Last Modified: Tue, 17 Aug 2021 07:32:49 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19e7acd9f95bdfdb4bd171e2357c863cf10acb85f97a06aba4d58c5c62607f1`  
		Last Modified: Tue, 17 Aug 2021 07:32:52 GMT  
		Size: 2.6 MB (2639742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6b354b20d3f4fe1519b6043b8c22f9ff156ae706e0c8d555ea9b151bf04ea`  
		Last Modified: Wed, 18 Aug 2021 23:55:00 GMT  
		Size: 3.1 MB (3051505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm variant v7

```console
$ docker pull hylang@sha256:7cdfe6a7adf097ebd2ff7b3238a41375efc0ca1b611ab33bb6d1d6ccb6091225
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42592602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c09eac63e23b721d3b854effd495e96f76640bfcea217724db9acf2d4391d2ff`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:16 GMT
ADD file:56b22dfd365932a88a68ec72e6b9c1af8c5747606e0387a2c189dfb49998d029 in / 
# Tue, 17 Aug 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 03:27:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 03:27:20 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 05:38:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:42:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 06:42:25 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 07:05:17 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 07:05:18 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 07:05:19 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 07:05:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 07:05:20 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 07:05:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 07:05:47 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 04:30:47 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 04:30:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 04:30:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8cb10f7ccaa8117b68a975362a370a0cbe9272ee95488ac4870c6f8a80c2e3`  
		Last Modified: Tue, 17 Aug 2021 08:30:13 GMT  
		Size: 1.0 MB (1041287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5be3c0909b27ac0ba061f2db4da9fc365926e2f330f04b5d5b2c1046476d4d4`  
		Last Modified: Tue, 17 Aug 2021 08:31:37 GMT  
		Size: 9.3 MB (9294071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4e03c80967692bdb83754f65104975b40c18fe513f4e61df7ba412758ca11`  
		Last Modified: Tue, 17 Aug 2021 08:31:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344974aab55b939c6eca3d047614689f993a644079a0293f495a67e58f02328e`  
		Last Modified: Tue, 17 Aug 2021 08:31:33 GMT  
		Size: 2.6 MB (2639936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998a9d62a7af7bdc2b3e45fdf3981bd55a82fee462a30d54f5d4586b65db7cb7`  
		Last Modified: Thu, 19 Aug 2021 04:39:43 GMT  
		Size: 3.1 MB (3051501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d7a161a4a4915fc7c1acc59aacb0b504243087b2b44d38a49ef05336bc1068f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46943532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0e97bb0e629370f970b5be46b4d61ae743f07b9aaf186045deca40437ff5a5`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:18:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 02:18:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 02:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 03:20:16 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 03:20:16 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 03:28:00 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 03:28:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 03:28:01 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 03:28:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 03:28:01 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 03:28:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 03:28:13 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:41:21 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:41:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:41:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a3ccea200b2b1adaa4aadbba08ac118a2f3b728c010185c47e6ca110ad8639`  
		Last Modified: Tue, 17 Aug 2021 04:02:25 GMT  
		Size: 1.1 MB (1064360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e151313c67cddac4dfa3ede3d3749e1b6eea82f9782698523c0a933782ef4`  
		Last Modified: Tue, 17 Aug 2021 04:03:25 GMT  
		Size: 10.1 MB (10139181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f14a418f5f939b87e7f9728f5d7e5acb2b277e7b584708cf600df5d2fe713`  
		Last Modified: Tue, 17 Aug 2021 04:03:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7a2bec527e17dc78a6b7e16243215727d5f0cfb332246d22364a859e4a7bd5`  
		Last Modified: Tue, 17 Aug 2021 04:03:24 GMT  
		Size: 2.6 MB (2639750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51857de6b27efa38d3e6e2c62574ae0a2430533bff6530e490ec6c2cd312daba`  
		Last Modified: Wed, 18 Aug 2021 23:46:37 GMT  
		Size: 3.1 MB (3051209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; 386

```console
$ docker pull hylang@sha256:afeb46a22e1e0e1bc73084834390ca0c9262d7b6e5eb1b4df1be39a1b88cb2a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49363423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df60be60ea9c9a738e11811d1200eb9805b1037a13b2c7f39723172bb7e7266`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:52:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 02:52:05 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 05:27:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 05:27:11 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 05:42:30 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 05:42:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 05:42:32 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 05:42:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 05:42:33 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 05:42:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 05:42:54 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:40:31 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:40:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:40:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb573c693c387bcd21769cc02c784c894b68746d059617b2f9fd209a7b88d2ec`  
		Last Modified: Tue, 17 Aug 2021 07:06:28 GMT  
		Size: 1.1 MB (1088312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b627d28fb80e96d3782e0cb390472d0b0bfbd3e3057b52657af2dba53ef98c7`  
		Last Modified: Tue, 17 Aug 2021 07:07:54 GMT  
		Size: 10.2 MB (10208121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee595b42c18be08ffc0b800e5c4bce3a21f43f71b6380acbc195ef6ea1d677b`  
		Last Modified: Tue, 17 Aug 2021 07:07:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55ae3458be9b9849ef6505795328d298bd8231d279521a638f3a5f8651fae0`  
		Last Modified: Tue, 17 Aug 2021 07:07:52 GMT  
		Size: 2.6 MB (2639866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b35f0e619b9431a4ec01e24c09133ed27ce32135963317ead9008d414b2fd8e`  
		Last Modified: Wed, 18 Aug 2021 23:45:57 GMT  
		Size: 3.1 MB (3051235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; mips64le

```console
$ docker pull hylang@sha256:eb147dcf0bb85fa20fca667dc707a5a3a04d46ab617f162db57a87a70447cf71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46387157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffd622386fa638cea4663799574a6b86f3448a72495533aedf59d2416ed8e55`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:35 GMT
ADD file:4dff23dfe5a1c3cf77be5121c29de84ee66c4d10c85faa65f6122da1bfa13500 in / 
# Tue, 17 Aug 2021 01:11:36 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:52:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 02:52:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:27:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:35:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 09:35:30 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 10:17:55 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 10:17:57 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 10:17:58 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 10:17:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 10:17:58 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 10:18:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 10:18:40 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 00:08:23 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 00:08:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 00:08:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8375ff99ce3f614d73dc69b03575c7ebf072f4e05da52b0319fc3782d5ebb578`  
		Last Modified: Tue, 17 Aug 2021 01:20:19 GMT  
		Size: 29.6 MB (29619986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02574db3e29a65b0e54826d8d3dda060466177723b3a35e65d214465874d8370`  
		Last Modified: Tue, 17 Aug 2021 12:41:32 GMT  
		Size: 1.0 MB (1049214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc57c5ae7282ce9075647ddd7c55f8b8d351b1934617193856f62517408ac95c`  
		Last Modified: Tue, 17 Aug 2021 12:42:38 GMT  
		Size: 10.0 MB (10026824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4bc87cce54a6e2592b69972646f76f3c37ebe5aca977d563a85b2703442af`  
		Last Modified: Tue, 17 Aug 2021 12:42:32 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb67ac173427c6e61d55e7268276e13fc78bfd0c0f4b25e0aa12d0653ca2452`  
		Last Modified: Tue, 17 Aug 2021 12:42:34 GMT  
		Size: 2.6 MB (2639700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d0c055cf2603ce107b4b836d5ac1e71e1127dd0df4903c81c2b3469b6a99f`  
		Last Modified: Thu, 19 Aug 2021 00:10:34 GMT  
		Size: 3.1 MB (3051201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; ppc64le

```console
$ docker pull hylang@sha256:c8868111b31362db6af8fda203bbf4ba729ec2f5d0976ff6fd50cf93b289cfc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52515203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adb9e56f701159f1f6c8f1c19098cb5553f4214c7f5b1fffca67da8bbec79e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:09 GMT
ADD file:b7348f0e1a41ce54354496488a0ee8bb949743444973dc6ab51ea80926f596f2 in / 
# Tue, 17 Aug 2021 01:33:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:16:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 02:16:06 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:39:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 05:40:34 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 05:40:38 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 06:04:45 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 06:05:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 06:05:04 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 06:05:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 06:05:13 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 06:06:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 06:06:08 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 02:33:53 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 02:34:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 02:35:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6eed55e29b2bbfa5327718f00ab9826c5db2a0234566c0a0375f60a482f7de`  
		Last Modified: Tue, 17 Aug 2021 07:33:00 GMT  
		Size: 1.1 MB (1094458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52188898c09f2d8d834e009e02942d1031cab84d4f2332b4011166d1e357d0`  
		Last Modified: Tue, 17 Aug 2021 07:33:54 GMT  
		Size: 10.5 MB (10462447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe2ac2f942aef00985edf649d5d662309f16095b3ec6f35c9fa7c8acbc29d7`  
		Last Modified: Tue, 17 Aug 2021 07:33:52 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44d7f81feaca3a8e685ab5abb6833151093a285b19580b7b35cb2863161353`  
		Last Modified: Tue, 17 Aug 2021 07:33:53 GMT  
		Size: 2.6 MB (2641838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685099255fb8f975c66ad9caa2d36ff284d9bbc0384fba4395c16652b234ab38`  
		Last Modified: Thu, 19 Aug 2021 02:42:44 GMT  
		Size: 3.1 MB (3052216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; s390x

```console
$ docker pull hylang@sha256:7ed4c647d65a9ba765f02d8f9e2d6aeaee634b15e2669f115bd8f56f07be04a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46381053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e8f0f5dd4ca1a12cd07ff6c1d8cfa8cd8ca54ba89f8a0b06150c9b52826abea`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:21:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 02:21:40 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 03:07:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 03:29:24 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 17 Aug 2021 03:29:24 GMT
ENV PYTHON_VERSION=3.7.11
# Tue, 17 Aug 2021 03:35:51 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 03:35:54 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 03:35:54 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 03:35:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 03:35:55 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 03:36:10 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:43:20 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:43:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:43:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2981d961833d1984a683ac92f24fcd335ea517f95b610f33fc033e4319711f4`  
		Last Modified: Tue, 17 Aug 2021 04:11:32 GMT  
		Size: 1.1 MB (1075399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdbd14864081c6e39fbf8b61217ea68931c8f5a068ec42d073f877f60f4f4f4`  
		Last Modified: Tue, 17 Aug 2021 04:12:13 GMT  
		Size: 10.0 MB (9967251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3f64e2483062d78e338681fa611a6a3917895a7d345edf0052718e2342315d`  
		Last Modified: Tue, 17 Aug 2021 04:12:11 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c48f615faa9b835cc2da1ec338a5934f8c9a02a128ee305008b1809d1e9273a`  
		Last Modified: Tue, 17 Aug 2021 04:12:11 GMT  
		Size: 2.6 MB (2639949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a346d1079dfbfc0992ee5bcef8557992c74fe45b302d50ab37f3a720860bdb`  
		Last Modified: Wed, 18 Aug 2021 23:47:12 GMT  
		Size: 3.1 MB (3051194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
