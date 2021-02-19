## `python:latest`

```console
$ docker pull python@sha256:5c23b2b14f58364221442deddba3f0bb81c56165f9ce5864d215438edc82df12
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
	-	windows version 10.0.17763.1757; amd64

### `python:latest` - linux; amd64

```console
$ docker pull python@sha256:2a7e1b9e632b7a3a967dbddbf8c80fff234f10f9cb647b253c6405252db41c9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339818571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a93c239d591553ed9c25ef20ed7c7a1542e8644f57d352e3a1446f0a5f0412d`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:37:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:12:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:12:23 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 07:12:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:32:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 07:32:51 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 07:43:34 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 07:43:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 07:43:37 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 07:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 07:43:37 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 07:43:50 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 07:43:50 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a0f46f8c38f4ca7daecf160ba9cdb3ddeafda769e2741e179851cfaa14eec`  
		Last Modified: Tue, 09 Feb 2021 04:46:23 GMT  
		Size: 51.8 MB (51830963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937782447ff61abe49fd83ca9e3bdea338c1ae1d53278b2f31eca18ab4366a1e`  
		Last Modified: Tue, 09 Feb 2021 04:47:13 GMT  
		Size: 192.3 MB (192328407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b7aaaab2cfb7598d50ad36633611a75bff6116d6a0acc2d37df61b5c797be`  
		Last Modified: Tue, 09 Feb 2021 09:51:01 GMT  
		Size: 6.1 MB (6145524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c4d8634a1a306e07412154f682d30988cee9a788c10563e0143279d23fa69b`  
		Last Modified: Tue, 09 Feb 2021 09:51:33 GMT  
		Size: 19.1 MB (19122077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b6aa65d161c7afc7d1b5741224751f55ea238144036e416037b02e22d73dff`  
		Last Modified: Tue, 09 Feb 2021 09:51:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fc0748308d6904bfdd5e91721ba058abdd1a415247a65089b44392f4be9fc9`  
		Last Modified: Tue, 09 Feb 2021 09:51:28 GMT  
		Size: 2.2 MB (2164028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm variant v5

```console
$ docker pull python@sha256:b597a38b382dee4151cb0f56d8e59ee79def2d5d38d9b41a0276043d0e19984f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312302426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70f3049d8b4c08997cb3f5070dadea4f082d9f0b749a64d56cba2d609a88a2d`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:49:48 GMT
ADD file:0d42654e4fb3d6743aca1ff6ed0c1438b6af430c0e32f32a645a069650192ba8 in / 
# Tue, 09 Feb 2021 02:49:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:25:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:29:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:22:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 04:22:27 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 04:22:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:50:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 19 Feb 2021 17:02:37 GMT
ENV PYTHON_VERSION=3.9.2
# Fri, 19 Feb 2021 17:15:05 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 19 Feb 2021 17:15:09 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 19 Feb 2021 17:15:10 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Fri, 19 Feb 2021 17:15:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Fri, 19 Feb 2021 17:15:12 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Fri, 19 Feb 2021 17:15:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 19 Feb 2021 17:15:29 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:caefd74d211732bd2d8529a8957297fee583b1eed876add26edaae597ec7eeb3`  
		Last Modified: Tue, 09 Feb 2021 02:58:42 GMT  
		Size: 48.1 MB (48111499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a124d5143cc689eb683e6266a65032891dfe62eeb6cb6b509b97db15c76b32c`  
		Last Modified: Tue, 09 Feb 2021 03:40:13 GMT  
		Size: 7.4 MB (7376268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa139a8bae24b22edced2ecd5c232ad41726a2d3c7735379b893172896d68f7`  
		Last Modified: Tue, 09 Feb 2021 03:40:14 GMT  
		Size: 9.7 MB (9687544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acd73801003dec84d303d6956df994b26ab304d99a457d6b1bd1c70427b5852`  
		Last Modified: Tue, 09 Feb 2021 03:40:39 GMT  
		Size: 49.6 MB (49571258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2cfcf4c167befe0465ffcaf03d11ab2a43a477abef9c4a4c4d01db2cd7b6f`  
		Last Modified: Tue, 09 Feb 2021 03:41:40 GMT  
		Size: 171.3 MB (171288803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28c1eeaee0acb2da6e8bcf5fad4cff2c30930fb79375bc747388670406c0421`  
		Last Modified: Tue, 09 Feb 2021 07:08:51 GMT  
		Size: 5.8 MB (5840429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0046d9139978d706f10e136ae533f6dc1bb9aaae90bdf45694dd32a11554a03`  
		Last Modified: Fri, 19 Feb 2021 17:58:03 GMT  
		Size: 18.3 MB (18262134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5f1ad0b800763934c30b4be7ab73a8ec5513d8ee402257e1f3c1ea2579e9cd`  
		Last Modified: Fri, 19 Feb 2021 17:57:57 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be5b61645a56fcd0d0c9c12c520226e4ccc0e9c9c8fc4a720fc39836cdddfb6`  
		Last Modified: Fri, 19 Feb 2021 17:57:58 GMT  
		Size: 2.2 MB (2164258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm variant v7

```console
$ docker pull python@sha256:07b38010ab951410de525e8671317aca28a507df3e272d451cc2a195e250783f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303929261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb637885a9aa52b3fa370a39850672d43a424b51a1db312f08df7624138c0f8d`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:29 GMT
ADD file:817a4ff41fcac0be44e95d3f0a51c9fa878d16dac7cdab68bfc445f630c43c22 in / 
# Tue, 09 Feb 2021 03:00:33 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:26:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:26:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:28:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 13:07:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 13:07:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 13:08:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 13:35:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 13:35:46 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 13:48:38 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 13:48:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 13:48:42 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 13:48:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 13:48:43 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 13:48:57 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 13:48:58 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:4c2a0a79594a20b9c2f0bfbd535f875ca1b079625052cdd801afb1cc0362d6d0`  
		Last Modified: Tue, 09 Feb 2021 03:09:18 GMT  
		Size: 45.9 MB (45867053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c11c595f6421f88e1b10286a766ae8db88f67c2c0f41cedd170640aee498ab`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 7.1 MB (7123173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cb22b679409f00e04b8d645444df7181f05cb2967ed73f1a377e7f774b6873`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 9.3 MB (9343495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e90d4e143c069feee70f90eea83d55b7b0761c67fbbfb7f3734c16c0811ac13`  
		Last Modified: Tue, 09 Feb 2021 04:40:02 GMT  
		Size: 47.4 MB (47355624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7064acb6373ca1f0f12ecbbace9c16a2f741e61286783b17096d3db440b91c`  
		Last Modified: Tue, 09 Feb 2021 04:40:59 GMT  
		Size: 168.5 MB (168545440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df02116face90b959309647c1079aba91692478f29e5d94d8273fd09a2d5b81`  
		Last Modified: Tue, 09 Feb 2021 16:11:06 GMT  
		Size: 5.5 MB (5536302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f15eeab06f046953509e9366c81dcfe1b0d3e3f5527564050ce66b511abf58b`  
		Last Modified: Tue, 09 Feb 2021 16:11:47 GMT  
		Size: 18.0 MB (17993718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae41b23ae0a27ecbee0b9ad655af3d242930253f890e9ca41a15b8d8981c08b8`  
		Last Modified: Tue, 09 Feb 2021 16:11:41 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8802bcdaf5e78a9dd8e1970f4bc1a884bed67846405297d6f171975f415b2cd`  
		Last Modified: Tue, 09 Feb 2021 16:11:42 GMT  
		Size: 2.2 MB (2164224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm64 variant v8

```console
$ docker pull python@sha256:3cb0ab4a815457fb78fb84a41c66981420aaee5d06726859b77d250b65c1e990
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329931884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbd49098d8eebfdb20ed5a074e0af80951e13ec88f68cf06230462fa9101110`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:46:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 14:57:29 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 14:57:30 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 14:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 15:17:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 15:17:54 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 15:26:40 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 15:26:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 15:26:44 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 15:26:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 15:26:46 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 15:26:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 15:27:00 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb44d26a138a8d064a4ab8f9b472c64e7136c2482ec5af19bab8811b6d2c15b7`  
		Last Modified: Tue, 09 Feb 2021 04:57:46 GMT  
		Size: 52.2 MB (52165287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195488cfc78f0e257698fa052494b5340338b5acfdec4df1b249942044222274`  
		Last Modified: Tue, 09 Feb 2021 04:58:39 GMT  
		Size: 183.9 MB (183888365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91064730500746be97b6f35ae9c33bf1d9b7b0b4e9fd5f766c84ff08d25502b`  
		Last Modified: Tue, 09 Feb 2021 17:26:59 GMT  
		Size: 6.3 MB (6259602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88c09aad7fe916f528741afa2a4072f4b8514725f54c9a9e3b0d8e38d7cf98d`  
		Last Modified: Tue, 09 Feb 2021 17:27:47 GMT  
		Size: 18.6 MB (18592470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c492206888c962a8cd02d08cdbdc962f2a10b7e2373d1aca6ac94a817ca309c`  
		Last Modified: Tue, 09 Feb 2021 17:27:42 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ebfb02ddcff9e4c8d2b993f909b47b7141ba9fb8aa2719d96e6279e865f713`  
		Last Modified: Tue, 09 Feb 2021 17:27:42 GMT  
		Size: 2.2 MB (2164296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; 386

```console
$ docker pull python@sha256:24d51c588d4ace982c923ce4269eb5fe2a3887904028c91c1af239b8654dba72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.9 MB (348884277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45377dd8afb28ec5523f13073fb458902fdeb19e65cf02eb0adf76fa16e9f29f`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:32 GMT
ADD file:174c1471a32619d54d725ea84d52c784b0093e0fa3327988de11aa4c7a1a74f8 in / 
# Tue, 09 Feb 2021 02:39:32 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:09:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:10:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:11:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 15:14:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 15:14:08 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 15:14:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 15:50:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 15:50:11 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 16:07:29 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 16:07:31 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 16:07:31 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 16:07:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 16:07:32 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 16:07:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 16:07:47 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ddc66558221fdd621c8a9a9b10318a2be0e73e6e9b5201713c51d24dc672e99f`  
		Last Modified: Tue, 09 Feb 2021 02:45:29 GMT  
		Size: 51.2 MB (51163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3367f7dc54e20f15e3eb446308d1d90921807cbbbe026653f1e081e0f3f800d4`  
		Last Modified: Tue, 09 Feb 2021 03:20:37 GMT  
		Size: 8.0 MB (7996266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d8d6b6155811224781274d8019eebe0788d1437193d1cc61be4e579108dd74`  
		Last Modified: Tue, 09 Feb 2021 03:20:37 GMT  
		Size: 10.3 MB (10338853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d650a4bdf99a8c28d0ec7f0b518cd93231802ba93726fa384a15c5ea536a87b`  
		Last Modified: Tue, 09 Feb 2021 03:21:05 GMT  
		Size: 53.4 MB (53433487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1edc34ad398b012dca57207b4b1f686bd58ddc8e58d310af2a4ed94c733a8f`  
		Last Modified: Tue, 09 Feb 2021 03:22:29 GMT  
		Size: 198.9 MB (198875043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1195ced9c28baa322763ce881b94483f9a1cbedaeed937d15398a3c8ee86a9`  
		Last Modified: Tue, 09 Feb 2021 18:29:43 GMT  
		Size: 6.5 MB (6489554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e15bb53062bc973912faebdd0d0432b28a283017d197f8a5d62d549eaa471`  
		Last Modified: Tue, 09 Feb 2021 18:30:18 GMT  
		Size: 18.4 MB (18423542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78248f4ec382c3987b3ceee4edcec2a6067e2fc51e1190074de791a5e89888a9`  
		Last Modified: Tue, 09 Feb 2021 18:30:12 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007ce42e9cbbbc710bce0bc1bfb40296f29c2235ddbfa9ea513c8aeed7597706`  
		Last Modified: Tue, 09 Feb 2021 18:30:13 GMT  
		Size: 2.2 MB (2164128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; mips64le

```console
$ docker pull python@sha256:a24c87629656a91c72609cc543a1f6088a34c9f286e4e8c5414c1775bbef03aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.4 MB (324351588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b98749dbcb692ca133a2f4195905a35978facb07b845e4873d0e4d7de89bcb6`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:04 GMT
ADD file:490a48a20d3dd7f37fb99df67136dba1fd328a9916a73fbc13da9be27e7fd95d in / 
# Tue, 09 Feb 2021 03:09:04 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:05:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:05:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:06:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:08:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:48:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:48:24 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 09:48:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:12:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 11:12:47 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 11:53:34 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 11:53:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 11:53:36 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 11:53:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 11:53:37 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 11:53:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 11:53:59 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c66db2c7cd9b921e61702131302689efe48861f2def6b11e1d3ebe56fc06fdad`  
		Last Modified: Tue, 09 Feb 2021 03:15:07 GMT  
		Size: 49.0 MB (49027959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4558012499a65e8af9c0d92bfddea26b0adc56b688f78ce2c33bb72ff0e24b3`  
		Last Modified: Tue, 09 Feb 2021 04:16:37 GMT  
		Size: 7.3 MB (7250591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c64a7693227b692aae0c22e05c8c9b808f4d4ddf20575237a1fec0a0c8fba8d`  
		Last Modified: Tue, 09 Feb 2021 04:16:38 GMT  
		Size: 10.0 MB (10016352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9f01a8e276f4df19d07d9706dc3b0dec6edc61799fcc5f3270e0514fe6c29c`  
		Last Modified: Tue, 09 Feb 2021 04:17:30 GMT  
		Size: 50.8 MB (50843339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f814d99f843c120f6d7158646910bb2eae4df6b5b6c806b793e6dd3900827`  
		Last Modified: Tue, 09 Feb 2021 04:19:42 GMT  
		Size: 179.8 MB (179837581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1745c20745584ce2d3f9facdffad4c1bde5641fa3b852ccad39b53db40d29776`  
		Last Modified: Tue, 09 Feb 2021 16:18:17 GMT  
		Size: 6.5 MB (6455225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58388a547fbfa96d2e51915f66290804ec9c9c2515ba2bbd91b998e098b8bae5`  
		Last Modified: Tue, 09 Feb 2021 16:19:33 GMT  
		Size: 18.8 MB (18756194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed1b7d97d33f34188f38133f41ed398c77ba1cffb8591ff217ec63a07a65d2`  
		Last Modified: Tue, 09 Feb 2021 16:19:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4139614ff5055b6293231707a4cbe8d3523c80f79ba8d135bd0c36f4f5d1493f`  
		Last Modified: Tue, 09 Feb 2021 16:19:21 GMT  
		Size: 2.2 MB (2164116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; ppc64le

```console
$ docker pull python@sha256:e0fa82d9ce228c9c185d22a60027a8f1f067344162338ac106b90d42345c6901
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362449047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf13f5d315b620581351f7bd7b27809109c96cbeb2b8789207a39110d2dac29a`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:18:34 GMT
ADD file:0fc1572a1f7f423ae98036bea9f9d1f9237ea74bf582a925ecf956383f7dc8e1 in / 
# Tue, 09 Feb 2021 02:18:46 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:03:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 05:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:22:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:22:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 18:22:17 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 18:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 19:08:33 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 09 Feb 2021 19:08:45 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 09 Feb 2021 19:18:48 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 09 Feb 2021 19:19:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 09 Feb 2021 19:19:12 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Tue, 09 Feb 2021 19:19:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Tue, 09 Feb 2021 19:19:28 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Tue, 09 Feb 2021 19:20:02 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 09 Feb 2021 19:20:13 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:9311932ee2fcc8fed8d2911fda20f73ee92ea26879166cf6cc3192522e83fd0a`  
		Last Modified: Tue, 09 Feb 2021 02:27:25 GMT  
		Size: 54.1 MB (54135809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881ebf746bce396a8b31a683ca6cbcb81f5c9aa7bb2c9e236996aa2c7b5610d5`  
		Last Modified: Tue, 09 Feb 2021 05:48:15 GMT  
		Size: 8.3 MB (8271305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27336f6700d8773d71eb0faf6090217770cffe60d1132c3d46f5375639b8a2e9`  
		Last Modified: Tue, 09 Feb 2021 05:48:16 GMT  
		Size: 10.7 MB (10727781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afedf8a01deada06218528a166adc4366030e683f7c3442f16812ece04158aa`  
		Last Modified: Tue, 09 Feb 2021 05:48:41 GMT  
		Size: 57.5 MB (57455475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2317e35552d5e6d953cd88b1a7cc311db6ba2358abb26bf0a222fc60393503`  
		Last Modified: Tue, 09 Feb 2021 05:49:45 GMT  
		Size: 203.2 MB (203178937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f361e4de9c4a6ac16897454d2fea6023fafae2f0dc9e959ab5089e9dd3f116c1`  
		Last Modified: Tue, 09 Feb 2021 21:44:18 GMT  
		Size: 6.9 MB (6893019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97143409176fdaee32dfe969e276fd3cd76ace7075825b0e338d40927c3533b7`  
		Last Modified: Tue, 09 Feb 2021 21:45:08 GMT  
		Size: 19.6 MB (19622166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbeaaf7dff6f38833c661a14c31f09edb7afcd1de39281acffb51dec08b214e`  
		Last Modified: Tue, 09 Feb 2021 21:45:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e543a51bb4d79c4f2b73ebb3eec2475c589b48d28eb53ecabf642a582c4aba07`  
		Last Modified: Tue, 09 Feb 2021 21:45:04 GMT  
		Size: 2.2 MB (2164322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; s390x

```console
$ docker pull python@sha256:8fcf2c2dcd16d65872b108fd21aebc079c56a22d3a4ac5251b1de7be5c58804b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321547069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f19d19dbef7ec445798940855aed88352e7dccf3aed62c7f129a64a9ccb5f29`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:56 GMT
ADD file:f390b371893461fffed2fb48d65b6c930137539a82b9c5329410cef322a5a9ea in / 
# Tue, 09 Feb 2021 02:41:59 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:05:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:05:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:05:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:06:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:34:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:34:47 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:34:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:45:22 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 19 Feb 2021 17:02:15 GMT
ENV PYTHON_VERSION=3.9.2
# Fri, 19 Feb 2021 17:07:42 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 19 Feb 2021 17:07:43 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 19 Feb 2021 17:07:44 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Fri, 19 Feb 2021 17:07:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Fri, 19 Feb 2021 17:07:44 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Fri, 19 Feb 2021 17:07:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 19 Feb 2021 17:07:51 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:fb61e252baf0cdce361b288d8df47eab4b2adb45935d61331700aa9281372c74`  
		Last Modified: Tue, 09 Feb 2021 02:45:12 GMT  
		Size: 49.0 MB (48970386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21893889b63220b2786e70a7182ba39dfc2fffcecd394424c4be2eba9d090798`  
		Last Modified: Tue, 09 Feb 2021 03:11:48 GMT  
		Size: 7.4 MB (7399445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadc5e0216d8dc7f2fc17b19146d9e168fadadf4acf3bfee694853596f8ee659`  
		Last Modified: Tue, 09 Feb 2021 03:11:47 GMT  
		Size: 9.9 MB (9883127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c25bdb77d50c2365abbf0b825665a3320edce80f9ee8ce5985b29effa66c21`  
		Last Modified: Tue, 09 Feb 2021 03:12:03 GMT  
		Size: 51.4 MB (51379480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93feec1083c1d250480d7067cac7e1e517fdf9a3932367d21c7e0a31c5a0a77`  
		Last Modified: Tue, 09 Feb 2021 03:12:32 GMT  
		Size: 176.8 MB (176847767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d60a4b0616ec2c567dd5db1329dd29ad9dc35b03546a64ab58d04dd775a96f`  
		Last Modified: Tue, 09 Feb 2021 07:28:56 GMT  
		Size: 6.1 MB (6058246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cdeed492774c621699ba9ab1d5d8f7c461a0c3e72d381413faa50b3278a57`  
		Last Modified: Fri, 19 Feb 2021 17:47:45 GMT  
		Size: 18.8 MB (18844295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978ec4770cc832085225606bc44570e6aff61b9006b78102dbcd45910113fa44`  
		Last Modified: Fri, 19 Feb 2021 17:47:42 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f522b1bce48b00504e97ddd607e424e7a8657e1b4a63c26b8e7ffbaec7ca3821`  
		Last Modified: Fri, 19 Feb 2021 17:47:42 GMT  
		Size: 2.2 MB (2164091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull python@sha256:2303af134f2df44ef20e686d9215499cd8618c65f00058c820123e20ee0f6873
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2508586559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab79abded34a3c9b3341ee99db5de99ccde38ad3d728d06eefa527623c7bdc5b`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 16:07:47 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 19 Feb 2021 17:07:55 GMT
ENV PYTHON_VERSION=3.9.2
# Fri, 19 Feb 2021 17:07:56 GMT
ENV PYTHON_RELEASE=3.9.2
# Fri, 19 Feb 2021 17:09:35 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 19 Feb 2021 17:09:37 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Fri, 19 Feb 2021 17:09:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Fri, 19 Feb 2021 17:09:39 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Fri, 19 Feb 2021 17:10:32 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 19 Feb 2021 17:10:34 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b84e06535ce9db874df389992b93e0bd5a992e8067ba9fc73059f40ef8966dd`  
		Last Modified: Wed, 10 Feb 2021 16:34:31 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24772355d3c3d70048c28dd692c7805143451bb923d9a2c3bbfda8a55984a084`  
		Last Modified: Fri, 19 Feb 2021 17:22:56 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53dfbec8592b7551f09d4304078d7711487d12fbca13c22f6373fddec3518e`  
		Last Modified: Fri, 19 Feb 2021 17:22:56 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde426e380aca6ed7a2323366a3c2b4d00c53e1ffc9c4c6b619cb92acb1af0d`  
		Last Modified: Fri, 19 Feb 2021 17:24:06 GMT  
		Size: 59.0 MB (59012403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50351ac87fbf15ed0fb8b2c59d4911aecf3271b1f5c2b4fa041db7d9de346664`  
		Last Modified: Fri, 19 Feb 2021 17:22:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd3e7708fcdd3013e9a80f70facdfdefe46bf0ba2483b07978d96f61a9ed593`  
		Last Modified: Fri, 19 Feb 2021 17:22:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0594574028c731dade4c10ddba212aaa13d7a8decbb2917be44ea2089e3fc83e`  
		Last Modified: Fri, 19 Feb 2021 17:22:53 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812f7693e1abb0930fe7fce7dfb98ba9fc0e40e152c0bac853fb1d257f26cf54`  
		Last Modified: Fri, 19 Feb 2021 17:22:56 GMT  
		Size: 10.3 MB (10296102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f28efab335bd56a656e740762a09fcc14c648cb22fc9b27e585990d7abe638e`  
		Last Modified: Fri, 19 Feb 2021 17:22:53 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
