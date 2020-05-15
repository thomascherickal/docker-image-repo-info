## `hylang:0-buster`

```console
$ docker pull hylang@sha256:6d539c5a31330217ac0b861d2d9fa06e38af2f21f952800fc0dcb7cae83e1183
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

### `hylang:0-buster` - linux; amd64

```console
$ docker pull hylang@sha256:790456f18a43e4817f3c87ef0036cb36201dcc33e2257f13d54226224e66adcd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65972761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145463f38a0e3877c5d765e2d16e9b1b5a2d15a702ba4746ba73774445328dcf`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:17:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 11:17:32 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 11:17:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:17:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 11:17:40 GMT
ENV PYTHON_VERSION=3.8.3
# Fri, 15 May 2020 11:28:41 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 11:28:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 11:28:42 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 11:28:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 11:28:43 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 11:28:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 11:28:56 GMT
CMD ["python3"]
# Fri, 15 May 2020 12:28:54 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 12:29:01 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 12:29:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf47e503ea90fb83d7f185a9a929560b5d9f75ae715bf6eb1aaaeaa3f06bc40`  
		Last Modified: Fri, 15 May 2020 12:27:01 GMT  
		Size: 2.7 MB (2749097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b3e3d1255f2960514b419b363ed4b1dccb5c82c74a9d0bf3d9fea6e9122939`  
		Last Modified: Fri, 15 May 2020 12:27:07 GMT  
		Size: 31.1 MB (31095184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7661b83ac739c561940d7488de1797670207986b74b4831ccdfe885b7bb3566`  
		Last Modified: Fri, 15 May 2020 12:27:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab48912491af821f62d72c1969ad5157e1edf54f31dc6584ab54d1ec2d83c35`  
		Last Modified: Fri, 15 May 2020 12:27:01 GMT  
		Size: 2.2 MB (2218958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53517d7fca6c6d8a923021b965e81e1f9645ea005fad12535463787c80c212fa`  
		Last Modified: Fri, 15 May 2020 12:32:17 GMT  
		Size: 2.8 MB (2810533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:04b1adb0eb9ef3d752bf4f18f80969e97da8ca19f2f15c6bc91acd130c8a49d8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60858617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e65ed789512b141afab1e6426b608e69893df7895328c50854896e113f37eda0`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:59:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 05:59:57 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 06:00:15 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 06:00:16 GMT
ENV PYTHON_VERSION=3.8.3
# Fri, 15 May 2020 06:13:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 06:13:52 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 06:13:53 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 06:13:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 06:13:55 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 06:14:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 06:14:28 GMT
CMD ["python3"]
# Fri, 15 May 2020 13:06:31 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 13:06:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 13:06:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470b259359208d20211d57cf65bda82a48f01e1411de914fc3d113b5dc49a25e`  
		Last Modified: Fri, 15 May 2020 08:21:04 GMT  
		Size: 2.4 MB (2448096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61862c372453ae6632bd06fea5df780d0096775a664d9a045bc176f359e4da47`  
		Last Modified: Fri, 15 May 2020 08:21:17 GMT  
		Size: 28.5 MB (28541876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf7127426977da67929e545164585ac30197b609f892e5bc7f745ad864e6bb`  
		Last Modified: Fri, 15 May 2020 08:21:04 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d645b537f04728c4f3cde6e61b59df2d054b04d9ef81ec81c3d4ddda5131d82f`  
		Last Modified: Fri, 15 May 2020 08:21:04 GMT  
		Size: 2.2 MB (2218779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af611b743f6b2641c01106133da9ad19b6cf033609e8ed2f5069fa61857bb2d`  
		Last Modified: Fri, 15 May 2020 13:10:06 GMT  
		Size: 2.8 MB (2811164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:c039180d7a7ccced276df60bb3fe9edd2192f8bc6c59a42bc96cf3a77141a418
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58146418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fdfcee9febed4c2c7c44bd7573c5a97dc724d0fa7ce3e6b07dfd5e5fc4ecdda`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 02:47:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 02:47:22 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 02:47:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 02:47:39 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 02:47:39 GMT
ENV PYTHON_VERSION=3.8.3
# Fri, 15 May 2020 03:01:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 03:01:24 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 03:01:27 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 03:01:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 03:01:29 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 03:02:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 03:02:03 GMT
CMD ["python3"]
# Fri, 15 May 2020 04:19:46 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 04:19:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 04:19:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c7698a4d77144751a47e2b5394b243967a950e4831863e2a77b0387dd5671f`  
		Last Modified: Fri, 15 May 2020 04:17:01 GMT  
		Size: 2.3 MB (2345917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831e7439d483321c300d994cfab6dfba217fedfb116a9768eb68eb28878fb517`  
		Last Modified: Fri, 15 May 2020 04:17:11 GMT  
		Size: 28.1 MB (28064664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1c9d50c648c45e05b0f7f8f1f2b7b27ac86e689f6e41a1022d95b180433b6`  
		Last Modified: Fri, 15 May 2020 04:17:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c7fa1024a3babc645d0837104c1bd3f031b37b1648d2c2aca8ca458b6b1be0`  
		Last Modified: Fri, 15 May 2020 04:17:02 GMT  
		Size: 2.2 MB (2218953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2891d6be18957bd56cefdf085536b770b12cc4dfbde81917c4ca6c479998f8a5`  
		Last Modified: Fri, 15 May 2020 04:24:10 GMT  
		Size: 2.8 MB (2810726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:6f36c9703d286d9a9d1098b8de01ff07b944c435d1bec6505b990e06a25b8cd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63576529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b1c71e670ea64c298ad8a7534b60de9fbe63149f5d775ed90b2bde9137d19b`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 12:59:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 12:59:33 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 12:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 12:59:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 23 Apr 2020 12:59:47 GMT
ENV PYTHON_VERSION=3.8.2
# Thu, 23 Apr 2020 13:09:36 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 13:09:40 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 29 Apr 2020 18:01:15 GMT
ENV PYTHON_PIP_VERSION=20.1
# Wed, 29 Apr 2020 18:01:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Wed, 29 Apr 2020 18:01:19 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Wed, 29 Apr 2020 18:01:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 29 Apr 2020 18:01:55 GMT
CMD ["python3"]
# Wed, 29 Apr 2020 19:10:05 GMT
ENV HY_VERSION=0.18.0
# Wed, 29 Apr 2020 19:10:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 29 Apr 2020 19:10:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538d0f6124c2ad1cad6bcdbcfb70e62d493c2e5220f52cb7f64772a6c92919cb`  
		Last Modified: Thu, 23 Apr 2020 15:19:22 GMT  
		Size: 2.6 MB (2622296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b414093370b8458e41f4550a53581ff85095662879abbb2521cbc02b2bf26d3`  
		Last Modified: Thu, 23 Apr 2020 15:19:31 GMT  
		Size: 30.1 MB (30066565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcda210f8f871d909b2e8ed0a9d831d6866063c5431f9264ba01d3a07f5efee4`  
		Last Modified: Thu, 23 Apr 2020 15:19:21 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed03bf55d7f03788fed958549c1bf758b1320bf55b726a6b30beb960b0ac8e98`  
		Last Modified: Wed, 29 Apr 2020 18:15:32 GMT  
		Size: 2.2 MB (2218982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97af9133dd724cc1b9cadafb7cb68ec90b77c7c4399d477427fdf8adc68cdfd`  
		Last Modified: Wed, 29 Apr 2020 19:15:08 GMT  
		Size: 2.8 MB (2810651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; 386

```console
$ docker pull hylang@sha256:3316753e92e463e658cfb227785ad2404aa15f98aabc33f3e4367ecfb8a5a2ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64744729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e095678ad75c060e3fa2b2ab8d8fa817240d8370abed062d6d933be8715ace9`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:07:46 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 10:07:46 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 10:07:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:08:00 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 10:08:00 GMT
ENV PYTHON_VERSION=3.8.3
# Fri, 15 May 2020 10:25:16 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 10:25:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 10:25:17 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 10:25:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 10:25:17 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 10:25:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 10:25:43 GMT
CMD ["python3"]
# Fri, 15 May 2020 11:47:02 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 11:47:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 11:47:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42469d7380d795ba959212081b4efd96e165c72ad38f51952ffa94bb4a9b1204`  
		Last Modified: Fri, 15 May 2020 11:38:50 GMT  
		Size: 2.8 MB (2762597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35a6ec4b7de44812da21c3de33c3bb101acaf0414bea42e329d4f0e50a1d8bb`  
		Last Modified: Fri, 15 May 2020 11:38:58 GMT  
		Size: 29.2 MB (29197838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fec319f69ed95933900eed0feb3dcf7fbff0975949f9073a4d4ae4d1b6293`  
		Last Modified: Fri, 15 May 2020 11:38:49 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25230f1c1ab1eb7b48e321ff3c56ca5753a3c6e41306a0e41d5e001846bcbffb`  
		Last Modified: Fri, 15 May 2020 11:38:51 GMT  
		Size: 2.2 MB (2218629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f67b188095f24c7ab3e6b2c07d5ff5b8c7f887c21dfdb32f68e89d0b7dfa8b4`  
		Last Modified: Fri, 15 May 2020 11:49:44 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:6d965f9b133fc46eddbf0b94d3a2cc1b0a1b8bda65de851ea765b48e98216858
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63756274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f9a627d2c103162a7efa0b322693aa43e413a339493ce09012ae497a9d3de59`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 15 May 2020 04:48:19 GMT
ADD file:1163d3a5831eb58d132b66b60303169816e7bd8289f19caaac1157179a95f6f9 in / 
# Fri, 15 May 2020 04:48:19 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:06:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 05:06:09 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 05:06:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:06:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 05:06:27 GMT
ENV PYTHON_VERSION=3.8.3
# Fri, 15 May 2020 05:49:09 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 05:49:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 05:49:12 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 05:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 05:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 05:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 05:49:53 GMT
CMD ["python3"]
# Fri, 15 May 2020 08:51:25 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 08:51:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 08:51:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d22357c747999d33ec7501da2c05aa9e95079ebddefbcb326976c5ed5b176b3f`  
		Last Modified: Fri, 15 May 2020 04:57:10 GMT  
		Size: 25.8 MB (25764292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389f36570e3ce36ace69142916f704cf2dc80d8df1d57832fdeace3638bd1d1`  
		Last Modified: Fri, 15 May 2020 08:46:36 GMT  
		Size: 2.3 MB (2309008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed778839b957f68ae3c9e8f225c5a004fe4d0e3d6d35b6defe47083f04e08c`  
		Last Modified: Fri, 15 May 2020 08:47:02 GMT  
		Size: 30.7 MB (30653496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60ba2d6d9809037aa0ae295b43f01209a015fe2dbf0cd77f21295fce5cd2e85`  
		Last Modified: Fri, 15 May 2020 08:46:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94c6c48f8eec367a70fa7da3a70381df2d410e98f95009566ce473f1ade7ed`  
		Last Modified: Fri, 15 May 2020 08:46:36 GMT  
		Size: 2.2 MB (2218411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46886bedc219c159cc44d74d5f1c2c5b36addc2a0e25eba276390df79ee99e17`  
		Last Modified: Fri, 15 May 2020 08:54:13 GMT  
		Size: 2.8 MB (2810835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:1c013160ff601e015f9f767cdbcffe1749adf80a5e9892c9a2d4373c8a476474
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70415226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8cfc84e4832d761bf1327ed6a2e45dccc8ae7385d542ffdec0c584a28fd0f4`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 00:59:56 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 12:06:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 12:06:07 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 23 Apr 2020 12:06:11 GMT
ENV PYTHON_VERSION=3.8.2
# Thu, 23 Apr 2020 12:20:58 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 23 Apr 2020 12:21:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 29 Apr 2020 17:43:46 GMT
ENV PYTHON_PIP_VERSION=20.1
# Wed, 29 Apr 2020 17:43:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Wed, 29 Apr 2020 17:43:52 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Wed, 29 Apr 2020 17:44:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 29 Apr 2020 17:44:38 GMT
CMD ["python3"]
# Wed, 29 Apr 2020 19:18:20 GMT
ENV HY_VERSION=0.18.0
# Wed, 29 Apr 2020 19:18:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 29 Apr 2020 19:18:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cb5076c799329dc89187a26d1abe3fce98e16a90a828966bf55c6bf1d915d2`  
		Last Modified: Thu, 23 Apr 2020 14:54:54 GMT  
		Size: 2.9 MB (2871706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59df2fc5fe5a66d21ac1b47383b6544b6b74e79685e5ea5fc19f5c78d982b90`  
		Last Modified: Thu, 23 Apr 2020 14:55:11 GMT  
		Size: 32.0 MB (31987401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082908ce76923f53cd35f426cb4c3a3471d6f4302dfba1adff0aaa4853e04309`  
		Last Modified: Thu, 23 Apr 2020 14:54:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf846455b7ef55a7f2b079e8a2834b9d464d1ccead1f0e9554ef9a0c8bea05cc`  
		Last Modified: Wed, 29 Apr 2020 18:08:04 GMT  
		Size: 2.2 MB (2220251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17db4b64b1d9c6fb5af33b8456d2b8eff1b7a2b4bdfb5f6c185a231aa2868585`  
		Last Modified: Wed, 29 Apr 2020 19:26:40 GMT  
		Size: 2.8 MB (2810995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; s390x

```console
$ docker pull hylang@sha256:89994ede024521066de24e7ca16959983e768104e364e6d83caf2c70cf989134
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63961928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b389d97b854e32743298f847ca59586391b644cfb39a9327390129e2ec022c3b`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:29:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 May 2020 23:29:06 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 23:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 23:29:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 14 May 2020 23:29:11 GMT
ENV PYTHON_VERSION=3.8.3
# Thu, 14 May 2020 23:34:01 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 14 May 2020 23:34:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 14 May 2020 23:34:03 GMT
ENV PYTHON_PIP_VERSION=20.1
# Thu, 14 May 2020 23:34:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Thu, 14 May 2020 23:34:03 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Thu, 14 May 2020 23:34:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 14 May 2020 23:34:14 GMT
CMD ["python3"]
# Fri, 15 May 2020 00:09:02 GMT
ENV HY_VERSION=0.18.0
# Fri, 15 May 2020 00:09:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 15 May 2020 00:09:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7df72789485ce816b1118bfcfc62a6bf98e3302780d2d7832d4da361dfba3a`  
		Last Modified: Fri, 15 May 2020 00:06:50 GMT  
		Size: 2.4 MB (2442337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c650cdc83ba245cd3df19245fd365a9ec6d052122d004bdf0bb59c270ac87111`  
		Last Modified: Fri, 15 May 2020 00:06:58 GMT  
		Size: 30.8 MB (30777180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1667870b64fe0c21149df827e0046d0253efcc16ae39f8746d639511f627c`  
		Last Modified: Fri, 15 May 2020 00:07:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebe24670a3f0938645217f2db0103c986670c5319d1c4a4c35ca4666308788c`  
		Last Modified: Fri, 15 May 2020 00:06:55 GMT  
		Size: 2.2 MB (2218536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d881a2cf5fd08a666c36832ac14218c285321cace37d26f17b47fb9ebba84`  
		Last Modified: Fri, 15 May 2020 00:11:49 GMT  
		Size: 2.8 MB (2810711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
