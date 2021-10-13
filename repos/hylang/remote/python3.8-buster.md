## `hylang:python3.8-buster`

```console
$ docker pull hylang@sha256:d45b6a2c20b79685df89cfa1fa9d433183f1ab1a6db826f1164e85af6d9044bb
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

### `hylang:python3.8-buster` - linux; amd64

```console
$ docker pull hylang@sha256:53ea0fc734a15d1e4549336ed31dbfc8a24aa9db95dbd25376f8073458070cd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46391067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0614cda1e8db555dc08eb8b745a8c39bd2f39cbac32584f2efba36d98f6e3e5e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:27:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:27:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:06:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 03:06:59 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 03:17:13 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 03:17:14 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 03:17:14 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 03:17:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 03:17:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 03:17:15 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 03:17:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 03:17:35 GMT
CMD ["python3"]
# Tue, 12 Oct 2021 17:40:44 GMT
ENV HY_VERSION=1.0a3
# Tue, 12 Oct 2021 17:40:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Oct 2021 17:40:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c44d634db0b14bf8679c170f6add62868c6df5e69e0b63c8fc3a247859d20c`  
		Last Modified: Tue, 12 Oct 2021 04:00:37 GMT  
		Size: 2.8 MB (2770140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9667f949f66d2ac5ec4830972842cd04eebbb378cc8521bafdb3961c7a2cda8d`  
		Last Modified: Tue, 12 Oct 2021 04:00:39 GMT  
		Size: 10.7 MB (10725735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f5c1d871efc0d134593e1022481d0f9c14d9d6c14102b7fa821c72781d4dc`  
		Last Modified: Tue, 12 Oct 2021 04:00:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954a1f8b4d672aada9702d3377d29af7fd5144af0361b859c5ec5e1aa317323d`  
		Last Modified: Tue, 12 Oct 2021 04:00:37 GMT  
		Size: 2.6 MB (2637177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2167827ff56149f0a5337ed0dda557d91b079cbe6ee724912a3fe1e91c6a6d0`  
		Last Modified: Tue, 12 Oct 2021 17:44:41 GMT  
		Size: 3.1 MB (3118272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:b0547f11e725ef00d315a168764ddf31eeea15e082ae6e3ec6b1ce975433afd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43482894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d84144f2afa15bdd79a5722c4e075a894550c618cb0e05ec57a26c4cd465777`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:55:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:02:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:02:10 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 04:02:10 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 04:17:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 04:17:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 04:17:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 04:17:13 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 04:17:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 04:17:14 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 04:17:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 04:17:46 GMT
CMD ["python3"]
# Tue, 12 Oct 2021 18:04:57 GMT
ENV HY_VERSION=1.0a3
# Tue, 12 Oct 2021 18:05:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Oct 2021 18:05:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226ef4dedb99b4005832955dbbe38d4da960ca0f5beaa6c289a54ba4c883bf4e`  
		Last Modified: Tue, 12 Oct 2021 05:31:49 GMT  
		Size: 2.5 MB (2460750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a7150e0917e55d1e24b47665c45a76bf726784d529b8afa4265ffcefba085`  
		Last Modified: Tue, 12 Oct 2021 05:31:55 GMT  
		Size: 10.4 MB (10393819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da0b7bd0042f7f8ac4ce86d522ebcc971d39f23574b41e6655e75532f985a82`  
		Last Modified: Tue, 12 Oct 2021 05:31:48 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f48d913fab692656225403713f5a1059a31e64e6d34229229dff65667aa06`  
		Last Modified: Tue, 12 Oct 2021 05:31:50 GMT  
		Size: 2.6 MB (2636745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e587817cc54a753d4327966ba2137dd8f4410f1c89345682fd31c785bd789b73`  
		Last Modified: Tue, 12 Oct 2021 18:10:53 GMT  
		Size: 3.1 MB (3118644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:0bd8a006db8dd75af154c86d06efae81c8c0a8186a5477504cde2d5fac5f7a32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40791037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396934b452543dc036f7833789ae6740d1eb1eced11788668dc0535c755a284c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 14:38:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 14:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:07:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:07:20 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 16:07:20 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 16:26:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 16:26:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 16:26:05 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 16:26:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 16:26:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 16:26:06 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 16:26:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 16:26:35 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 13:27:35 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 13:27:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 13:27:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f53a94afb1693ce51bceab3ba81983eb0311e1b230c67c857422abe1559baf0`  
		Last Modified: Tue, 12 Oct 2021 17:59:30 GMT  
		Size: 2.4 MB (2359017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed77bce9f0a80a2745deb1b7a27049a9a2c1800664ad16116b6df7bcb3d8da`  
		Last Modified: Tue, 12 Oct 2021 17:59:35 GMT  
		Size: 9.9 MB (9936645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9348c5224e266562cb4f5068038daa76f48fa0db93b4ca4f0bd06cc85781b125`  
		Last Modified: Tue, 12 Oct 2021 17:59:29 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cb006d86faaf3beb5ff7179181d77a750405cb806dfb6fa9b2b58bbc640418`  
		Last Modified: Tue, 12 Oct 2021 17:59:32 GMT  
		Size: 2.6 MB (2636678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac53dc1d1b01590374e4e8a2e3449ac6093ba227e71ceb7c6acef9c9fd3b5538`  
		Last Modified: Wed, 13 Oct 2021 13:37:26 GMT  
		Size: 3.1 MB (3118766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:0f7a170aec9a8a50f8cde4c833a8ae5ee56d817ea2744dc3a8e888f82cbf12ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45031849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd9142381a132ad425d8082e8bb5d5436015e335765b4099836c020e38576bd`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 14:03:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 14:03:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 14:56:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 14:56:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 14:56:11 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 15:02:21 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 15:02:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 15:02:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 15:02:22 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 15:02:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 15:02:23 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 15:02:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 15:02:35 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 16:57:00 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 16:57:05 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 16:57:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458735577bb9e6e7aca003f4898c32331ce168b4b0322fea5410a032f256c3a`  
		Last Modified: Tue, 12 Oct 2021 16:07:10 GMT  
		Size: 2.6 MB (2636435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e86fcffb8cbf29529fecb621989c7ead644078f6780d724c6ddf54634643fa`  
		Last Modified: Tue, 12 Oct 2021 16:07:11 GMT  
		Size: 10.7 MB (10732425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d99b310865df95f0cb47ad8e4005ad21d5741bc86a34d48d9ed095a495c628f`  
		Last Modified: Tue, 12 Oct 2021 16:07:09 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a32e79bcc174f0f0a5592e8bb856e0d75f3fd7ab0d2a8b32000fbccf09c44d`  
		Last Modified: Tue, 12 Oct 2021 16:07:10 GMT  
		Size: 2.6 MB (2636660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e75b22dfaab8425e279d66e23f95623af859c89f3b6a889e991168e08ef405`  
		Last Modified: Wed, 13 Oct 2021 17:04:22 GMT  
		Size: 3.1 MB (3117617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; 386

```console
$ docker pull hylang@sha256:30c69d9953301f8711579891d886c5f2156266035171f1bb37a129172d8a464f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a691a5aa8a8de64b0efc2deea9e1c684389b3652331e9faf5620728d6f186cd7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:34:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 11:34:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 13:22:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 13:22:37 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 13:22:37 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 13:36:36 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 13:36:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 13:36:37 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 13:36:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 13:36:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 13:36:38 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 13:36:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 13:36:54 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 02:28:06 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 02:28:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 02:28:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9c1102067825a5230e998a0050b5c88eb7bb9dd1ee6946a2f900e81dcad2a`  
		Last Modified: Tue, 12 Oct 2021 15:21:21 GMT  
		Size: 2.8 MB (2781591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2e80b95ec96202c7fb2795809c191bf284f24ba44104b215d4b3572d389073`  
		Last Modified: Tue, 12 Oct 2021 15:21:24 GMT  
		Size: 10.8 MB (10838940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd88e22dd24a3c622c6a217e71291699d4f6bcef74d76484e575dfe1aa625af`  
		Last Modified: Tue, 12 Oct 2021 15:21:20 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ce1b361e2cd8a31705ed1675e8002f0a36ce18a515cb49392f3ef0f91a4fcd`  
		Last Modified: Tue, 12 Oct 2021 15:21:22 GMT  
		Size: 2.6 MB (2636817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf580d2e4fc0a0c1a38caef749e9e7cbc80c976329548d9ce5071a97d5b7d30c`  
		Last Modified: Wed, 13 Oct 2021 02:36:25 GMT  
		Size: 3.1 MB (3118645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:e0d939271bc1be44941729e20a9cdbd63c4cd1fd23a469ae8287c919d5c7ec7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44502324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d437d727cfe4f1289045efefc2fc41a31a3acc9be772b43b83c3fffb26da8f8b`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:12:07 GMT
ADD file:a467fbf2015350da455cad98b5f5f247d88749cf317062ca09c466c27d53f87b in / 
# Tue, 12 Oct 2021 01:12:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:09:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 06:09:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:04:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:04:32 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 12:04:33 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 12:44:44 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 12:44:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 12:45:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 12:45:28 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 10:21:36 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 10:21:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 10:21:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4d8cdee9d607e77b6f8c2203cc9cc02b38004def2b7fe162538c1538da10c870`  
		Last Modified: Tue, 12 Oct 2021 01:21:36 GMT  
		Size: 25.8 MB (25806535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b3f0a0c95842077ac80397ca7ffcb063c0b0846dde4d6f43daf33ea110bacd`  
		Last Modified: Tue, 12 Oct 2021 17:45:19 GMT  
		Size: 2.3 MB (2321420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce905852c6e37194cc90d84c3f4eb4a434b03d27e520b4b9a4175e47328dec69`  
		Last Modified: Tue, 12 Oct 2021 17:45:25 GMT  
		Size: 10.6 MB (10619362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e34f06620c2c70873163463dd8bc04a917373393680ab59da7c9a40340574`  
		Last Modified: Tue, 12 Oct 2021 17:45:18 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b5380c000faf10eb7c6159a514481ad1412f64733b79a58002283a72c572f5`  
		Last Modified: Tue, 12 Oct 2021 17:45:21 GMT  
		Size: 2.6 MB (2636482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b449c9e03dc7101fac2ad1a7440944d25df148596c047f23681bb7b8423cdaf`  
		Last Modified: Wed, 13 Oct 2021 10:25:09 GMT  
		Size: 3.1 MB (3118292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:0d29795a5fe10c55fc9c92844f9b0564d0042df0437e9c8a8f11daa23488a14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50715243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edce3dfa960beca15cd753163efd3410fecadc64219923b09e635e2ee82070b6`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 19:50:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Oct 2021 19:50:42 GMT
ENV LANG=C.UTF-8
# Tue, 05 Oct 2021 22:07:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 22:07:54 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Oct 2021 22:07:56 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 05 Oct 2021 22:20:43 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 05 Oct 2021 22:20:52 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 05 Oct 2021 22:20:54 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 05 Oct 2021 22:20:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 07 Oct 2021 02:39:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Thu, 07 Oct 2021 02:39:26 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Thu, 07 Oct 2021 02:40:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Oct 2021 02:40:30 GMT
CMD ["python3"]
# Thu, 07 Oct 2021 03:11:11 GMT
ENV HY_VERSION=1.0a3
# Thu, 07 Oct 2021 03:11:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 07 Oct 2021 03:11:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5295f0d1dc29e70dfc0192f04d2db94d7b676632ecc260e09a41f1a8c202ed`  
		Last Modified: Wed, 06 Oct 2021 00:43:07 GMT  
		Size: 2.9 MB (2887518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d93035b2fa310819744fe3471a1b4a334bb8408e9611e57c43115274c4967a`  
		Last Modified: Wed, 06 Oct 2021 00:43:15 GMT  
		Size: 11.5 MB (11516691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c02eed51657ad14a523a63a98c6ae5ef4161a6b46346290f8ee1d9f367987e`  
		Last Modified: Wed, 06 Oct 2021 00:43:00 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec184706a0d3617d2d874eb71ad77e519170d9b863cfbab032ee82d394cf2ef0`  
		Last Modified: Thu, 07 Oct 2021 02:59:55 GMT  
		Size: 2.6 MB (2638112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b3bed386e026b96342f45ecf8f5bc5b3803a4e520d055242e6569c0effc87f`  
		Last Modified: Thu, 07 Oct 2021 03:24:09 GMT  
		Size: 3.1 MB (3118962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; s390x

```console
$ docker pull hylang@sha256:2dd87fbb9ca16254620af7be2aeb0524706ee8884be8efbde92cf8657f88c648
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44549717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd362e1a0c8db3d5830fa0f519353778ff4d524335b0a434ad4ed47390c8e9b`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 05:45:02 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:06:31 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 06:06:31 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 06:11:15 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 06:11:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 06:11:16 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 06:11:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Oct 2021 06:11:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Tue, 12 Oct 2021 06:11:17 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Tue, 12 Oct 2021 06:11:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Oct 2021 06:11:31 GMT
CMD ["python3"]
# Tue, 12 Oct 2021 10:05:49 GMT
ENV HY_VERSION=1.0a3
# Tue, 12 Oct 2021 10:05:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Oct 2021 10:05:53 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dccb8e162df86a19516f0eb41841c99a6d5ed40e271a648481d29c4deafa52a`  
		Last Modified: Tue, 12 Oct 2021 06:37:09 GMT  
		Size: 2.5 MB (2459514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e916102790c8aa6b4750948b86529a7ec4b69f1484cfd21074233c23028f62`  
		Last Modified: Tue, 12 Oct 2021 06:37:10 GMT  
		Size: 10.6 MB (10581213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef6b6676ed4f8f096df78e9c4aa1c5a694452d8a282abb830397a433639b21e`  
		Last Modified: Tue, 12 Oct 2021 06:37:09 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab69cedd6c724bb409fe3568296c7b8cbf41519df53ce3d3386734b40c4efbb`  
		Last Modified: Tue, 12 Oct 2021 06:37:09 GMT  
		Size: 2.6 MB (2636221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766bd9dc0df30c34f27b0933f23d5c1fdd076a8a154ddbd26717cd1c822db23`  
		Last Modified: Tue, 12 Oct 2021 10:10:52 GMT  
		Size: 3.1 MB (3118284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
