## `hylang:python3.7-stretch`

```console
$ docker pull hylang@sha256:fd83363cb3084b135e212d1ef0dce1871d15f10533cafe979150f193aadc8b7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:python3.7-stretch` - linux; amd64

```console
$ docker pull hylang@sha256:cb68b5416dc0053ad65fcba11ef0efecebcf3109a7875b634d2b5d829dd24d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55760538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6a34728c39167afe498ceb7a7d56446941449ad160dd742958bca20fcc7a54`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:28:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 04:28:48 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 16:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 16:07:56 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 31 Mar 2020 16:07:56 GMT
ENV PYTHON_VERSION=3.7.7
# Tue, 31 Mar 2020 16:17:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 31 Mar 2020 16:17:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Mar 2020 16:17:06 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 16:17:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 16:17:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 16:17:20 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 16:17:20 GMT
CMD ["python3"]
# Wed, 01 Apr 2020 02:12:28 GMT
ENV HY_VERSION=0.18.0
# Wed, 01 Apr 2020 02:12:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Apr 2020 02:12:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961d7fa433a7838b5e3c41307cce3664068a1c7390419628f061d2c6bda0009c`  
		Last Modified: Tue, 31 Mar 2020 17:51:01 GMT  
		Size: 2.5 MB (2531185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73ff10f7cde809ff2b1dd6b80340c17fc4ee32a57355da274c00350ca13a87a`  
		Last Modified: Tue, 31 Mar 2020 17:51:09 GMT  
		Size: 25.8 MB (25816724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c5fff9b9cb92372e8f1366050f5464a0cd85076ec0e59f617617575d5fed4`  
		Last Modified: Tue, 31 Mar 2020 17:51:00 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ef6adeb7127ecefb440d8820df06c4367b3109f461f017218b1354518f8445`  
		Last Modified: Tue, 31 Mar 2020 17:51:01 GMT  
		Size: 2.2 MB (2174519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d494d16313ada7b722455dc5cf776e4ca469f101583f95b5c3fd50d6417e3f06`  
		Last Modified: Wed, 01 Apr 2020 02:14:31 GMT  
		Size: 2.7 MB (2724496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; arm variant v5

```console
$ docker pull hylang@sha256:6dfcf9ca28080b26eb745590fb9a87df0a33e0a95bcc16619c5d113f84683680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51122252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acef46ccba2bc63a1a7d72031223dadc37df8de1748278c69e22582b977eaa6`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 05:39:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 05:39:56 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 05:40:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 05:40:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 16 Apr 2020 05:40:14 GMT
ENV PYTHON_VERSION=3.7.7
# Thu, 16 Apr 2020 05:50:31 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 16 Apr 2020 05:50:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 16 Apr 2020 05:50:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 16 Apr 2020 05:50:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 16 Apr 2020 05:50:42 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 16 Apr 2020 05:51:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 16 Apr 2020 05:51:14 GMT
CMD ["python3"]
# Thu, 16 Apr 2020 13:38:22 GMT
ENV HY_VERSION=0.18.0
# Thu, 16 Apr 2020 13:38:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Apr 2020 13:38:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7416050986fddaf92e310a0b70efa344f029c41e84db3efa4e70d09f6a31fd`  
		Last Modified: Thu, 16 Apr 2020 06:57:12 GMT  
		Size: 2.3 MB (2256554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875307e0676165055d3c9f9aaea209e6f470c2277b39daad5d39e48463d41707`  
		Last Modified: Thu, 16 Apr 2020 06:57:20 GMT  
		Size: 22.8 MB (22774786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bca7880754b59dc36938d27501984ac9305009155f2ea3d2f25357fb146871c`  
		Last Modified: Thu, 16 Apr 2020 06:57:12 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6845dc36c46add6f191443c25670021a4aaac8e834bd3cbb9d529b9bb9ae53b2`  
		Last Modified: Thu, 16 Apr 2020 06:57:13 GMT  
		Size: 2.2 MB (2174850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab3d63bfdf02ad7ac007404a8cc562725ff77df884215dae0997aef67a61820`  
		Last Modified: Thu, 16 Apr 2020 13:41:17 GMT  
		Size: 2.7 MB (2725025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; arm variant v7

```console
$ docker pull hylang@sha256:115d6e2c364cbb548e5193697ce30dbb1758848b94251ce6bd220bc5a3eff888
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49688305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70fd83489c93257ff9d34a23f2a8e1f42b0283627290a0cb3ad8f68f85395da`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 01:52:50 GMT
ADD file:1e233b688c850d7a8a47f185e6f7bb82ad66d729fb1714ecced354cff7be80cd in / 
# Tue, 31 Mar 2020 01:52:52 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 14:15:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 14:15:24 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 14:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 14:15:43 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 31 Mar 2020 14:15:44 GMT
ENV PYTHON_VERSION=3.7.7
# Tue, 31 Mar 2020 14:28:54 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 31 Mar 2020 14:28:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Mar 2020 14:28:59 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 14:29:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 14:29:01 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 14:29:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 14:29:30 GMT
CMD ["python3"]
# Wed, 01 Apr 2020 00:51:57 GMT
ENV HY_VERSION=0.18.0
# Wed, 01 Apr 2020 00:52:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Apr 2020 00:52:09 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4d2af5687ff47f04bedeb1936ed8fe931d68c5684a6959606402065ca5dcb2c5`  
		Last Modified: Tue, 31 Mar 2020 02:00:11 GMT  
		Size: 19.3 MB (19298305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5aff28d233c138c974a45896d6896df1b3e06b21b5b4b75d680d420b47c17d`  
		Last Modified: Tue, 31 Mar 2020 16:31:06 GMT  
		Size: 2.2 MB (2177869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08da5d6cb469f765971f0b74b9b7af1b7678ceac53301e86aebc2aac648abd7`  
		Last Modified: Tue, 31 Mar 2020 16:31:14 GMT  
		Size: 23.3 MB (23312144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a07ab950fcbbfac4f36d1e8f873fff5c93f67381dbcb61595354343a5cc6928`  
		Last Modified: Tue, 31 Mar 2020 16:31:06 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc6c85779e811c1d9d5ec726fee131a95d5d9c94024034bde3000c6db4f597`  
		Last Modified: Tue, 31 Mar 2020 16:31:07 GMT  
		Size: 2.2 MB (2174818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15917d1f9663deb9240e71fecf29f18fff165827c300fc44640404cc34cfbb7b`  
		Last Modified: Wed, 01 Apr 2020 00:55:22 GMT  
		Size: 2.7 MB (2724928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:10f229afde7f6abe4c3e403fdcfc4dfd4cd7e19f064af053bc4a9b7803833474
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52157255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b42f5a26f163bfeb1b268a61e5d1f70b86bf3d70b189fb6d291e037917a184`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 02:08:41 GMT
ADD file:002dfad10aab7242b4c5779d19cdca9d7fc4c9fc6fdfa8ed7f282c459fab5da4 in / 
# Tue, 31 Mar 2020 02:08:44 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 06:19:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 06:19:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 16:41:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 16:41:34 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 31 Mar 2020 16:41:35 GMT
ENV PYTHON_VERSION=3.7.7
# Tue, 31 Mar 2020 16:54:13 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 31 Mar 2020 16:54:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Mar 2020 16:54:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 16:54:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 16:54:18 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 16:54:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 16:54:46 GMT
CMD ["python3"]
# Wed, 01 Apr 2020 00:53:44 GMT
ENV HY_VERSION=0.18.0
# Wed, 01 Apr 2020 00:53:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Apr 2020 00:53:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:43bf72d10816e9fab289a20d17eb586989e2caecbf80328a1c24f031683c350a`  
		Last Modified: Tue, 31 Mar 2020 02:14:33 GMT  
		Size: 20.4 MB (20369961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940a4d21b23b8e4db81732c9db30bb7ddd4e5e23b49de866f4e267f2160258c2`  
		Last Modified: Tue, 31 Mar 2020 18:54:15 GMT  
		Size: 2.2 MB (2238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af22db21c432c7197ba410e3cb72fa27161e1bd7ea7d10b1b8693c81f9ec38d`  
		Last Modified: Tue, 31 Mar 2020 18:54:24 GMT  
		Size: 24.6 MB (24648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450a68f617dc5ae67906d85a34bf88b940d256d2ab41c8e6729de921930176f6`  
		Last Modified: Tue, 31 Mar 2020 18:54:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d1e4b4ae3b14269a30aecb08bef003b11a241220202f4ed7bd6f4fb08e37d7`  
		Last Modified: Tue, 31 Mar 2020 18:54:16 GMT  
		Size: 2.2 MB (2174605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b1366ad7402258d87de7a9d7f405320e35b24a3275e8a673561f1fbe9c858b`  
		Last Modified: Wed, 01 Apr 2020 00:57:32 GMT  
		Size: 2.7 MB (2725012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; 386

```console
$ docker pull hylang@sha256:20da5cd8404819b501a878e003c3056e565a75333342e796eb181375a68f110e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54758876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2ac63f5e2f65aa629ddc120f4ecbbd83b9c61e38b55e479f3bf9354cc75bff`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 00:42:50 GMT
ADD file:3b9d63dd21a9a32c414c2ec2fda6cd46b6d0ea83cd89b56de0f238f27458082f in / 
# Tue, 31 Mar 2020 00:42:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:20:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 02:20:32 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 17:18:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 17:18:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 31 Mar 2020 17:18:57 GMT
ENV PYTHON_VERSION=3.7.7
# Tue, 31 Mar 2020 17:29:16 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 31 Mar 2020 17:29:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Mar 2020 17:29:17 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 17:29:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 17:29:17 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 17:29:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 17:29:33 GMT
CMD ["python3"]
# Tue, 31 Mar 2020 19:51:42 GMT
ENV HY_VERSION=0.18.0
# Tue, 31 Mar 2020 19:51:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 31 Mar 2020 19:51:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7101806a3a87632f9e8e3ed7e99547db8d61727cb461d50f91fa2099ee987d87`  
		Last Modified: Tue, 31 Mar 2020 00:48:47 GMT  
		Size: 23.1 MB (23141421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94b6918102c11ba89c8d209b6b5424cdd25dc905c81226b42adc6de4822255c`  
		Last Modified: Tue, 31 Mar 2020 19:38:59 GMT  
		Size: 2.5 MB (2532892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2b01e5bbab4ae546e1a07b7339fc34c79905bbea7b094d10ce9b82387609`  
		Last Modified: Tue, 31 Mar 2020 19:39:06 GMT  
		Size: 24.2 MB (24185211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e330180a2b908f379e1dfd9c862f97c1cb51a2aaa52c20f822d934654d4f23`  
		Last Modified: Tue, 31 Mar 2020 19:38:58 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbf7bac8b7b5f09f98cb57929cc9cfc11a70f164736d0aa338e853ed48a0bd2`  
		Last Modified: Tue, 31 Mar 2020 19:38:59 GMT  
		Size: 2.2 MB (2174485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7484e71983170240248ac93913542c7106e0a709f32f5d2deb8983522f3535`  
		Last Modified: Tue, 31 Mar 2020 19:54:53 GMT  
		Size: 2.7 MB (2724625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; ppc64le

```console
$ docker pull hylang@sha256:409abf12c754ff142f712b54bd819efcd50c2c1bc5cdad9da6e5dc50e5c6d510
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55767250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0a0144bd5863f52f71ae7553aa41195e95c3e449d3b5e356c698d909be9e15`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 01:36:47 GMT
ADD file:18fbbcdf5b1b1e93b849dccfac9d28a25ed63c4c13f3e6cb141579d7474401e7 in / 
# Tue, 31 Mar 2020 01:36:53 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:00:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 02:00:38 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 14:26:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 14:26:15 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 31 Mar 2020 14:26:22 GMT
ENV PYTHON_VERSION=3.7.7
# Tue, 31 Mar 2020 14:42:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 31 Mar 2020 14:42:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Mar 2020 14:42:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 14:42:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 14:42:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 14:43:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 14:43:13 GMT
CMD ["python3"]
# Wed, 01 Apr 2020 04:21:27 GMT
ENV HY_VERSION=0.18.0
# Wed, 01 Apr 2020 04:22:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Apr 2020 04:22:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:12443815c8d74f5cceb21d06ea95ceca887ebe0a6f2e2084bd2131a6ad9c6af0`  
		Last Modified: Tue, 31 Mar 2020 01:54:08 GMT  
		Size: 22.8 MB (22785257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e9accc1091ac0d04f2c775e2e25ca9286b550b895633d9878816b65c59cf75`  
		Last Modified: Tue, 31 Mar 2020 17:22:23 GMT  
		Size: 2.2 MB (2192848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be38e33a21355e4f5fbdbb92440b8aa5aae15247f296ed0c9bd00e9fe14f04`  
		Last Modified: Tue, 31 Mar 2020 17:22:29 GMT  
		Size: 25.9 MB (25887649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff6b4551f5118b60297887758087e49477405c0fc9dc92b2158ebd3dca8bfd7`  
		Last Modified: Tue, 31 Mar 2020 17:22:22 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965857f1441d7b67b10169d37e7a1ed5eb39b4de8e6edacfde8bf9100bdc1f3e`  
		Last Modified: Tue, 31 Mar 2020 17:22:23 GMT  
		Size: 2.2 MB (2175997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2977517b57149443a989d802dd288c06a1fcc2f7a65e2c242d0ffc039a9ab8a6`  
		Last Modified: Wed, 01 Apr 2020 04:27:49 GMT  
		Size: 2.7 MB (2725256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-stretch` - linux; s390x

```console
$ docker pull hylang@sha256:946bc49f99035ce40d00cd9d96d3e8df9e5c1813d093102878d0bdfaacbd76e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56495215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e663c23f0b9770a737613ed9a3257c5d6981b0188c5605604118ac339b2b0de3`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 16 Apr 2020 00:44:02 GMT
ADD file:316fb059b77553ea3f4064090106c72f87b737be109396d29a752a1b33295450 in / 
# Thu, 16 Apr 2020 00:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:37:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 07:37:23 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 07:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 07:37:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 16 Apr 2020 07:37:29 GMT
ENV PYTHON_VERSION=3.7.7
# Thu, 16 Apr 2020 07:43:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 16 Apr 2020 07:43:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 16 Apr 2020 07:43:10 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 16 Apr 2020 07:43:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 16 Apr 2020 07:43:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 16 Apr 2020 07:43:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 16 Apr 2020 07:43:21 GMT
CMD ["python3"]
# Thu, 16 Apr 2020 10:01:22 GMT
ENV HY_VERSION=0.18.0
# Thu, 16 Apr 2020 10:01:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Apr 2020 10:01:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4d56eb3b82632a7f0507bf24d9239e9df75f437207bf7b4afc7eb72888f0b62f`  
		Last Modified: Thu, 16 Apr 2020 00:48:31 GMT  
		Size: 22.4 MB (22365447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff816881ebb3a6743284db2d530b9176ff3b60bd19e039628103452502e9235e`  
		Last Modified: Thu, 16 Apr 2020 08:38:33 GMT  
		Size: 2.3 MB (2269062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c876f9430da87dc495b2b061b9b0de211e7fbe5102f6463c3a8a63da77bed88f`  
		Last Modified: Thu, 16 Apr 2020 08:38:38 GMT  
		Size: 27.0 MB (26961990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e197e80dea5e5f88154ee2e0efc5e6c4ce63a91bb708a9a016a33fe2c4c161b`  
		Last Modified: Thu, 16 Apr 2020 08:38:38 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec6d0ce1f705fcf5e30ad71a75ec8177c10541f37536f1c1e8d899fde684255`  
		Last Modified: Thu, 16 Apr 2020 08:38:39 GMT  
		Size: 2.2 MB (2173801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c574b7c5a2c813726f48c5d029555780cbabc95ea367ed37dc2712671762bb`  
		Last Modified: Thu, 16 Apr 2020 10:03:13 GMT  
		Size: 2.7 MB (2724674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
