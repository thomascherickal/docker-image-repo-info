## `hylang:python3.10-rc-buster`

```console
$ docker pull hylang@sha256:6777050e6b9c8fd95423de182a0719e8740a3bba6e6d13a7e531304bedeea755
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

### `hylang:python3.10-rc-buster` - linux; amd64

```console
$ docker pull hylang@sha256:85dc6abdb43658ea99cc7d3c5dc42d23c3666880acd8e79a8fa4f17b1910169d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46884901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df42be4f9fc0048e4e7901ff66330d7f25427ab8e99014d5ec20f62863b2d38d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:24 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 01:44:24 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 01:44:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:44:32 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 01:44:32 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 01:53:30 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 01:53:31 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 01:53:31 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 01:53:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 01:53:32 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 01:53:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 01:53:47 GMT
CMD ["python3"]
# Fri, 03 Sep 2021 21:18:22 GMT
ENV HY_VERSION=1.0a3
# Fri, 03 Sep 2021 21:18:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 03 Sep 2021 21:18:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ea433a9572670eceec19913c64e365f711b13e24378ccfe5c3c318545c8043`  
		Last Modified: Fri, 03 Sep 2021 03:22:55 GMT  
		Size: 2.8 MB (2770118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ee2331ed5cc0c85bc0371346596138ed7cf7c757cbba90330a77007284e9df`  
		Last Modified: Fri, 03 Sep 2021 03:22:56 GMT  
		Size: 11.1 MB (11065858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6fbc58d7649f5d2f9705e79f84eb723ab6012040f937ac8d3f5adcb64641d1`  
		Last Modified: Fri, 03 Sep 2021 03:22:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbf6ee4070074c589b99eda478007ef34a63fe15dfffe269814efda2e27f69c`  
		Last Modified: Fri, 03 Sep 2021 03:22:55 GMT  
		Size: 2.6 MB (2636730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4558141b7a6acfc949b07df4129908972164d2d1d99ff2e90d68ec23af9989`  
		Last Modified: Fri, 03 Sep 2021 21:22:39 GMT  
		Size: 3.3 MB (3266121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:a1434d4b44258df769524de591322fb54f75842575ff268ab024d38e3a5ec62f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43960354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:963d183a9aa018693fc587ec90f2c224d1cba37b780fc988f8c20f854d1330e1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:12:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:12:31 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:12:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:12:53 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 13:12:54 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 13:28:31 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 13:28:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 13:28:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 13:28:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 13:28:34 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 13:29:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 13:29:09 GMT
CMD ["python3"]
# Sat, 04 Sep 2021 04:40:48 GMT
ENV HY_VERSION=1.0a3
# Sat, 04 Sep 2021 04:40:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 04 Sep 2021 04:41:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c0f7237cecebe4726c383f06f45ea83634f06ae1adda877e58474ae99a850`  
		Last Modified: Fri, 03 Sep 2021 16:42:27 GMT  
		Size: 2.5 MB (2460710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4b0bc987b755075e95cbbed83aba6aa8e0ee9230dd0935ba532e4dce5536fe`  
		Last Modified: Fri, 03 Sep 2021 16:42:33 GMT  
		Size: 10.7 MB (10717348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af84e1af2cd03d07ddbbb333ca21adc7c0d1d63a4048d6a229bd939200ddafc2`  
		Last Modified: Fri, 03 Sep 2021 16:42:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe0aaf43381261ab3faf9dc640bef95fcca0d8868a717e8119f427abed1b436`  
		Last Modified: Fri, 03 Sep 2021 16:42:28 GMT  
		Size: 2.6 MB (2636376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b788991e6ecd3e427a0e3e9263bad5b3e9d01917766ff81513ae32007c9cc590`  
		Last Modified: Sat, 04 Sep 2021 04:45:25 GMT  
		Size: 3.3 MB (3266578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:65980f7212f316b4f6cae8824a3048d5418982b1508ef7034540a644c384166f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41243555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0663a1bc7bf64fe5f338d984245ad68f9e30b3868e53a33980c876324c692a7d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 18:02:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 18:02:05 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 18:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 18:02:25 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 18:02:26 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 18:22:24 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 18:22:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 18:22:27 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 18:22:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 18:22:28 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 18:22:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 18:22:58 GMT
CMD ["python3"]
# Sat, 04 Sep 2021 23:02:08 GMT
ENV HY_VERSION=1.0a3
# Sat, 04 Sep 2021 23:02:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 04 Sep 2021 23:02:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa1209a00e067346e307e9f7b77640d7a1cd76871efbfabd234fc9c211aa1b`  
		Last Modified: Fri, 03 Sep 2021 23:57:14 GMT  
		Size: 2.4 MB (2358934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda74ff4e45e363e1af8b3e7148f9bae9b94670d5e0db32f1fa3faed1087c1c2`  
		Last Modified: Fri, 03 Sep 2021 23:57:19 GMT  
		Size: 10.2 MB (10235183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acae72811eaeaa15cd3a0d77e8dd92b70bc4fcf625be95ab3556fa483081fe6`  
		Last Modified: Fri, 03 Sep 2021 23:57:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb50a3112a710cfc546d325818d51631e7466baa4b74bf32ceb497dbb58f93`  
		Last Modified: Fri, 03 Sep 2021 23:57:15 GMT  
		Size: 2.6 MB (2636455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aa08ec99aa40c7975853c3c6a7b281ae815d389c333da587fde0082f922c2b`  
		Last Modified: Sat, 04 Sep 2021 23:11:18 GMT  
		Size: 3.3 MB (3266601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:ac8c041300aa91ae5bb8f4c55ffc4663c354644fa38eae8b245ae5000ed09830
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45527018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2249d84f691db95c40c6565f25eeeda966d0bf72e9af344777d620bb6d4a8211`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:07:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 05:07:18 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 05:07:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:07:24 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 05:07:24 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 05:14:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 05:14:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 05:14:03 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 05:14:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 05:14:03 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 05:14:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 05:14:17 GMT
CMD ["python3"]
# Fri, 03 Sep 2021 13:44:41 GMT
ENV HY_VERSION=1.0a3
# Fri, 03 Sep 2021 13:44:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 03 Sep 2021 13:44:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25c18b3a0433f2d2b9b108a379ca7357b8de96ae95cb06504aa9f07392cb83f`  
		Last Modified: Fri, 03 Sep 2021 07:08:32 GMT  
		Size: 2.6 MB (2636426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1c0eef36ff71347a1f60d0cad9eee6e71cdd4b131e8538ad5f745ac56c088b`  
		Last Modified: Fri, 03 Sep 2021 07:08:33 GMT  
		Size: 11.1 MB (11072887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df1ad249d00b96719beb591a67bf85e61e594f80683ae944a22b62d21a430ea`  
		Last Modified: Fri, 03 Sep 2021 07:08:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebb75532a806c633762225ba1978b27a5e2cf9e612602393af8ad6171e291d3`  
		Last Modified: Fri, 03 Sep 2021 07:08:32 GMT  
		Size: 2.6 MB (2636435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5b4849f00cb51f91603576b9570d3ae5d267e25e2c2632093b2e0a8141bcf4`  
		Last Modified: Fri, 03 Sep 2021 13:51:04 GMT  
		Size: 3.3 MB (3266179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; 386

```console
$ docker pull hylang@sha256:f01a6322d52ced29d0355e685b60eab59f19bdbb1e76178a126d93156317be72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47689200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ad44980a98cfb485e3c99e67f54d311922955aa146edcef3cba400810520ed`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:33:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:33:39 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:33:55 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 17:33:55 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 17:48:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 17:48:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 17:48:11 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 17:48:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 17:48:12 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 17:48:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 17:48:28 GMT
CMD ["python3"]
# Sat, 04 Sep 2021 06:42:17 GMT
ENV HY_VERSION=1.0a3
# Sat, 04 Sep 2021 06:42:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 04 Sep 2021 06:42:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c50c96afac2f05d99ceadbd51f6e960f003ebcfdfb6cc11dab774131b187ae`  
		Last Modified: Fri, 03 Sep 2021 21:14:31 GMT  
		Size: 2.8 MB (2781634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c71d3d418e6d9e6cf8595571dfc7448279e1c53621e83d907c284da24e3207`  
		Last Modified: Fri, 03 Sep 2021 21:14:32 GMT  
		Size: 11.2 MB (11207007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516f52e4cda7600e50d517a5163ea479070cde759e50289e1e2c26736ead2450`  
		Last Modified: Fri, 03 Sep 2021 21:14:29 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d73a34a27b838f861483a6ba8be27aeb304ca0bd11e028a57e8db6e489d7708`  
		Last Modified: Fri, 03 Sep 2021 21:14:30 GMT  
		Size: 2.6 MB (2636497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51b18f3677f8639b26f6998b3e521fab9037de3f388b14f71e33f3f5e08a70`  
		Last Modified: Sat, 04 Sep 2021 06:51:09 GMT  
		Size: 3.3 MB (3266316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:046758a3470f2ac91bb60a4808ef276d9dfcc4a7d89e3ffadc7b41f77a92e44d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44993896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:398d0a3b012e1637f8768abc905df8784329ae48e01bf18f5018f25f8d135829`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:49 GMT
ADD file:219b2ce847fd4b227257f60cf40dee2eaf7688371fd76658752f6ccbac9c4353 in / 
# Fri, 03 Sep 2021 01:10:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:55:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:55:41 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:55:58 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 17:55:58 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 18:38:57 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 18:38:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 18:38:59 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 18:39:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 18:39:00 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 18:39:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 18:39:45 GMT
CMD ["python3"]
# Sat, 04 Sep 2021 11:39:05 GMT
ENV HY_VERSION=1.0a3
# Sat, 04 Sep 2021 11:39:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 04 Sep 2021 11:39:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c11f388d181c313e7657eea7b1ffa2d20856b4701922412adea724a19acdb79f`  
		Last Modified: Fri, 03 Sep 2021 01:19:51 GMT  
		Size: 25.8 MB (25812853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a53fc00eff7eb2abe8e5d63a84e31921f1f5cabf07a3d83bea2ce4839378bd`  
		Last Modified: Sat, 04 Sep 2021 05:26:25 GMT  
		Size: 2.3 MB (2321363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58193c4abe3cf180f08b8f3bbb88c85b192a4df28010ec7ff5f92c12b339197b`  
		Last Modified: Sat, 04 Sep 2021 05:26:30 GMT  
		Size: 11.0 MB (10956949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29bfb7ca0785b8eb67ed4b19b278d0f230b9b343f15606fef5cec2a1963c9a`  
		Last Modified: Sat, 04 Sep 2021 05:26:23 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373225de3991935b56dc0244a01762f30edcf2ae6b481d115dbbdca036247254`  
		Last Modified: Sat, 04 Sep 2021 05:26:25 GMT  
		Size: 2.6 MB (2636166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab22010f02dfda3ad8f0af423883c963259243aa4c22fc5899b1e5ab3f0fa268`  
		Last Modified: Sat, 04 Sep 2021 11:42:10 GMT  
		Size: 3.3 MB (3266332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:a57f147526938b398a735f52fb396d6d80d70bc00a2ef5f7d081a784adb16baa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51266872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d9e1cf5a9d7e214de7b714d0ebae567113011bcbfaea2adbabb421d710cfc1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:12:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 02:12:32 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 02:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:13:00 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 02:13:04 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 02:30:23 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 02:30:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 02:30:36 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 02:30:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 02:30:43 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 02:31:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 02:31:35 GMT
CMD ["python3"]
# Sat, 04 Sep 2021 00:12:39 GMT
ENV HY_VERSION=1.0a3
# Sat, 04 Sep 2021 00:13:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 04 Sep 2021 00:13:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07dfcdf395519b72e093d262be462c85a447a9c703abfb22ce73b3fd41af24c`  
		Last Modified: Fri, 03 Sep 2021 05:11:25 GMT  
		Size: 2.9 MB (2887496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3886d0a0e0695028201150e8d99878b58caa22766dc7045f0d21e7a60bc96`  
		Last Modified: Fri, 03 Sep 2021 05:11:27 GMT  
		Size: 11.9 MB (11920368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3d2a1d9f8465ace2750084c26530fbe52de3d53d8677375d355a20cfcbd958`  
		Last Modified: Fri, 03 Sep 2021 05:11:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15c90d1c9f282c6b5a0a85c891cffb9369d021d4c19b9fedd629b3ec3afde6b`  
		Last Modified: Fri, 03 Sep 2021 05:11:25 GMT  
		Size: 2.6 MB (2638083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e112db51de1ccf50dee04a861e5cc5850f2253e03771d63269a5c2d4c71321a7`  
		Last Modified: Sat, 04 Sep 2021 00:18:59 GMT  
		Size: 3.3 MB (3267019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-rc-buster` - linux; s390x

```console
$ docker pull hylang@sha256:1a9e430227b77f983b99ecd75e617c2dab204077651957d4e0d5bbc82ad4e010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45021865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff57e3d0b0bfff3522c084c0bab821118821df62c6031a329dbece2d46916f07`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:41:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:41:05 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:41:18 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 06:41:19 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 06:48:47 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 03 Sep 2021 06:48:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 06:48:52 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 06:48:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 06:48:53 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 06:49:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 06:49:11 GMT
CMD ["python3"]
# Fri, 03 Sep 2021 22:43:21 GMT
ENV HY_VERSION=1.0a3
# Fri, 03 Sep 2021 22:43:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 03 Sep 2021 22:43:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c8139548ae7cd86e5952b530d40323a413dfb0fa9508ee8175f86cd7c9f6a`  
		Last Modified: Fri, 03 Sep 2021 08:42:53 GMT  
		Size: 2.5 MB (2459558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f79715442b9e1b47a1e3d7cfecee86f17ce8ea65faf4855a5a73916e2402687`  
		Last Modified: Fri, 03 Sep 2021 08:42:54 GMT  
		Size: 10.9 MB (10898547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce3834350e8b729ef46e7e7af2e721998a39875adb1b93a8ba98c4a1a78ba1`  
		Last Modified: Fri, 03 Sep 2021 08:42:53 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79b1135b57f8aa4a546177b83ff8d31bc4ec728edb96b5c66a7b9c26f33ba7b`  
		Last Modified: Fri, 03 Sep 2021 08:42:53 GMT  
		Size: 2.6 MB (2636613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7101d9a3e309d7a89037ba41e82f378fb9018982576f6083f9a9b86a1c1fd654`  
		Last Modified: Fri, 03 Sep 2021 22:48:57 GMT  
		Size: 3.3 MB (3266158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
