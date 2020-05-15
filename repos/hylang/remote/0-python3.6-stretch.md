## `hylang:0-python3.6-stretch`

```console
$ docker pull hylang@sha256:d40b643f0a1c50a229bd2c3d30972c2915f90fbfa37204304ad1281701dd74ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `hylang:0-python3.6-stretch` - linux; amd64

```console
$ docker pull hylang@sha256:07e27ae4f6169b9b874c1f36bba455243f9380ce7f0ea7f061ecab6aaf85c58c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54398629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0a2187017c7652b982f30a0c1a9cada25bc2d57604a6c60d1ce6b8a0b1073f`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:40:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 11:40:07 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 11:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:40:16 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 15 May 2020 11:58:36 GMT
ENV PYTHON_VERSION=3.6.10
# Fri, 15 May 2020 12:06:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 12:06:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 12:06:07 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 12:06:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 12:06:08 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 12:06:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 12:06:31 GMT
CMD ["python3"]
# Fri, 15 May 2020 12:30:32 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 12:30:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 12:30:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc927b2aed6cc17bee0483331a6aaffe8cf0bfd648b6511b6b74e7a6f3b8f5b2`  
		Last Modified: Fri, 15 May 2020 12:27:28 GMT  
		Size: 2.5 MB (2531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331072d8ba4dcee639c1858f9ac0e790ad65eee54d4bf140dd6c0a75a6e3ab79`  
		Last Modified: Fri, 15 May 2020 12:27:56 GMT  
		Size: 24.4 MB (24380602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66878c6cf762a59570bd319037c9a51501b6bfc4ba00f3a14b227611cb80db86`  
		Last Modified: Fri, 15 May 2020 12:27:50 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1f298f868a72d48ae72cad2f6583c7f1685425b9d2a3bfd05aa7533284a14`  
		Last Modified: Fri, 15 May 2020 12:27:51 GMT  
		Size: 2.2 MB (2214017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ebf1ad117776865db29fa05c4e59c331c5298e44d351c25e94e98e2f5983f`  
		Last Modified: Fri, 15 May 2020 12:33:15 GMT  
		Size: 2.8 MB (2752709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; arm variant v5

```console
$ docker pull hylang@sha256:ac344f9a92f93bb758961a9e6467f08be46a65402b6071da21295c1407d5a7fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50130081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83c0d8365040abc5a99117a72a376075e1d93e728f8dd49db240914c50ed2eb`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 06:55:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 06:55:11 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 06:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 06:55:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 15 May 2020 07:33:50 GMT
ENV PYTHON_VERSION=3.6.10
# Fri, 15 May 2020 07:39:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 07:39:52 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 07:39:53 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 07:39:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 07:39:54 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 07:40:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 07:40:31 GMT
CMD ["python3"]
# Fri, 15 May 2020 13:08:16 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 13:08:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 13:08:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d06d1bed20064d2e8a1407748e9e2cc05c6f5f9834ea1afe82f83825f8de25e`  
		Last Modified: Fri, 15 May 2020 08:22:28 GMT  
		Size: 2.3 MB (2256572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48ab9b684a97000d23a16be19d2b8d6030fb8ce61702865b9280f33be88ea`  
		Last Modified: Fri, 15 May 2020 08:23:35 GMT  
		Size: 21.7 MB (21708854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296069cc469bdf4e28728fbbf3104b0dbb5b7baacd7734dd71b298dfeffe8e7`  
		Last Modified: Fri, 15 May 2020 08:23:27 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462e3036041b1dda97cc41b9f962525ce88e10baed4223d990f8be9ca31ad934`  
		Last Modified: Fri, 15 May 2020 08:23:28 GMT  
		Size: 2.2 MB (2214019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4a277bd5a433da8c39de2c2e321dbd4481dae6cf8e96e34f5e8c63ff313689`  
		Last Modified: Fri, 15 May 2020 13:10:47 GMT  
		Size: 2.8 MB (2753313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; arm variant v7

```console
$ docker pull hylang@sha256:17ccaffc0650451660b89ba3ca3d59ff218cf4012379caa6343c1a86f4dc66c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48355598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5457617de44cfdeca3a6a4fba1d5a9117d4a19001c1b6bec75412f2c4e434b2`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 01:06:56 GMT
ADD file:a0ecfe1283dbc15e795cd274e422095545ef6e8af80bc23ee7063abb597a5a88 in / 
# Fri, 15 May 2020 01:07:00 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:19:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 03:19:14 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 03:19:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:19:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 15 May 2020 03:46:29 GMT
ENV PYTHON_VERSION=3.6.10
# Fri, 15 May 2020 03:54:52 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 03:54:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 03:54:56 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 03:54:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 03:54:58 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 03:55:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 03:55:34 GMT
CMD ["python3"]
# Fri, 15 May 2020 04:22:07 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 04:22:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 04:22:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:90cadb81644e46b7fbfb33027f8b34af18f1e04db99f6b29cc1ff98aafe9b5d6`  
		Last Modified: Fri, 15 May 2020 01:15:03 GMT  
		Size: 19.3 MB (19304729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb74e57153aa468e45d1446b3eaec3b5e2880a0a445c2a9bdd321b1fd2741ec0`  
		Last Modified: Fri, 15 May 2020 04:17:43 GMT  
		Size: 2.2 MB (2177897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c1f6e1f826bdcc96e243127bf84f39361c3f54093b59622bbba46bfac97978`  
		Last Modified: Fri, 15 May 2020 04:18:29 GMT  
		Size: 21.9 MB (21905548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea172b8a495d12f3479b97835614999abacec1775effb256c49cdba2e1722fc`  
		Last Modified: Fri, 15 May 2020 04:18:21 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93fdc5b795b7a0814a63d57cbc1510cdfb54d83c356eef9ff308fe1e6f4b76`  
		Last Modified: Fri, 15 May 2020 04:18:22 GMT  
		Size: 2.2 MB (2214148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6267ead5c4180915d185b6c8581ee5e8ca1fbf9c20c4fcff1cb1faa7198c59`  
		Last Modified: Fri, 15 May 2020 04:25:26 GMT  
		Size: 2.8 MB (2753036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:8bd6e91c18b8d4d6e579b4b94c2f01f197c7229d42bc34e5b180e901dd93dc2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50799803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417828c8baa4cfc5339ff24f3e4dd93037ff80a459d9acd85784687544e96b6d`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 00:59:03 GMT
ADD file:da103bb73d1c28697756e3558eaa49cc235b07dfea96895f56929eb8fd0fb67c in / 
# Thu, 23 Apr 2020 00:59:05 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:51:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 13:51:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 13:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 13:51:33 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Apr 2020 14:33:31 GMT
ENV PYTHON_VERSION=3.6.10
# Thu, 23 Apr 2020 14:41:55 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 14:41:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 29 Apr 2020 18:08:28 GMT
ENV PYTHON_PIP_VERSION=20.1
# Wed, 29 Apr 2020 18:08:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Wed, 29 Apr 2020 18:08:29 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Wed, 29 Apr 2020 18:09:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 29 Apr 2020 18:09:09 GMT
CMD ["python3"]
# Wed, 29 Apr 2020 19:12:15 GMT
ENV HY_VERSION=0.18.0
# Wed, 29 Apr 2020 19:12:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 29 Apr 2020 19:12:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:191ef9a1fd49ca372c51c235b6f6f4579bddb73cfd390f67b4878b465f9bdfd2`  
		Last Modified: Thu, 23 Apr 2020 01:05:53 GMT  
		Size: 20.4 MB (20370093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1e4abd7f0a1aae36a5263ba3c990b6954c9b65fce50d5dbd68eecfa75b13d`  
		Last Modified: Thu, 23 Apr 2020 15:20:31 GMT  
		Size: 2.2 MB (2238946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07ce497714a72fe7574748eaf24db238870576e9f552fc386261b070881291`  
		Last Modified: Thu, 23 Apr 2020 15:20:38 GMT  
		Size: 23.2 MB (23223057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ff29317bd430c1bfde1999d481451d993a949e2e09c8eb72699ffc9b7a6c3e`  
		Last Modified: Thu, 23 Apr 2020 15:20:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c7057e4b3522a8bd08dfeb4bbf15d01e097f76c10f7b44ea2a889d17f84a2`  
		Last Modified: Wed, 29 Apr 2020 18:17:09 GMT  
		Size: 2.2 MB (2214053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d5ac5e7cbb4d29730b153faa1daee68f768c72fadf78597d652984ecd5e6db`  
		Last Modified: Wed, 29 Apr 2020 19:16:42 GMT  
		Size: 2.8 MB (2753414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; 386

```console
$ docker pull hylang@sha256:cf342739a6d172325fc6088525ba1c4ad32b975dded5a0f8259380156fe8f564
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53470199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f979024bb881adfaba4dd29e2734a61482af87ca9469fdfa90d715721ce9bc5d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 07:12:59 GMT
ADD file:2008ddcaad4151bac993aa4ee2257b34c811b262f730e06af22a1feb84e3c81f in / 
# Fri, 15 May 2020 07:13:00 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:43:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 10:43:28 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 10:43:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:43:44 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 15 May 2020 11:08:06 GMT
ENV PYTHON_VERSION=3.6.10
# Fri, 15 May 2020 11:16:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 11:16:20 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 11:16:21 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 11:16:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 11:16:21 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 11:16:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 11:16:37 GMT
CMD ["python3"]
# Fri, 15 May 2020 11:48:13 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 11:48:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 11:48:19 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a5a8cf045c967a24918301a73357fee572dec550e91771d3a97fb26fc5d61070`  
		Last Modified: Fri, 15 May 2020 07:23:21 GMT  
		Size: 23.1 MB (23147615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25ca329ec400c01fe4bf222537f837eef089f91d5a269912004d1ab8335efd0`  
		Last Modified: Fri, 15 May 2020 11:39:23 GMT  
		Size: 2.5 MB (2533016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7172af62788b8250910aeaec5ad26ca0d5ac6b066d288ce4c4e361dba9295768`  
		Last Modified: Fri, 15 May 2020 11:39:52 GMT  
		Size: 22.8 MB (22822826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88396b696742b255d793b6424f23e2f46c750218e23e73ca2830fa160c92e773`  
		Last Modified: Fri, 15 May 2020 11:39:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d25f70712f6f6f0019a61324133a2a600eda10d4277859138b49297ada0112c`  
		Last Modified: Fri, 15 May 2020 11:39:46 GMT  
		Size: 2.2 MB (2213817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f7fdd5f3d2cfa378b07cca679bbab5da3a598a5f403e840d67f8bf10cc8b76`  
		Last Modified: Fri, 15 May 2020 11:50:56 GMT  
		Size: 2.8 MB (2752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; mips64le

```console
$ docker pull hylang@sha256:ab758237d5a793aa607c799473005b3305cc701b9f9b1869f1fdbc744a43e723
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53120851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e613b677e79b5a40990979edaedbbe03c1a99d003eb13ff39997f72b300df0b1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 04:51:57 GMT
ADD file:98962deede6c5529a4217d0d6c8d403c4804c3de013e043f9838f3bc9b2a2a9c in / 
# Fri, 15 May 2020 04:51:57 GMT
CMD ["bash"]
# Fri, 15 May 2020 06:32:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 06:32:20 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 06:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 06:32:42 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 15 May 2020 07:33:52 GMT
ENV PYTHON_VERSION=3.6.10
# Fri, 15 May 2020 07:53:24 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 07:53:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 07:53:27 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 07:53:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 07:53:28 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 07:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 07:54:11 GMT
CMD ["python3"]
# Fri, 15 May 2020 08:52:43 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 08:52:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 08:52:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9b9d1d2f829f5d8638261d18639c2d5ea32d3784d9a9b3bf6e3c6c2829c0ba71`  
		Last Modified: Fri, 15 May 2020 05:02:30 GMT  
		Size: 22.2 MB (22179472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ddc06cec7ab94e522db0828ac237951ec56f9125c68cd10fb7f6140cdba2e3`  
		Last Modified: Fri, 15 May 2020 08:48:11 GMT  
		Size: 2.1 MB (2110921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe9412c71775a1f4d1cd9bd9a20e64f199fb8642b513d3f581edec893c5df7a`  
		Last Modified: Fri, 15 May 2020 08:49:48 GMT  
		Size: 23.9 MB (23863745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ff5c566466260b03ce1038e8e72dfa20103a869111d2923fadad415a8550e`  
		Last Modified: Fri, 15 May 2020 08:49:24 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfb743bed23918ecb44ac5d772165965c5fa0a7597febfeefd7a1566fdbf25a`  
		Last Modified: Fri, 15 May 2020 08:49:26 GMT  
		Size: 2.2 MB (2213469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234a6d4ffb0ed74a1f77d7a31c54f8ac412088f8524539e06976eb6ff00b78eb`  
		Last Modified: Fri, 15 May 2020 08:55:40 GMT  
		Size: 2.8 MB (2753005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; ppc64le

```console
$ docker pull hylang@sha256:66fa9f0a0ffa794396595ef2389890c1b0f7224b415b3b2fe28a16c6c0033d97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54292443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d56afbcb929b9c11023fd2d65a48d146e29aa1058aecd345e957a56177a827ca`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 00:42:37 GMT
ADD file:a18cd8947224196f50b4845289d03b1f4deafb438223194400da0ed4dae92656 in / 
# Thu, 23 Apr 2020 00:42:40 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:05:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 13:05:09 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 13:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 13:05:33 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Apr 2020 13:55:39 GMT
ENV PYTHON_VERSION=3.6.10
# Thu, 23 Apr 2020 14:07:35 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 14:07:43 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 29 Apr 2020 17:55:55 GMT
ENV PYTHON_PIP_VERSION=20.1
# Wed, 29 Apr 2020 17:55:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Wed, 29 Apr 2020 17:56:03 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Wed, 29 Apr 2020 17:57:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 29 Apr 2020 17:57:33 GMT
CMD ["python3"]
# Wed, 29 Apr 2020 19:22:26 GMT
ENV HY_VERSION=0.18.0
# Wed, 29 Apr 2020 19:22:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 29 Apr 2020 19:22:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4efde6fe2246d87988ee174dc3ed2e4c3158360e5c80fcb0433bc70a732bd77e`  
		Last Modified: Thu, 23 Apr 2020 00:55:34 GMT  
		Size: 22.8 MB (22785405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b36549097b4ed5a0974197d14362130b168a1c2522b3a98eae342c1d17382a7`  
		Last Modified: Thu, 23 Apr 2020 14:57:39 GMT  
		Size: 2.2 MB (2192692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c5c8215a93c31a78a91fc8e5a5d9e7d5cc234bd1cd64e279ea8ca1e40c3da0`  
		Last Modified: Thu, 23 Apr 2020 19:58:41 GMT  
		Size: 24.3 MB (24345405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafd49361f52b88397508a53c258447710d0c29b599f6b9834e1f03b7a7133a8`  
		Last Modified: Thu, 23 Apr 2020 19:58:30 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4288a4aee1b377c407f3d5cf7b87c9fd1e5a32aa9bb0e3916268debc59b81ffa`  
		Last Modified: Wed, 29 Apr 2020 18:10:54 GMT  
		Size: 2.2 MB (2215250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1360417be245dcb979a5b4371e66bb343bac653577a9f98765efe24d9a1a81`  
		Last Modified: Wed, 29 Apr 2020 19:29:16 GMT  
		Size: 2.8 MB (2753448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.6-stretch` - linux; s390x

```console
$ docker pull hylang@sha256:da1c39d89e4e02272b0f0bd51e1231589cbdfc9e20006cac5e41d1b4add34c43
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54785744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0fd1a99d84e1a23eb17a0068388792be1ae4b5a7b625904ce7dfbf7c4593aea`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 14 May 2020 23:08:41 GMT
ADD file:e1cd927f3559fa02ccd2572d2fd827883170cec8852227234d97e7bbe5b4dcb1 in / 
# Thu, 14 May 2020 23:08:43 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:40:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 May 2020 23:40:23 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 23:40:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 23:40:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 14 May 2020 23:51:30 GMT
ENV PYTHON_VERSION=3.6.10
# Thu, 14 May 2020 23:55:50 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 14 May 2020 23:55:52 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 14 May 2020 23:55:53 GMT
ENV PYTHON_PIP_VERSION=20.1
# Thu, 14 May 2020 23:55:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Thu, 14 May 2020 23:55:53 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Thu, 14 May 2020 23:56:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 14 May 2020 23:56:05 GMT
CMD ["python3"]
# Fri, 15 May 2020 00:10:06 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 00:10:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 00:10:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:38486053f3d91064afa779225f4f0240f9ac9ead070d46c3c941242bd19a924c`  
		Last Modified: Thu, 14 May 2020 23:13:04 GMT  
		Size: 22.4 MB (22371322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77afc93fb74fe6ed00def77d79679a3dbde1db644549a30cd8c0a1c4b8720`  
		Last Modified: Fri, 15 May 2020 00:07:26 GMT  
		Size: 2.3 MB (2269066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816bc8f74f564efa17336fee0445b4c9ebea45b87fc7d04c7705cbdb572ff1e5`  
		Last Modified: Fri, 15 May 2020 00:08:04 GMT  
		Size: 25.2 MB (25178895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef6c7b3093d78273018e7e7c121b041c2fadec48131168e1162174f30f887bc`  
		Last Modified: Fri, 15 May 2020 00:08:05 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9240363e6253f167b7febc6a91a8f63933fc27778c7ee17485ed69fd8d1f6`  
		Last Modified: Fri, 15 May 2020 00:08:04 GMT  
		Size: 2.2 MB (2213441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd4ca4256171239425e335df12608892074765bad9754a7a41faeead9fff20b`  
		Last Modified: Fri, 15 May 2020 00:12:48 GMT  
		Size: 2.8 MB (2752782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
