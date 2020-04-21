## `python:rc`

```console
$ docker pull python@sha256:0f6877ea0eadeaeaba49308bb8dcb61c8e657af3dafe3d6a74e4520952e7752f
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
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `python:rc` - linux; amd64

```console
$ docker pull python@sha256:0ee452e6cbef7594d7918bf30f0537080679442baf753a0961e9ac968d7c8ce6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349054898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae2295e92e65e87edd5ef8d44404ac06cde0117912a1c2c42d6c163f9b9add2`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:03 GMT
ADD file:a0c8e81c4c7fa85b43d4a9daaed7ba25964a0bf494711b6911cd4b7f5201a17f in / 
# Thu, 16 Apr 2020 03:22:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:00:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:01:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 17:54:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 17:54:41 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 18:07:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:07:35 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 16 Apr 2020 18:07:35 GMT
ENV PYTHON_VERSION=3.9.0a5
# Thu, 16 Apr 2020 18:17:09 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 16 Apr 2020 18:17:09 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 16 Apr 2020 18:17:10 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 16 Apr 2020 18:17:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 16 Apr 2020 18:17:10 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 16 Apr 2020 18:17:16 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 16 Apr 2020 18:17:16 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:7e2b2a5af8f65687add6d864d5841067e23bd435eb1a051be6fe1ea2384946b4`  
		Last Modified: Thu, 16 Apr 2020 03:31:27 GMT  
		Size: 50.4 MB (50382957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6f03ffac4cb4e42f8ab0bfc480bd3a3fa20e1ddee37784db63bc886b0cbb3`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 7.8 MB (7812113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f0c679f0f4c39597721c1df5cdb4f9685b26bd789a44eeb406835a1800d5f`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 10.0 MB (9996327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b47407fc30b8206971ec60f280b107b00df8007da2fb912ebb8656b53695e`  
		Last Modified: Thu, 16 Apr 2020 04:16:23 GMT  
		Size: 51.8 MB (51826807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32f6bf7d96d26a22dc62da6522f384dcdc936c30c88b233d378e06cf127346d`  
		Last Modified: Thu, 16 Apr 2020 04:17:13 GMT  
		Size: 192.2 MB (192169929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940e1b5707393ed528b2fce32b91fa0ba0062cc1ad382edea050e45c7a2d5b1`  
		Last Modified: Thu, 16 Apr 2020 20:47:18 GMT  
		Size: 6.1 MB (6145243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d940571110ef969a5e10c5dc0527defed5985bb2ed8dbbb595c50dfbccd6548f`  
		Last Modified: Thu, 16 Apr 2020 20:47:24 GMT  
		Size: 28.8 MB (28829957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a915c90c91d61fc8d89a62c8bdd2440971143fd38860a641705bbdea3ffe61c`  
		Last Modified: Thu, 16 Apr 2020 20:47:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d88f981c5ec9380fc3a41852c4cb5e57ddc0058b37dde1ef2561b62d88e5de4`  
		Last Modified: Thu, 16 Apr 2020 20:47:16 GMT  
		Size: 1.9 MB (1891332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm variant v5

```console
$ docker pull python@sha256:12e3e1e3fd517bd7dccf0bf1c5650b3c5db1e0885fbd22ac22144f1741af02a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.1 MB (320132877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dd1a4435e112d7b239456b60112a8e9c4c025a98d9c04880cb127cdc8c3f8b`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 00:49:45 GMT
ADD file:1daed63e84abade24fb29c2232024fa993101aafe8a874d4bef96c5635c9ce6e in / 
# Thu, 16 Apr 2020 00:49:48 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 07:41:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 07:42:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:55:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 05:48:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 05:48:44 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 05:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 05:49:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 05:49:02 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 06:00:39 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 06:00:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 06:00:45 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 06:00:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 06:00:47 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 06:00:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 06:01:00 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e139f841569e5d49ea694b0ac42568ff6f00a378e70c53d3153f77487eba09c0`  
		Last Modified: Thu, 16 Apr 2020 00:58:04 GMT  
		Size: 48.1 MB (48096823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e32d16714097e2c6a4b9e2757bc2308e1f2d411ca29c1bf91e72f5a61e587d`  
		Last Modified: Thu, 16 Apr 2020 08:05:33 GMT  
		Size: 7.4 MB (7358957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae86c403d09ed5ec0d2aac79554b33727224226a2329a81ee2ecf02c534aa5b`  
		Last Modified: Thu, 16 Apr 2020 08:05:33 GMT  
		Size: 9.7 MB (9687025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f86ab913051811dbb288b1b8149881c9dfb98b9b98dba2dbd26f6f7ccee378`  
		Last Modified: Thu, 16 Apr 2020 08:06:04 GMT  
		Size: 49.6 MB (49565578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f86a2ec0ec36cd87d1edd1ae91eeaa713dd003a983c0954226527f5f2ec3e41`  
		Last Modified: Tue, 21 Apr 2020 02:09:39 GMT  
		Size: 171.1 MB (171134550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55aafd3aae58da04b37e9ab8eb56dd34146ed2a7e9478e25ebc8f20bcff030d8`  
		Last Modified: Tue, 21 Apr 2020 07:31:15 GMT  
		Size: 5.8 MB (5840053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fcb108fb8bc0a6fff1dd0bee50aa9a463fa2cc9168669a363406683dcafde6`  
		Last Modified: Tue, 21 Apr 2020 07:31:23 GMT  
		Size: 26.6 MB (26557838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ccecb1b1e60d76cd6fa5ab2d1390a483156154a49311707b0747b38dd48fed`  
		Last Modified: Tue, 21 Apr 2020 07:31:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704495c83be4d4ee3051a6bd585b5fe37f08e3dc2fd11bc16e75d557f4ff7049`  
		Last Modified: Tue, 21 Apr 2020 07:31:14 GMT  
		Size: 1.9 MB (1891820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm variant v7

```console
$ docker pull python@sha256:b7f2ad3f3777fca09c1ced96672079d428c37c1e2c0f4288001c8807856f27be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311662628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd6612aebab88f6877ed1ca761c1a30baa3f5f91931b1147a7e9c9dd2d15ff1`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:14 GMT
ADD file:c2369e5669e570f90abaa1fd4fcea4ae1e6654bbd81e8fa070a5b2484c03ee74 in / 
# Thu, 16 Apr 2020 00:59:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:38:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:06:21 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 08:12:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 08:12:41 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 08:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 08:12:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 08:12:59 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 08:25:39 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 08:25:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 08:25:43 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 08:25:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 08:25:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 08:25:56 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 08:25:56 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:020b29c91094d59c5eb128b7bc2b0b835e2ba4414358664e467428fe8b95bf52`  
		Last Modified: Thu, 16 Apr 2020 01:08:38 GMT  
		Size: 45.9 MB (45864371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878eece65f73163f26e0755d7bf2d0280b635e9354ee5ac677dd0e1c3b9f485`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 7.1 MB (7096553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070c5585774beab3cf31d2f66df886bd4295763a00c5f013aab32f261a9559fb`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 9.3 MB (9343267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e454adb17af2402de86f3b7834eb2d85a7ab8d1199be3963a7ddf802e25a5480`  
		Last Modified: Thu, 16 Apr 2020 01:57:17 GMT  
		Size: 47.3 MB (47343806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b102b59f2834fd732b37f921e8316b384ecf42a8f1a8a0a71b315ae932cca6f`  
		Last Modified: Tue, 21 Apr 2020 01:24:18 GMT  
		Size: 168.4 MB (168386966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fd21b77c85be495f57dd18e60d53556df930dabe22273450522176b065279e`  
		Last Modified: Tue, 21 Apr 2020 10:01:12 GMT  
		Size: 5.5 MB (5535985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e051f9e4b7e28ecab6eb35c671c5c46cd55a7466ac69317be9ce88004fa0177`  
		Last Modified: Tue, 21 Apr 2020 10:01:20 GMT  
		Size: 26.2 MB (26199641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5828d575650f51910a337ce1164c4f71e885753b3345c3a209920ce3b79d88`  
		Last Modified: Tue, 21 Apr 2020 10:01:10 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd33a12db673a90f5291190bc9e4c3f40d299f5e965c87b358657af570653d9c`  
		Last Modified: Tue, 21 Apr 2020 10:01:11 GMT  
		Size: 1.9 MB (1891806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm64 variant v8

```console
$ docker pull python@sha256:78cfaa1635a230dfc9c18aece30155ca8c8ddd51582002e122276868d14b1926
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.8 MB (338759038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0caf769ec7eb9e6a4a18f1a9e32326ce0970191d60cac0ca8af46e1382e1eeaf`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:20 GMT
ADD file:02afb66e938cbc67271aaf8cbee75def87458a21d961d02e86383e0ed36b0c71 in / 
# Thu, 16 Apr 2020 02:41:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:48:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 02:11:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 02:11:41 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 08:32:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 08:32:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 08:32:12 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 08:40:34 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 08:40:38 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 08:40:39 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 08:40:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 08:40:41 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 08:40:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 08:40:53 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d080dad46627d4103daddf54c89f2ef0a0b72ba8270066c50e95ffbf4a79362e`  
		Last Modified: Thu, 16 Apr 2020 02:48:36 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c76f347939ef96b2815e45f9fa43995940a8d4a01525012b2bce1adcbfc3a`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 7.7 MB (7681332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6b37aa5fec6dcadc18e45dc6d58e4cf4b967540152c4f44030737e2f5351`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 10.0 MB (9983908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa3b2294305ed3cf1d91d1fe2e2dbf3e294a694a4f636dea6bf733975e237a`  
		Last Modified: Thu, 16 Apr 2020 03:28:16 GMT  
		Size: 52.2 MB (52155917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b47ba45af89a4c13c0c56e12431cbedfa1e0836733d37eb58461934ebca5619`  
		Last Modified: Tue, 21 Apr 2020 02:06:11 GMT  
		Size: 183.7 MB (183710129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf26ff8300b21be55f6b9681fcc3ef0acf3bea980b7edab5b4c4b2b91556b504`  
		Last Modified: Tue, 21 Apr 2020 10:06:04 GMT  
		Size: 6.3 MB (6259344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0535eb3318b929e692322cb9da9f891cec86458dbce070195a3f31bfc5853869`  
		Last Modified: Tue, 21 Apr 2020 10:06:12 GMT  
		Size: 27.9 MB (27906887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4b0992463eb041b8b8ccdc5bb46dc36b5123ca8cf283d8b1c4d5322a49157`  
		Last Modified: Tue, 21 Apr 2020 10:06:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bacfd6ad5ed5ab8463127852b776ad5136f237d255312179697fa63f3e26db0`  
		Last Modified: Tue, 21 Apr 2020 10:06:02 GMT  
		Size: 1.9 MB (1891767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; 386

```console
$ docker pull python@sha256:928c481d9a3d14ed11f47b8f068141a66badfddbfef81bc6302bf17de4583de7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.9 MB (356865344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768925be396683b4210515f34cf2a4d9789c15e1cd307165bd6e6d900f31d19b`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:37 GMT
ADD file:9a9b9c1d98dfe76e20b3ed67b866e2bdbc1095e26de13b892d07f2a3ee062c83 in / 
# Thu, 16 Apr 2020 01:39:37 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:44:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 08:23:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 08:23:24 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 09:04:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 09:04:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 09:04:50 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 09:25:09 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 09:25:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 09:25:11 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 09:25:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 09:25:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 09:25:23 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 09:25:23 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6a29df432ebf22a237e5e0940a65a1f908be66a5204c5ef240ead7315c27335f`  
		Last Modified: Thu, 16 Apr 2020 01:46:01 GMT  
		Size: 51.1 MB (51147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec62877ba52bb13d1e47ca6d0c47e1e0d1c61598a0ff5c3590b28c93b2718c3`  
		Last Modified: Thu, 16 Apr 2020 02:37:17 GMT  
		Size: 8.0 MB (7981604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab3373b511919f98b91c8b654596e531ed2f4612bf5b9d63614e0aa420ee01`  
		Last Modified: Thu, 16 Apr 2020 02:37:18 GMT  
		Size: 10.3 MB (10338497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80102fc76b236a12f5fdd11396159f29e8b9567c8c5a159b09b8dc46fc9c003`  
		Last Modified: Thu, 16 Apr 2020 02:37:39 GMT  
		Size: 53.4 MB (53423402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10121c7476fdf7e345350cb7ea5494e30098fdcde728e748932ee1cd9d534c1b`  
		Last Modified: Tue, 21 Apr 2020 01:59:03 GMT  
		Size: 198.7 MB (198713677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead0d58bce4d1cbc34d213b786b7c059ff845e621ca9cb9711148afe028f3922`  
		Last Modified: Tue, 21 Apr 2020 11:19:43 GMT  
		Size: 6.5 MB (6489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd602598be1ce2f7308fccd67d27e12c0ff8aa087192bbb8f62a46d78b2d5fd`  
		Last Modified: Tue, 21 Apr 2020 11:19:49 GMT  
		Size: 26.9 MB (26880246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a85dd2daf4fc0ee1649a09aeda0acf798c5be98953d25405ab77e5f3c3fd79`  
		Last Modified: Tue, 21 Apr 2020 11:19:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6d30cea22f73c5ef68b79deec0998ad2f012c39777462ecfd489c5a092d317`  
		Last Modified: Tue, 21 Apr 2020 11:19:41 GMT  
		Size: 1.9 MB (1891604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; mips64le

```console
$ docker pull python@sha256:8b491a9fb0b8a226e6f046eb1340037d979ed4a8005ea37dcebaafeb5c7053da
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.6 MB (333644844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a19c3a21c1e3077ded3aedf85285438862b5c1891b06c9d00fb91ae9bd7884bd`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 03:30:04 GMT
ADD file:dbf70dae7766ac8359a9b7eaeb438ecc109d3622097f3003b8520b1cabc754c6 in / 
# Thu, 16 Apr 2020 03:30:06 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:12:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:13:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:14:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:13:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 02:37:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 02:37:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 02:38:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 02:38:09 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 02:38:09 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 03:20:45 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 03:20:47 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 03:20:48 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 03:20:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 03:20:48 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 03:21:07 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 03:21:08 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6e78cab9698d138941c3838a9153c6a0bac08790291a111677e8db68f80af8f3`  
		Last Modified: Thu, 16 Apr 2020 03:56:06 GMT  
		Size: 49.0 MB (49019170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f93eb49422094c50dd707d3c5633863bc2fe34eda90dfe261f6030c88fcc1`  
		Last Modified: Thu, 16 Apr 2020 04:37:07 GMT  
		Size: 7.2 MB (7229616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eca121496b949e626e045108b6b42b000a5657dd4dd344e0e96c8823201620`  
		Last Modified: Thu, 16 Apr 2020 04:37:10 GMT  
		Size: 10.0 MB (10015772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c50efa3f9dd776e017bd4c731cc2a64b2570ef3d5f58ee935bb3483c3766d2f`  
		Last Modified: Thu, 16 Apr 2020 04:38:33 GMT  
		Size: 50.8 MB (50838609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bca0ec1c8f7fa08dfd00e45b2195764df95c90bef3913db81162fff26b7a01`  
		Last Modified: Tue, 21 Apr 2020 01:25:22 GMT  
		Size: 179.7 MB (179711592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e720c4b4a233dd9b0bcce3f1dc4d5fab4d8137bf1e269849573c2b2372e272`  
		Last Modified: Tue, 21 Apr 2020 07:39:40 GMT  
		Size: 6.5 MB (6454846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eac98bdfcb1806554bfb93b51e4d2782b39881492be89d46e4140e089a3c2d8`  
		Last Modified: Tue, 21 Apr 2020 07:40:02 GMT  
		Size: 28.5 MB (28483396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6555ff6e66247ff1e19f0a03c12ff821f082f76e85c5aba85960b9028ad8466`  
		Last Modified: Tue, 21 Apr 2020 07:39:33 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264d306103f89f005bb660c8a7b2841ec0bdc7afb6e4c04601bfef762c6476ed`  
		Last Modified: Tue, 21 Apr 2020 07:39:35 GMT  
		Size: 1.9 MB (1891608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; ppc64le

```console
$ docker pull python@sha256:5dd573e56a03fa56d3d75baf0fb06f61994825c5b18d87a83263358387447ba0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.0 MB (372003453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84a2a37e72d9ad5db455c55c76159b9109e446aff41a2eac28fe12fbb2d19c64`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 01:37:39 GMT
ADD file:5ea6b62430ec58194ba5685d0b5ecbc2df83c01b4e6c7d8b70f3e96c89390cd5 in / 
# Thu, 16 Apr 2020 01:37:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 05:40:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 05:40:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 05:42:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 02:02:14 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 03:16:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 03:16:55 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 09:21:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 09:21:04 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 09:21:06 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 09:30:19 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 09:30:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 09:30:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 09:30:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 09:30:36 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 09:30:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 09:30:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:219153a374347511566d1327acf4e45fd3425c20cd49110ef8041930fdb965a4`  
		Last Modified: Thu, 16 Apr 2020 01:53:24 GMT  
		Size: 54.1 MB (54139564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e33f6c16e453e5df771f6cd708cef378a7a3ce2d208a3cce02ff05a4015406`  
		Last Modified: Thu, 16 Apr 2020 06:20:09 GMT  
		Size: 8.3 MB (8252420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c7698edca1a58c5374b3f4a126bef6a2d822e931e0c85cd62b78199c597e72`  
		Last Modified: Thu, 16 Apr 2020 06:20:10 GMT  
		Size: 10.7 MB (10727150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a291b3427f488e71a39ecccd11fbbaf98a0e8d552444fbc7db68c1e1f16e3a`  
		Last Modified: Thu, 16 Apr 2020 06:21:11 GMT  
		Size: 57.5 MB (57452416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f83410406ceb9458a1867baed2d7041b05b7d29f66849af6dbbd249c4b5076`  
		Last Modified: Tue, 21 Apr 2020 02:49:14 GMT  
		Size: 203.0 MB (202983456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821771de12ad158bb69d75ee091871f2316fcac455dfd8c898e4d49dbcc79ef`  
		Last Modified: Tue, 21 Apr 2020 10:57:18 GMT  
		Size: 6.9 MB (6892186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe106db7c4c1fdd5923a362939f6674388ed7455c84877d31642e6d036417a4e`  
		Last Modified: Tue, 21 Apr 2020 10:57:25 GMT  
		Size: 29.7 MB (29664211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a40f8e19ae55ab61c0ec907d3fda91e1001e9c3a69924ff67f2368ca1e4052`  
		Last Modified: Tue, 21 Apr 2020 10:57:16 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7d0a346b27519d7d9eaa297701dab49ba36b5517494c3003da947bde994b8d`  
		Last Modified: Tue, 21 Apr 2020 10:57:18 GMT  
		Size: 1.9 MB (1891817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; s390x

```console
$ docker pull python@sha256:ca114e6ed2597cbb08640b9c86084c837ec77194100acc95c58dbddc173d1650
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331054719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03e99a167a8fb9c28a3d2b9d5d9afd6890d8a41c86b7adda34d4e602fe13377`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:03 GMT
ADD file:26367817216af13dc3ba9f495303f7bee8fe138fc8fb728289781563308ce0bd in / 
# Thu, 16 Apr 2020 00:42:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:58:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:45:38 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:55:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Apr 2020 01:55:40 GMT
ENV LANG=C.UTF-8
# Tue, 21 Apr 2020 07:25:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 07:25:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Apr 2020 07:25:40 GMT
ENV PYTHON_VERSION=3.9.0a5
# Tue, 21 Apr 2020 07:30:14 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 21 Apr 2020 07:30:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 21 Apr 2020 07:30:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 21 Apr 2020 07:30:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 21 Apr 2020 07:30:16 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 21 Apr 2020 07:30:21 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Apr 2020 07:30:22 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:54e2fb160a5d4a95ec7efe70c0045923ee557e87ee68ce03f2150b8366f26729`  
		Last Modified: Thu, 16 Apr 2020 00:46:03 GMT  
		Size: 49.0 MB (48960213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f0f1e0f91312a55967b48addc24054fb2e7fb63926a621dd6e86ea62aff2b4`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 7.4 MB (7382082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ce4aae52f7ba529ea00a3a1bfe7656e52dc1d8b0168a3d70b4e0a4392989f`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 9.9 MB (9882086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5250b872c2e5d6fcb26d734d43c62187b594e1ce80d34f0cf57fd5e3666b8f`  
		Last Modified: Thu, 16 Apr 2020 02:06:39 GMT  
		Size: 51.4 MB (51370893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c251493ce073cfec454cb816617c6712b99f88c1fd88a5642248e6f6b96111`  
		Last Modified: Tue, 21 Apr 2020 01:53:11 GMT  
		Size: 176.7 MB (176726730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbac423909dbf93c61e715b8c184b6b9315cb7ce61a5fc9ab79c7c8a7a4d1fd`  
		Last Modified: Tue, 21 Apr 2020 08:13:23 GMT  
		Size: 6.1 MB (6057804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd38b05a1befc066a834588833665d3576a1381db9a31b4464ee4ef546c3cd`  
		Last Modified: Tue, 21 Apr 2020 08:13:28 GMT  
		Size: 28.8 MB (28783060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c2cd49b48007b17e08d863cb0fa29610a7afac1d45c61f9bc1fd1d94fef03`  
		Last Modified: Tue, 21 Apr 2020 08:13:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840b2cf7ae27aeea43225696fd857a4bf23e11f33b17ccc2225a2bf67552659`  
		Last Modified: Tue, 21 Apr 2020 08:13:39 GMT  
		Size: 1.9 MB (1891617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - windows version 10.0.14393.3630; amd64

```console
$ docker pull python@sha256:84ddbd6daaf9301f2325800700a78c26e12a701037873306101da6b5dd2e047d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5796168241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd38806f5d33e4463bc4fe5bd6a456c4cec8112d7970cd1be67b4cf65e4702f`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:28:53 GMT
ENV PYTHON_VERSION=3.9.0a5
# Wed, 15 Apr 2020 16:28:54 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 15 Apr 2020 16:31:12 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:31:13 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 15 Apr 2020 16:31:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 15 Apr 2020 16:31:15 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 15 Apr 2020 16:32:50 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:32:51 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a493c71045f6e4812f46b85e1bf41872ddacade20f5ba83a0af530bb09e2c8b6`  
		Last Modified: Wed, 15 Apr 2020 17:26:32 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e50e78bbde1f29de6ccd3a324074d0f69265c88103c40ce9ff24cc8ebe0e7`  
		Last Modified: Wed, 15 Apr 2020 17:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e812c41d1b4ed20e6155ee195904c25b4d347343235cf03f5fff0bccdf4a4e4`  
		Last Modified: Wed, 15 Apr 2020 17:26:41 GMT  
		Size: 57.7 MB (57683674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22f1b9e01e5195374856d713b417c595d10b6b2e8366dac102b3d9ac4bf0d9a`  
		Last Modified: Wed, 15 Apr 2020 17:26:30 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05358df0d764ab2714768e516b5a8b1d955454fb83f636a09fe56d67f0cd4e5`  
		Last Modified: Wed, 15 Apr 2020 17:26:29 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a07cdf81a4f90d7bc3f76ef176672d984bce92e8e3b1fbe2acde04dacac3b7`  
		Last Modified: Wed, 15 Apr 2020 17:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a59b739f67d196ba095f28acbc3233c7b58f75dcf8bb177995afe143e66bb7c`  
		Last Modified: Wed, 15 Apr 2020 17:26:32 GMT  
		Size: 10.4 MB (10409058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83ee30b252c7e3ce9c759a6d6f92b2ce65f4e230253744dc93c49c26c30ce1e`  
		Last Modified: Wed, 15 Apr 2020 17:26:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - windows version 10.0.17763.1158; amd64

```console
$ docker pull python@sha256:57da6f1cadcd7c9493717d71f0343adf278a59df34782e88b6de0dcf0edd2a32
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328603255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5484012967e4d8b4424fc07d546caab99080b41f19b9a9e0968d244407c3e52`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:33:05 GMT
ENV PYTHON_VERSION=3.9.0a5
# Wed, 15 Apr 2020 16:33:06 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 15 Apr 2020 17:04:45 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 17:04:47 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 15 Apr 2020 17:04:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 15 Apr 2020 17:04:49 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 15 Apr 2020 17:05:31 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 17:05:32 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e412d30a806a81ca31d50673757e275ec269422cc5750e8f516cddd4669e77`  
		Last Modified: Wed, 15 Apr 2020 17:26:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c543aefcf850e4a1a779045f45b7a16afed8b9629caf8d7b54b94bf170987b0`  
		Last Modified: Wed, 15 Apr 2020 17:26:56 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0269aff770e9f46ca34db6a2cc77d2086f0074958411f028b72d86d4b58ae1a`  
		Last Modified: Wed, 15 Apr 2020 17:27:04 GMT  
		Size: 52.5 MB (52520154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5ef4db813d083320f6195bc0600d69b41847092c2d9c79b4febeed17c9aba`  
		Last Modified: Wed, 15 Apr 2020 17:26:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa9db23302a5abd7af2eed65edb2f554765746d94e35255c6128bf51171f6af`  
		Last Modified: Wed, 15 Apr 2020 17:26:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a8d12aa1844cf90f76b6b172735dd50c538d12789ef2442497e3dc1737e7ca`  
		Last Modified: Wed, 15 Apr 2020 17:26:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6af7b0b7d52590bdae05e3fdd9810f38309a2790f869078019197b3b53ef959`  
		Last Modified: Wed, 15 Apr 2020 17:26:56 GMT  
		Size: 5.4 MB (5367928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c29680cd8c339c5f67a340a55209d33e467e0cdc4782c8648034c207a0021`  
		Last Modified: Wed, 15 Apr 2020 17:26:54 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
