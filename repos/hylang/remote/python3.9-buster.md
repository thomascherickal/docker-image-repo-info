## `hylang:python3.9-buster`

```console
$ docker pull hylang@sha256:4914600eaff35da184dce8744ac1a80c7e38e22b41d8627acda6c19f6c6a9ce6
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

### `hylang:python3.9-buster` - linux; amd64

```console
$ docker pull hylang@sha256:f91fae088d7dcff2f66c4149f174ee5009bf2cd2060b2c3e744e66d004239b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46145106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4597554554c85f8378b25ad09a4abf30933d5ca43c3b496b723f4b5d4a0847b3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 09:37:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 09:37:39 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 09:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:25:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 18 Jan 2022 21:36:21 GMT
ENV PYTHON_VERSION=3.9.10
# Tue, 18 Jan 2022 21:46:06 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 18 Jan 2022 21:46:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 18 Jan 2022 21:46:08 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 18 Jan 2022 21:46:09 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 18 Jan 2022 21:46:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 18 Jan 2022 21:46:10 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 18 Jan 2022 21:46:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 18 Jan 2022 21:46:32 GMT
CMD ["python3"]
# Tue, 18 Jan 2022 22:34:41 GMT
ENV HY_VERSION=1.0a4
# Tue, 18 Jan 2022 22:34:41 GMT
ENV HYRULE_VERSION=0.1
# Tue, 18 Jan 2022 22:34:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 18 Jan 2022 22:34:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8da7e1588a5d7907234c843859e39c9897d78b1f9543d48a3462bb0567b80d1`  
		Last Modified: Tue, 21 Dec 2021 12:33:58 GMT  
		Size: 2.8 MB (2770123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13580742df49a71c088090dad37bab056bfe1dc4fae55adf997e8bb3e65b57e`  
		Last Modified: Tue, 18 Jan 2022 22:15:05 GMT  
		Size: 11.0 MB (11017436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008dd7d44d4b70963280829fb9e29059d8bb32797aa2947225074e84e917132f`  
		Last Modified: Tue, 18 Jan 2022 22:15:00 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2049aad3508dc00ed14c012cab944767a5c9591a05387b7879a86a91021b21b5`  
		Last Modified: Tue, 18 Jan 2022 22:15:00 GMT  
		Size: 2.6 MB (2637446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dca8296d03918076aa62381ae12374e7e1659b64373ede5d6c7caffda4d087a`  
		Last Modified: Tue, 18 Jan 2022 22:38:26 GMT  
		Size: 2.6 MB (2566145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:02ad445493f0e732c1071f51d7f469e419e1b8a4f1bac70b7e9082a89c255286
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43237114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b374aa825e8836f154657ffc5e251125e6c6354b8a4191c5c26447388780f2c2`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:52:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 22:52:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 22:52:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 00:06:52 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 18 Jan 2022 22:57:57 GMT
ENV PYTHON_VERSION=3.9.10
# Tue, 18 Jan 2022 23:13:46 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 18 Jan 2022 23:13:47 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 18 Jan 2022 23:13:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 18 Jan 2022 23:13:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 18 Jan 2022 23:13:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 18 Jan 2022 23:13:49 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 18 Jan 2022 23:14:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 18 Jan 2022 23:14:23 GMT
CMD ["python3"]
# Tue, 18 Jan 2022 23:42:55 GMT
ENV HY_VERSION=1.0a4
# Tue, 18 Jan 2022 23:42:56 GMT
ENV HYRULE_VERSION=0.1
# Tue, 18 Jan 2022 23:43:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 18 Jan 2022 23:43:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337031897eef93595c0a5356544adc321f2e31345e6ba782aca5652f06812fd`  
		Last Modified: Wed, 22 Dec 2021 03:33:20 GMT  
		Size: 2.5 MB (2460726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44823e4b130b1a2250b6acda58cbf4ab79c59dd6491474ccf01ca39eeef294cd`  
		Last Modified: Tue, 18 Jan 2022 23:25:07 GMT  
		Size: 10.7 MB (10686761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16b8e8811e3def83aac263ffcdef85803793ffce8108e255e6c1572343285bc`  
		Last Modified: Tue, 18 Jan 2022 23:25:00 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc8ca90104ce9a36d7c9dd0353a25775b067974126041a752c9f2e086123cb1`  
		Last Modified: Tue, 18 Jan 2022 23:25:02 GMT  
		Size: 2.6 MB (2636878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfaadda959667a71dfc4ab020f7b33224770fa5950c87b79ba7badb8bf55045`  
		Last Modified: Tue, 18 Jan 2022 23:47:04 GMT  
		Size: 2.6 MB (2566262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:ee557c418ab6548ea715a7e227b97efe30e486344d10388b78d2c809dd5e836a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40531466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bda233c08ca21e7d9218cecd1781d64b11f08387e2e8f4daf4f0bb4c19ffec7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 21:08:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 21:08:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 21:08:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:46:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 19 Jan 2022 00:37:53 GMT
ENV PYTHON_VERSION=3.9.10
# Wed, 19 Jan 2022 00:58:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 19 Jan 2022 00:58:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 19 Jan 2022 00:58:05 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 19 Jan 2022 00:58:06 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 19 Jan 2022 00:58:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 19 Jan 2022 00:58:07 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 19 Jan 2022 00:58:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 19 Jan 2022 00:58:36 GMT
CMD ["python3"]
# Wed, 19 Jan 2022 01:57:14 GMT
ENV HY_VERSION=1.0a4
# Wed, 19 Jan 2022 01:57:14 GMT
ENV HYRULE_VERSION=0.1
# Wed, 19 Jan 2022 01:57:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 19 Jan 2022 01:57:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0e1e6c3bef72f8767533cfefaae5701fec179fe73b865f393b3f4fe16fc26f`  
		Last Modified: Wed, 22 Dec 2021 03:12:51 GMT  
		Size: 2.4 MB (2359022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9377d2367c84581f979a28ac4aa7d2e6717ebf96221963aff75540ecafaa8c6e`  
		Last Modified: Wed, 19 Jan 2022 01:37:07 GMT  
		Size: 10.2 MB (10214616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2015b2df23344a93d75e7864a71285bc11d2ccaff6d5476e877bdcc8891e9a5e`  
		Last Modified: Wed, 19 Jan 2022 01:37:00 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89019178886d007f8fd90f99128bc8fc7439a36ad70b6752b57470f4b0e8c6`  
		Last Modified: Wed, 19 Jan 2022 01:37:02 GMT  
		Size: 2.6 MB (2636932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19c92a3e790f5b0ce6d791982356da805121058b00ec78d22183b7e2b534753`  
		Last Modified: Wed, 19 Jan 2022 02:05:54 GMT  
		Size: 2.6 MB (2566338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:007c8ee938c6257fc6d9be38277cecca68a50bf2f72b6f7cc36eb1ff17294f97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44574583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512d7ad503acdd1d850c624189a30ec72bf2155a528ec920aeaac425dfd17476`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 14:24:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 14:24:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 14:50:29 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 26 Jan 2022 14:50:30 GMT
ENV PYTHON_VERSION=3.9.10
# Wed, 26 Jan 2022 14:55:34 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 26 Jan 2022 14:55:35 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Jan 2022 14:55:35 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 26 Jan 2022 14:55:36 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 26 Jan 2022 14:55:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 26 Jan 2022 14:55:38 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 26 Jan 2022 14:55:56 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 14:55:56 GMT
CMD ["python3"]
# Thu, 27 Jan 2022 01:38:52 GMT
ENV HY_VERSION=1.0a4
# Thu, 27 Jan 2022 01:38:53 GMT
ENV HYRULE_VERSION=0.1
# Thu, 27 Jan 2022 01:38:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 27 Jan 2022 01:38:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662021879a6b392662e2c0f577a5ee2365d9e8a629c8e365c3f9ebe922286e4`  
		Last Modified: Wed, 26 Jan 2022 15:49:22 GMT  
		Size: 2.6 MB (2636120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5121e63a4e839c739b3c850e839d33c333c8a562a7fe119db423a812d28d3b45`  
		Last Modified: Wed, 26 Jan 2022 15:50:41 GMT  
		Size: 11.0 MB (11021743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740e0b0ee5484045b4e302a8ff9e723d32189d7c2f5e794e0b765e355d796e3c`  
		Last Modified: Wed, 26 Jan 2022 15:50:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd515de44203e7dd86a59c9f6a23df484349d7dd6b50f3080fbea4b1a67ceb`  
		Last Modified: Wed, 26 Jan 2022 15:50:40 GMT  
		Size: 2.4 MB (2427129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c6e4346c8f985050c6a2fd1efaf7af889d46cb740f6f0aab0c719f7ce3a7b6`  
		Last Modified: Thu, 27 Jan 2022 01:44:21 GMT  
		Size: 2.6 MB (2566142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; 386

```console
$ docker pull hylang@sha256:5a292daf712523665184c8f360c1d49ebba216ab445fb59c9319ab2ad5410bae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46938147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b06058e30b8083ac69c6aae15cad644f8435bcb87e283c525ae744867db15dc`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:30 GMT
ADD file:0d3811120feb1258b2cbe48be0a91ae3389643fb759b10b83b6534ebca8cf795 in / 
# Wed, 26 Jan 2022 01:40:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 23:29:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 23:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 23:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:34:43 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 27 Jan 2022 00:34:43 GMT
ENV PYTHON_VERSION=3.9.10
# Thu, 27 Jan 2022 00:46:45 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 27 Jan 2022 00:46:47 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 27 Jan 2022 00:46:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Thu, 27 Jan 2022 00:46:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 27 Jan 2022 00:46:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Thu, 27 Jan 2022 00:46:48 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Thu, 27 Jan 2022 00:47:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 27 Jan 2022 00:47:03 GMT
CMD ["python3"]
# Thu, 27 Jan 2022 12:26:24 GMT
ENV HY_VERSION=1.0a4
# Thu, 27 Jan 2022 12:26:24 GMT
ENV HYRULE_VERSION=0.1
# Thu, 27 Jan 2022 12:26:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 27 Jan 2022 12:26:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:79e14f2e0ab2370ab81617ee0b4757c6c2e55d326ad5c7b5290a5068e50176df`  
		Last Modified: Wed, 26 Jan 2022 01:50:05 GMT  
		Size: 27.8 MB (27804600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94be7423a6ca096fc8be00439e285a77274cbc1c2bff0e9b798cbb44c735b4a2`  
		Last Modified: Thu, 27 Jan 2022 02:21:23 GMT  
		Size: 2.8 MB (2781577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0123e1e30bbdf536c69522b29269d21eb8957b3d1401db241f4fbf78f044467a`  
		Last Modified: Thu, 27 Jan 2022 02:23:12 GMT  
		Size: 11.1 MB (11148621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e06403e1d28bfbf2d8a4b6681abfeb46e21cc26c445a4c1d45dbf9d10e9575`  
		Last Modified: Thu, 27 Jan 2022 02:23:09 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82c231c979caf0e01839bdb68309258eab12ce6675f7fe7ced4ad1d88d4add`  
		Last Modified: Thu, 27 Jan 2022 02:23:09 GMT  
		Size: 2.6 MB (2636962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cb8b3bc84a8444c9ddbd0e498085821c33e4468f80003c6dfbcf7a62e1dea3`  
		Last Modified: Thu, 27 Jan 2022 12:32:53 GMT  
		Size: 2.6 MB (2566152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:6510ca970f5a10697afdc76ce2a2ba3bb39408d01141797482f48815a0e3ec7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44251114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab1219f1a1c216952620d609ec20cd130f8e6d9cb4fb6bfdc548ffa1df0616`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:59 GMT
ADD file:1e736cd218a1aa1d9d52dfb824407b84a8d10720ee840b3d81cdf74df62b74b8 in / 
# Tue, 21 Dec 2021 02:10:00 GMT
CMD ["bash"]
# Wed, 22 Dec 2021 07:01:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 07:01:53 GMT
ENV LANG=C.UTF-8
# Wed, 22 Dec 2021 07:02:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 10:25:00 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 19 Jan 2022 03:16:21 GMT
ENV PYTHON_VERSION=3.9.10
# Wed, 19 Jan 2022 03:58:55 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 19 Jan 2022 03:58:57 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 19 Jan 2022 03:58:57 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 19 Jan 2022 03:58:57 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 19 Jan 2022 03:58:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 19 Jan 2022 03:58:58 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 19 Jan 2022 03:59:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 19 Jan 2022 03:59:44 GMT
CMD ["python3"]
# Thu, 20 Jan 2022 19:11:05 GMT
ENV HY_VERSION=1.0a4
# Thu, 20 Jan 2022 19:11:05 GMT
ENV HYRULE_VERSION=0.1
# Thu, 20 Jan 2022 19:11:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 20 Jan 2022 19:11:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4425ebd1b1a185b87251c0eb43ab9b16b24ec96090a67323f44e2365b8f9bc19`  
		Last Modified: Tue, 21 Dec 2021 02:19:49 GMT  
		Size: 25.8 MB (25820202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44666251dc312e864969850998f8fc89d9e4212d4b80633c56363a6798db74c9`  
		Last Modified: Wed, 22 Dec 2021 18:55:10 GMT  
		Size: 2.3 MB (2321415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d00b3f8c92249d3955854d96c2e38a8e738eeda7af3ce0ab2e462b64c8ba544`  
		Last Modified: Wed, 19 Jan 2022 04:04:39 GMT  
		Size: 10.9 MB (10906293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa26f016e453d661e9ae7c468812616538561bf1ddc8afbaa3ed74219ab20858`  
		Last Modified: Wed, 19 Jan 2022 04:04:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b8b855e1d37d4d38f3ac9f97ec767cc02366d636b40d0d53a7d3154d11dc01`  
		Last Modified: Wed, 19 Jan 2022 04:04:34 GMT  
		Size: 2.6 MB (2636700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0195ca436c7d64cd4223d5c67bf16f606c3217b56e21f26d6fcb576b1c67b62a`  
		Last Modified: Thu, 20 Jan 2022 19:12:10 GMT  
		Size: 2.6 MB (2566271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:9e361481b4a6e9805cdfd9a5f7d16db52ce58b3480c23b9cb0e312e0ebfbd183
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50497206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d67a45869c1688bd1759d735b98b2e06658aeb9b821889feed4aff21b55a30b7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:21:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 12:21:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 12:21:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:16:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 18 Jan 2022 22:44:13 GMT
ENV PYTHON_VERSION=3.9.10
# Tue, 18 Jan 2022 22:59:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 18 Jan 2022 22:59:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 18 Jan 2022 22:59:19 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 18 Jan 2022 22:59:21 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 18 Jan 2022 22:59:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 18 Jan 2022 22:59:28 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 18 Jan 2022 23:00:06 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 18 Jan 2022 23:00:08 GMT
CMD ["python3"]
# Tue, 18 Jan 2022 23:47:31 GMT
ENV HY_VERSION=1.0a4
# Tue, 18 Jan 2022 23:47:36 GMT
ENV HYRULE_VERSION=0.1
# Tue, 18 Jan 2022 23:47:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 18 Jan 2022 23:48:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e283dbbadf653766a6a4005b913bd987dd24aa0f51e82933548f75fffc420`  
		Last Modified: Tue, 21 Dec 2021 16:01:53 GMT  
		Size: 2.9 MB (2887523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63d51372d221db5a3f27ec467d0a4fe68a597cb4ac9c4ae1d47e4903ab3366b`  
		Last Modified: Tue, 18 Jan 2022 23:27:42 GMT  
		Size: 11.8 MB (11842393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9977bd55b045844d223a589346d37593862eb71388d992b13a9eb9511f9434cb`  
		Last Modified: Tue, 18 Jan 2022 23:27:40 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d1dc20f96d38ac2fce5001081841ff51c7406515e381adfd86f19dadaac068`  
		Last Modified: Tue, 18 Jan 2022 23:27:41 GMT  
		Size: 2.6 MB (2638445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145f60462e4898faccf4a75fc8503901e255d8d5b31340d19ad0df240edfc820`  
		Last Modified: Tue, 18 Jan 2022 23:53:39 GMT  
		Size: 2.6 MB (2566300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; s390x

```console
$ docker pull hylang@sha256:8d171964e774e2aea75e9419d6dc09aae16567535a143ffc5efc1a15f145c048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44292364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1422c5efb52af1d37b6d01d93ad9f926684e62652ccc4cad70983548a9a3dd15`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:43 GMT
ADD file:27d2ddf8a67fd6bce8ec2eb1a83419b88265bc9b1640c3055d6b36b44586b03a in / 
# Wed, 26 Jan 2022 01:41:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:15:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:15:40 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:15:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:42:10 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 26 Jan 2022 09:42:11 GMT
ENV PYTHON_VERSION=3.9.10
# Wed, 26 Jan 2022 09:47:50 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 26 Jan 2022 09:47:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Jan 2022 09:47:51 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 26 Jan 2022 09:47:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 26 Jan 2022 09:47:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 26 Jan 2022 09:47:52 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 26 Jan 2022 09:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 09:48:06 GMT
CMD ["python3"]
# Wed, 26 Jan 2022 22:43:14 GMT
ENV HY_VERSION=1.0a4
# Wed, 26 Jan 2022 22:43:14 GMT
ENV HYRULE_VERSION=0.1
# Wed, 26 Jan 2022 22:43:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 26 Jan 2022 22:43:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:72d32cf8184f85de685e3d4f0354385b1ef6ed1ff7ce95a31b81ad20d6ae77c1`  
		Last Modified: Wed, 26 Jan 2022 01:47:30 GMT  
		Size: 25.8 MB (25769120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea15bd8750c2ec913d47657298933780e595d88435637e349f67c18067098ee`  
		Last Modified: Wed, 26 Jan 2022 10:34:41 GMT  
		Size: 2.5 MB (2459510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7cc5c3eaad8bf8d907ced240b25aad7a17558aad4ad78bbdcd9ebbc3083745`  
		Last Modified: Wed, 26 Jan 2022 10:35:40 GMT  
		Size: 10.9 MB (10860805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ae8c1aca38ab39ce7b272711a5c105e15d59bb717a053d994596e1e53728d`  
		Last Modified: Wed, 26 Jan 2022 10:35:38 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822d993ed9df8590ad0232f9618d1ee7dad538db8b9a232d79ecb01de44babad`  
		Last Modified: Wed, 26 Jan 2022 10:35:39 GMT  
		Size: 2.6 MB (2636606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592b818f0194f22acf2fa644d0add980bb5dfd50b6364889de4cf2ce4a05efa2`  
		Last Modified: Wed, 26 Jan 2022 22:47:51 GMT  
		Size: 2.6 MB (2566091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
