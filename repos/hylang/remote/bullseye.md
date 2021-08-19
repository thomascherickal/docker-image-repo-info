## `hylang:bullseye`

```console
$ docker pull hylang@sha256:47688bc02c14de0b587f054d1e724d5efe183dcade991e6e18c8b1c8098a791f
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

### `hylang:bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:6228b980b3708912758d21d46f4635f6d3b2ffb8e0180a86854ce01cbec88527
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49138994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d1a3d540b04f660822b90c1df66d2c162643852ce84bcd9f3f1637034f29e3`
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
# Tue, 17 Aug 2021 01:54:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:20:58 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 02:20:58 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 02:30:11 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 02:30:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 02:30:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 02:30:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 02:30:13 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 02:30:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 02:30:26 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 00:20:04 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 00:20:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 00:20:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae61f727682a7d9dbb8974480f2674f80187673a550423d383930a4e80cf237`  
		Last Modified: Tue, 17 Aug 2021 03:57:16 GMT  
		Size: 1.1 MB (1075845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466485ee627754b8f2ee4a302965fdea56ac3b2ed509b4f54e9796ab4162e837`  
		Last Modified: Tue, 17 Aug 2021 03:58:27 GMT  
		Size: 11.0 MB (10965504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de739b0566731810358ff60001048daf2672b9c3a9125a3bb2fa65165f26a8eb`  
		Last Modified: Tue, 17 Aug 2021 03:58:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374279231a56d30ab37ec576d0d9f339d627fdaa5e5b99a1a1c6216234e6731`  
		Last Modified: Tue, 17 Aug 2021 03:58:26 GMT  
		Size: 2.6 MB (2640115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1934b91eb2135ba9f17762625c045add3976289cefc87727de4ccef5a081fe50`  
		Last Modified: Thu, 19 Aug 2021 00:23:09 GMT  
		Size: 3.1 MB (3095983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; arm variant v5

```console
$ docker pull hylang@sha256:5a898ba92bab89bcff44b54a914b15292997e2e8e1e2c4b2df8eaa833a1fe44b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46187086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52c02ea02a3b4dada38a75d5be911acd84f4b575a21a1afa7f93c923244afab`
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
# Tue, 17 Aug 2021 03:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:32:28 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 04:32:29 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 04:47:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 04:47:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 04:47:07 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 04:47:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 04:47:08 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 04:47:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 04:47:42 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:48:57 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:49:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:49:08 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4493c45cf886f2d49d222c1e6508b7051515294719ac57ffe7e93f1bb054101`  
		Last Modified: Tue, 17 Aug 2021 07:28:33 GMT  
		Size: 1.1 MB (1059069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d819a4e199fe299641e71d9261cd4fc886bac4f2156656d45297a4fdd3685`  
		Last Modified: Tue, 17 Aug 2021 07:30:10 GMT  
		Size: 10.5 MB (10487590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076fc9212e3756eef91c3e73586c5e5f808e445d6e3feb50614b9731033de458`  
		Last Modified: Tue, 17 Aug 2021 07:30:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f737070e9e56bbe250ba7eaeaeb42f37b6295f837bd0e8323850d504a0e2220`  
		Last Modified: Tue, 17 Aug 2021 07:30:07 GMT  
		Size: 2.6 MB (2639899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497dbf3270837d5cafb930903637640b7ebbe2bd9b84d5ebec674586cda2ac4`  
		Last Modified: Wed, 18 Aug 2021 23:54:14 GMT  
		Size: 3.1 MB (3096127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; arm variant v7

```console
$ docker pull hylang@sha256:c7e89b9bfe70e3f0ebb9be9f8c2c62c3072b6c7416eeb50ffde9fcb0d6319697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43390507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b12c9a6558e01e8f304a7a4e3fd78e5e329f7a8dcfba18294d56c10ae90e63`
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
# Tue, 17 Aug 2021 03:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:34:03 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 04:34:03 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 04:55:47 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 04:55:49 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 04:55:49 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 04:55:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 04:55:50 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 04:56:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 04:56:20 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 04:28:38 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 04:28:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 04:28:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28072302e8164c0cbda51fce73bd0e077126c4421dd143a4783268ff63a101a2`  
		Last Modified: Tue, 17 Aug 2021 08:26:31 GMT  
		Size: 1.0 MB (1041281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c0ce6d0be1406a3c975a6873ff96342d78fd9e7c03ef070ebfab07025d4dc`  
		Last Modified: Tue, 17 Aug 2021 08:28:24 GMT  
		Size: 10.0 MB (10047345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c0b89dac903a886786de4a9d76ace799869b0f14d214af1299bbd7da80868d`  
		Last Modified: Tue, 17 Aug 2021 08:28:17 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5f63796f35a4b938c1113f696c2c54f264f62bfc8206a45df032d0b9c2dc14`  
		Last Modified: Tue, 17 Aug 2021 08:28:19 GMT  
		Size: 2.6 MB (2639914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce04b0fad96ab5b88cb04d6297c8fd8435f45c4636e18eb2ba3b3d30e252143`  
		Last Modified: Thu, 19 Aug 2021 04:38:28 GMT  
		Size: 3.1 MB (3096162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:0ce75256521062c7c016daded00a854974748f8fc78a5e9bf2c8d62578c33d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47811853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1af743a5337dde0dad7ac13877136bc5cf395fca5f9e00a7a3314e9525c5dc`
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
# Tue, 17 Aug 2021 02:18:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:39:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 02:39:05 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 02:45:24 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 02:45:24 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 02:45:25 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 02:45:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 02:45:25 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 02:45:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 02:45:39 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:40:21 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:40:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:40:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c366d4a5a53a7068e1ac8c8b63a619ef6fd9f2394bfdd6e131c0c92b68865d6`  
		Last Modified: Tue, 17 Aug 2021 03:59:46 GMT  
		Size: 1.1 MB (1064339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80361469e78fdc8824f4aa49ec5fb3b6c85d545b50e6cb917cf791462104b711`  
		Last Modified: Tue, 17 Aug 2021 04:01:05 GMT  
		Size: 11.0 MB (10962809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff3339d45e4e8354a02f47bc2b119b6606a455e475c906d4466f8cd65898bd`  
		Last Modified: Tue, 17 Aug 2021 04:01:04 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b8554d24f8a6f29e8deb1fefc91499d304d7dc383e216c908cc6d678080d9a`  
		Last Modified: Tue, 17 Aug 2021 04:01:04 GMT  
		Size: 2.6 MB (2639760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f0f7d257939fdd3e704f0502258300077652260ce14811e9864829963fa3e6`  
		Last Modified: Wed, 18 Aug 2021 23:45:46 GMT  
		Size: 3.1 MB (3095912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; 386

```console
$ docker pull hylang@sha256:c2125e9d2d777e71c4791ae62a66fd96bbbc94d7d97e79fb3598be6d1b5a67d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50267387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa3215275bc88a8abfbb884bbfef7fb6b9bdb9f7664214c78e2a42eec38c2d5`
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
# Tue, 17 Aug 2021 02:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 03:42:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 03:42:50 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 03:55:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 03:55:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 03:55:06 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 03:55:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 03:55:06 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 03:55:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 03:55:21 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:39:26 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:39:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:39:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe99215de170cec2910b957ec73f29a0e86ae89280c67408df7ed211011944a`  
		Last Modified: Tue, 17 Aug 2021 07:03:10 GMT  
		Size: 1.1 MB (1088286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219996341bcba86c7c0be2b9c40b397c7cc58ac0d5c5a6de908d2d2584585ba2`  
		Last Modified: Tue, 17 Aug 2021 07:04:46 GMT  
		Size: 11.1 MB (11067513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67c1b72e296b166c010f2c67d996156c5b1d24805c02e382f950198116d45e4`  
		Last Modified: Tue, 17 Aug 2021 07:04:43 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8c1d4627307ea64caa51655fe4989e89b6971d9de89990d9184edbaff72ebf`  
		Last Modified: Tue, 17 Aug 2021 07:04:44 GMT  
		Size: 2.6 MB (2639750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ed8d38e1b11768206f02ad748d6b12befc37adc098c1ec22953c178cb50a4`  
		Last Modified: Wed, 18 Aug 2021 23:45:06 GMT  
		Size: 3.1 MB (3095947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; mips64le

```console
$ docker pull hylang@sha256:0399184825ec3b830b90ea8318aa60a8284bc34e56e7f53af241952ce8040c0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47238562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a3ee89a77bdbf37547521a549c2114a2df594891c6b28aa9d44ba510b5d5e1`
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
# Tue, 17 Aug 2021 02:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 05:12:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 05:12:01 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 05:58:41 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 05:58:43 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 05:58:43 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 05:58:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 05:58:44 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 05:59:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 05:59:29 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 00:07:33 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 00:07:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 00:07:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8375ff99ce3f614d73dc69b03575c7ebf072f4e05da52b0319fc3782d5ebb578`  
		Last Modified: Tue, 17 Aug 2021 01:20:19 GMT  
		Size: 29.6 MB (29619986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9f3ed4fbce841601e9f43bf8967207ce69aff2eb78dac4cb8e3f02f1d9bcf1`  
		Last Modified: Tue, 17 Aug 2021 12:38:58 GMT  
		Size: 1.0 MB (1049228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b9553ed1f9d716b216c168e6f84ff6ae472156c9c77982d50f58742b9df53`  
		Last Modified: Tue, 17 Aug 2021 12:40:21 GMT  
		Size: 10.8 MB (10833330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a43ed3375608c3e614e5d816d1eacf168b79f2e3b9ef62393270a984b3b9ff`  
		Last Modified: Tue, 17 Aug 2021 12:40:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f994bb81fc9b616cde5a79892d6a7a905f1f2dfa17b2924349b22778642dd`  
		Last Modified: Tue, 17 Aug 2021 12:40:16 GMT  
		Size: 2.6 MB (2639662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25600acb09b68d0e454815ebae514ca5cc64f9959ffe2c6423540dcd82f5ff2`  
		Last Modified: Thu, 19 Aug 2021 00:09:59 GMT  
		Size: 3.1 MB (3096123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; ppc64le

```console
$ docker pull hylang@sha256:3d2b0bc1c657a5a2e6bed8604054b93afea3267eb333cb07c7539901c3fafe12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53428688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:654a574bcfe4c02df1ac9b8f742c1b35baf9ef6548f4819c018049f66a31961d`
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
# Tue, 17 Aug 2021 02:17:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 03:27:03 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 03:27:08 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 03:53:27 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 03:53:52 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 03:53:57 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 03:54:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 03:54:12 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 03:55:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 03:55:40 GMT
CMD ["python3"]
# Thu, 19 Aug 2021 02:30:33 GMT
ENV HY_VERSION=1.0a3
# Thu, 19 Aug 2021 02:31:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 19 Aug 2021 02:31:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24905932468a38a3bb273fd0b16d40e7478875b2f795a5cf0cdff5890bc964c2`  
		Last Modified: Tue, 17 Aug 2021 07:30:26 GMT  
		Size: 1.1 MB (1094468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf273f654790f4b9d64882e1edd5b98e50c7090b6218712efdefcb4c2063ac8`  
		Last Modified: Tue, 17 Aug 2021 07:31:46 GMT  
		Size: 11.3 MB (11331190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027c9d78230794fa5e16461a397c6f9798cdf1ff53d8e139a151a9e979ac88f4`  
		Last Modified: Tue, 17 Aug 2021 07:31:43 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c90c47e68a2ceb4a189cad422b8500c08c58e52f2650038985fcbb7ea82eac9`  
		Last Modified: Tue, 17 Aug 2021 07:31:43 GMT  
		Size: 2.6 MB (2641867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007ee73c68ee9b5d63a8ae7c3645b07a7fbe1632f942bdf74941d2392e01f703`  
		Last Modified: Thu, 19 Aug 2021 02:41:56 GMT  
		Size: 3.1 MB (3096920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:bullseye` - linux; s390x

```console
$ docker pull hylang@sha256:a425865f1859c1a5bb247f1bb7f10d26f9091ab5fb17367ce9900ec97ddb9ac2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47230076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53bbccc07c70aa0d6eca6473453443df3a7b1505b080c2f10471def3a605779`
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
# Tue, 17 Aug 2021 02:21:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:44:30 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 17 Aug 2021 02:44:30 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 17 Aug 2021 02:50:30 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 17 Aug 2021 02:50:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 17 Aug 2021 02:50:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 17 Aug 2021 02:50:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 17 Aug 2021 02:50:34 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 17 Aug 2021 02:50:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 17 Aug 2021 02:50:49 GMT
CMD ["python3"]
# Wed, 18 Aug 2021 23:42:16 GMT
ENV HY_VERSION=1.0a3
# Wed, 18 Aug 2021 23:42:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 18 Aug 2021 23:42:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091548844f51e9f781482ae5059c00df5fe55fb86ea6f276e2dedb65dcffce2c`  
		Last Modified: Tue, 17 Aug 2021 04:09:35 GMT  
		Size: 1.1 MB (1075366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6af61257aad320f1cdabe55f50cff56d6c9887fc0c80d88880d3f645944904`  
		Last Modified: Tue, 17 Aug 2021 04:10:31 GMT  
		Size: 10.8 MB (10771601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae78897d124113081bb1bacdc554e3aefb3382655aa485285bee5e23a091e82`  
		Last Modified: Tue, 17 Aug 2021 04:10:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf256876167eb1cd2f98fcea77132227a0b21a3a276afb7781b1c887618166c`  
		Last Modified: Tue, 17 Aug 2021 04:10:30 GMT  
		Size: 2.6 MB (2639879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dd288beee35fe52de8e1bddc411274c931c1c0111a86600fbfc2803727d4f4`  
		Last Modified: Wed, 18 Aug 2021 23:46:42 GMT  
		Size: 3.1 MB (3095970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
