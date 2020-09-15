## `python:rc-buster`

```console
$ docker pull python@sha256:e71d513cb5c881e91abd5cb1b1d56a9ea9e93e9ff9ad65b74d8732df0b353687
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

### `python:rc-buster` - linux; amd64

```console
$ docker pull python@sha256:3b04a5341b50ed002ef0c16cab04acf993f863b70663e1b8ca3acbe16475ec8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339640298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:462a64dd80bf18f09e3084770c9678a441265e2d235c72a1affe8532dababe06`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:59:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:01:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 16:17:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 16:17:40 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 16:17:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 16:17:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 16:17:47 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 16:28:07 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 16:28:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:28:08 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:28:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:28:08 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:28:15 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:28:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f1c9932170e54fface2382b2550b8052ae3d41f27e66ea1294e2055dd2b2e7`  
		Last Modified: Thu, 10 Sep 2020 01:15:45 GMT  
		Size: 51.8 MB (51829661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b3db15f518f11e53c95664d0675a5d78a5329d18d5316a406c2a45907a0723`  
		Last Modified: Thu, 10 Sep 2020 01:16:41 GMT  
		Size: 192.2 MB (192249513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3b8947ed83f2a39a813e0a9172cfdd571d4c943228a74e833af60e7536cac5`  
		Last Modified: Thu, 10 Sep 2020 18:56:49 GMT  
		Size: 6.1 MB (6145377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e778341484a5a794f279cb57047e4091523b59af8684f1ba454a1fe34cc9502c`  
		Last Modified: Thu, 10 Sep 2020 18:56:52 GMT  
		Size: 19.1 MB (19092385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb470fd1ac0bf4c914ccb121982609db19d7939e38d45aeeb5e8f0f8d5b7463`  
		Last Modified: Thu, 10 Sep 2020 18:56:48 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68424b9e533934991c96ff175cdafe6cbf28e16e9c096f88250b83854612093d`  
		Last Modified: Thu, 10 Sep 2020 18:56:49 GMT  
		Size: 2.1 MB (2119333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v5

```console
$ docker pull python@sha256:40b8642ceecb92622d0b5382386de416f512d064f478e359723a9ab64bb594bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.1 MB (312110223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be92631439f1ad44f6559ad1da11343340337e1c97e119a1786b9fdf175baa3`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:21 GMT
ADD file:a4eb5b1dc9adb84c94eff31b2ba5949b13b32831aff9a39d23ba20bc76d16449 in / 
# Wed, 09 Sep 2020 23:53:24 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:32:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:35:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:16:37 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:16:39 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:17:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:17:20 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 07:17:22 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 07:29:33 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 07:29:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 07:29:37 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 07:29:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 07:29:39 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 07:29:53 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 07:29:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:246514107a0cb62099f20170639c25bf457998ef723200e2e9343b78321b1a79`  
		Last Modified: Thu, 10 Sep 2020 00:02:25 GMT  
		Size: 48.1 MB (48108877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782f06ecaaa87e556c843fbb9f2ba81e608a4f62e6b36c0b02e627ed4c7afa5a`  
		Last Modified: Thu, 10 Sep 2020 00:53:18 GMT  
		Size: 7.4 MB (7361019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe955dad0e3dcf587c7999271c9c58b75f211e739238e437aa8aa37a0716f83`  
		Last Modified: Thu, 10 Sep 2020 00:53:28 GMT  
		Size: 9.7 MB (9687130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2960d535a0ecb57cddcd15111617c34c401d8eec5d61b7b91c571e5b814b9e4`  
		Last Modified: Thu, 10 Sep 2020 00:53:55 GMT  
		Size: 49.6 MB (49571381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912730f35f520361a961674e39c6135ff2762c42bbe6569725a85398d4e1f967`  
		Last Modified: Thu, 10 Sep 2020 00:54:52 GMT  
		Size: 171.2 MB (171214948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b44a4b7a17e3e072755cf4a5e42a01749c17cd8ffd4f8ff62728bb3b841dc9`  
		Last Modified: Thu, 10 Sep 2020 10:37:12 GMT  
		Size: 5.8 MB (5840248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45deda5ff40e46d9a4fe8c859fa337c3cb8f660345b40e86ed39c6816605099`  
		Last Modified: Thu, 10 Sep 2020 10:37:17 GMT  
		Size: 18.2 MB (18206431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92533c954ad3fafc73561c72038dbeef361c270bb4e382f64c7e6230ab50f4b`  
		Last Modified: Thu, 10 Sep 2020 10:37:10 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc2a72c31b41d6c3bc4e2f5feb701bfeb2ef16be065c53e2c2bbfa3281e1b6`  
		Last Modified: Thu, 10 Sep 2020 10:37:11 GMT  
		Size: 2.1 MB (2119956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v7

```console
$ docker pull python@sha256:ade623aa4d5f5de21707587a1ffc3f054526ac3a177af4beb7d9f5986a407b05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303763699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971be6f1ef2ffc11f664189dfdef0d9de2c51365266e7dbe73fcb75c86a3bb86`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 10 Sep 2020 00:07:32 GMT
ADD file:340663c3add65bd8904ba51984e6080c6aa6d237bd845f4e0aa22626d31497b7 in / 
# Thu, 10 Sep 2020 00:07:35 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:39:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:40:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:43:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 14:21:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 14:21:37 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 14:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 14:23:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 14:23:31 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 14:38:38 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 14:40:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:40:21 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:40:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:40:53 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:42:17 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:42:38 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:7d9beb74056b685831827b5f21351f021873d8ba1a1170b378e5edf5f46d114e`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 45.9 MB (45869299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689ccbaccf1b655191aa8867125206ed64238bf9a9e9839c4b10af714b1226f8`  
		Last Modified: Thu, 10 Sep 2020 02:01:37 GMT  
		Size: 7.1 MB (7097950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf7011b92214ace9e792fa4ef39707503be7ea5c29200c9e71ac3f6b1afb81`  
		Last Modified: Thu, 10 Sep 2020 02:01:37 GMT  
		Size: 9.3 MB (9343399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa216e44ff17d2fdb02fb4a79ef82fd1042dfaefb74d10c5db403575fbb03fc`  
		Last Modified: Thu, 10 Sep 2020 02:02:02 GMT  
		Size: 47.4 MB (47356064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857a8e60a96da34b0fc8a25f1eeaf9f81d4ca1f8bce6c5c08ccc371f1c37a762`  
		Last Modified: Thu, 10 Sep 2020 02:02:59 GMT  
		Size: 168.5 MB (168486706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f5a95380ce0c19ede4f3d868141970e6e7052ebffa254b7d0683f9fe5879ca`  
		Last Modified: Thu, 10 Sep 2020 17:54:27 GMT  
		Size: 5.5 MB (5536357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb244333d115b4ce5449c566013af08d2118901e0fab2b0bfab78c4d3a5ff615`  
		Last Modified: Thu, 10 Sep 2020 17:54:33 GMT  
		Size: 18.0 MB (17953633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b37926856ab0e790f71155e001457434bebd10c02e6f9eb55d8daf1c43c6d1`  
		Last Modified: Thu, 10 Sep 2020 17:54:25 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f73fa407a89512d68afb5d084e7dd27bc7c63e69f1959cf587d5906a2c8bbe`  
		Last Modified: Thu, 10 Sep 2020 17:54:27 GMT  
		Size: 2.1 MB (2120059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:b1d1a1fccf45182010cd2a19502d5f16c36b287fe79e4ffd2ddd277c803233f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.8 MB (329752016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527f8e9b8bf046f24c9e59788e2e1fa4c70a6e0eac4b8e1518234b74237e93c4`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:21 GMT
ADD file:c8c11e622b1b8a1e31f32e2457ff4d1314d5cd4a7ad22b3991ab9d0542db23fd in / 
# Wed, 09 Sep 2020 23:50:22 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:28:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:29:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:31:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 14:27:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 14:27:30 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 14:29:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 14:29:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 14:29:42 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 14:40:21 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 14:41:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:41:19 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:41:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:41:44 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:42:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:43:03 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d3a32671b6316bd11f4bf18cb034394ac94d2bb3bc6d09de388b19b06fb94b91`  
		Last Modified: Wed, 09 Sep 2020 23:58:45 GMT  
		Size: 49.2 MB (49175549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1202c4ddac582c7164a6b65b13a2442759bc04660da9ca7d62fabf75225482`  
		Last Modified: Thu, 10 Sep 2020 00:42:35 GMT  
		Size: 7.7 MB (7681394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f110d64c20212ec5e7a7f0622d610346edbd6e508fde94679db44e0f2827b2f9`  
		Last Modified: Thu, 10 Sep 2020 00:42:34 GMT  
		Size: 10.0 MB (9983858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c41999aa9f871546022553f35d4fbbd39cd2bfe8e1a03cce7b1bd78d2a5b0`  
		Last Modified: Thu, 10 Sep 2020 00:43:02 GMT  
		Size: 52.2 MB (52164372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0157cfd609602e37c3d21e409001f6bc0f2b58f2a6a91519d26ed4b164dedb`  
		Last Modified: Thu, 10 Sep 2020 00:43:58 GMT  
		Size: 183.8 MB (183789411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff11255613a75367041014989959207ccc3a973747ace191c5586e05048cb31c`  
		Last Modified: Thu, 10 Sep 2020 17:25:41 GMT  
		Size: 6.3 MB (6259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff9231ea4dc50440d5c6825b94d74e06e0f0deb972464ef44f030803f254e1`  
		Last Modified: Thu, 10 Sep 2020 17:25:45 GMT  
		Size: 18.6 MB (18577549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5009768b4c31d605d4cdc00ff0cd45a80562b2e4b599c2a3929d9b88d1443b9`  
		Last Modified: Thu, 10 Sep 2020 17:25:39 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19f9aecf6904e604530a1c3044da0992f0cdd0d7cfecb00589838081a3ce053`  
		Last Modified: Thu, 10 Sep 2020 17:25:40 GMT  
		Size: 2.1 MB (2120072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; 386

```console
$ docker pull python@sha256:f9137b06e219968d8155b21b1e192ccc67a82ad0722c466892873cdb32c23e87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce680d7d6006e515cd656e83bc6e0ab5f616c9a1531b452c0e3719fb86992d4`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 09 Sep 2020 23:39:58 GMT
ADD file:39c4b1e1e5d34f52ad1f95b26bfbbf45f307b94a52d472a561496c440f96d8a2 in / 
# Wed, 09 Sep 2020 23:39:59 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:50:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:51:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 11:50:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 11:50:35 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 11:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 11:50:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 11:50:48 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 12:07:37 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 12:07:38 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:07:39 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:07:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:07:39 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:07:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:07:52 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c89594b72f230eaccb7faa969906602c0f8e2667b7e30e66fe230243f1b5f1d0`  
		Last Modified: Wed, 09 Sep 2020 23:46:14 GMT  
		Size: 51.2 MB (51158853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b43dae2d508d4201f51ab75f9d5022efec80fbcc75ae14efd5ede61105a473f`  
		Last Modified: Thu, 10 Sep 2020 02:12:26 GMT  
		Size: 8.0 MB (7981208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad363e11f9c57ba13f1890587ea2eca980dd6204b267537d3668aa51dc315834`  
		Last Modified: Thu, 10 Sep 2020 02:12:26 GMT  
		Size: 10.3 MB (10338551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d8672d97325675a30cec8549334e1d5a9cacf2cc89afb39870cec739e2fb80`  
		Last Modified: Thu, 10 Sep 2020 02:12:57 GMT  
		Size: 53.4 MB (53432957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4945e32c0453d983e945c02baaa722127c521885dac39d0434ec07474cc3a5`  
		Last Modified: Thu, 10 Sep 2020 02:14:19 GMT  
		Size: 198.8 MB (198808259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df173b7755791d248eaddf3e6aa1a4b921d08677c6764381b73ce8e7fdcd97b9`  
		Last Modified: Thu, 10 Sep 2020 15:17:20 GMT  
		Size: 6.5 MB (6489293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfeb874c91cf023d3a8e28b1dbd10501cb34aaecf55cbb3ec3332eb8da66557`  
		Last Modified: Thu, 10 Sep 2020 15:17:24 GMT  
		Size: 18.4 MB (18379704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573cb255366c467aad18fb3a2410f9f098eea2397dbfdc67667f6f3a92d7d5d`  
		Last Modified: Thu, 10 Sep 2020 15:17:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d383670e3a77a59552dd4c72fed8e2b1b001c32cd9616b13546333270fe329ae`  
		Last Modified: Thu, 10 Sep 2020 15:17:18 GMT  
		Size: 2.1 MB (2119627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; mips64le

```console
$ docker pull python@sha256:fcde8f447c2278b9596c8e03fddbac89a824aa695dcacc17a53aa5142726f9ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.2 MB (324226847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b20ccd4330c5fb27f556d34d5b0e2d3bb6abd1417b984804d6bebd9977aba5e`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 10 Sep 2020 00:09:36 GMT
ADD file:c0072df9b5371ab5f33b6c7207cc89cead1e9ee00ea0f68bc3c41a9e360d8ba5 in / 
# Thu, 10 Sep 2020 00:09:36 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 05:47:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 05:47:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Sep 2020 05:48:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 05:51:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 07:05:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Sep 2020 07:05:43 GMT
ENV LANG=C.UTF-8
# Tue, 15 Sep 2020 07:06:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 07:06:02 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Sep 2020 07:06:02 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Tue, 15 Sep 2020 07:46:58 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 15 Sep 2020 07:47:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Sep 2020 07:47:01 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 15 Sep 2020 07:47:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 15 Sep 2020 07:47:01 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 15 Sep 2020 07:47:23 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Sep 2020 07:47:24 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d525d039bb76c93a9b7252a652280bfd235ea07921134a11c616ed2781990153`  
		Last Modified: Tue, 15 Sep 2020 01:12:33 GMT  
		Size: 49.0 MB (49017330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582e6413b08a125f3f8d57ff42fbc15492fcae4cc957e5c2a073b19f4edf724f`  
		Last Modified: Tue, 15 Sep 2020 05:58:57 GMT  
		Size: 7.2 MB (7231597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45ae024d80db0c67d73e5af137363cc520229d8c22f89df017d180115030a5f`  
		Last Modified: Tue, 15 Sep 2020 05:58:58 GMT  
		Size: 10.0 MB (10015803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f70ac9fca2f83d6713210044c73e67dd8323bacf53b8a56ab89d8c0848e50b1`  
		Last Modified: Tue, 15 Sep 2020 06:00:06 GMT  
		Size: 50.8 MB (50842489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c8920cb288af0deaee860d66afd9d6cc31a12f07715d540c56ff4e3e52e88e`  
		Last Modified: Tue, 15 Sep 2020 06:02:17 GMT  
		Size: 179.8 MB (179801554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b01acf7c346325e5a31a8b41b48cb98f6a844b96d4144cc04940c06701420e0`  
		Last Modified: Tue, 15 Sep 2020 13:08:55 GMT  
		Size: 6.5 MB (6455047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5f535c269f62515ea2d6f464aad0b233047fa765778dbe9bda7f4722918b38`  
		Last Modified: Tue, 15 Sep 2020 13:09:04 GMT  
		Size: 18.7 MB (18743037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2c8efd42f0657911c1348f9d8c1cd1a0f2912cdf4d43910d76e8fbf07f0bf1`  
		Last Modified: Tue, 15 Sep 2020 13:08:49 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ff899f628d99ec29d06266dc6f8a7f549d157fc14813e4b5321ca3d8e7cb6c`  
		Last Modified: Tue, 15 Sep 2020 13:08:51 GMT  
		Size: 2.1 MB (2119758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; ppc64le

```console
$ docker pull python@sha256:5b1e95d489931f73e82f0ddb3383dba9a12279f3af1dd8c9b7f74ad9d4649375
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362321219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a47a8fd7ac7a52ba614ead82f61c5a1ab6ed6d746d854be2b724014ef548b1`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 10 Sep 2020 01:04:56 GMT
ADD file:a2329a0372b3b40ca345795d86a78ab4cdaa3a1eeda3a5ece35a83881543db1a in / 
# Thu, 10 Sep 2020 01:05:18 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:56:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:58:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 03:04:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 03:28:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:35:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:35:30 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:37:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:37:39 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 07:37:45 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 07:48:14 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 07:48:48 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 07:49:04 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 07:49:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 07:49:22 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 07:50:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 07:50:10 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:aff7fe9e9819c2b9d4338fae03bd06eb6784016bcf53b2eeab88c21e47dea428`  
		Last Modified: Thu, 10 Sep 2020 01:26:27 GMT  
		Size: 54.1 MB (54142644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ac2eaf169d79a8354a5aaf6bab62ffaf296672724b4dd0027129293ddadf9`  
		Last Modified: Thu, 10 Sep 2020 04:10:06 GMT  
		Size: 8.3 MB (8255018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742b7f13bb5936990b399882cff555713c042bbc82bb798fb24d1910e772a5e`  
		Last Modified: Thu, 10 Sep 2020 04:10:07 GMT  
		Size: 10.7 MB (10727473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8644560ef7f8ccfd3073c9565885e70b26ed53108382c857d5d058bf92136a`  
		Last Modified: Thu, 10 Sep 2020 04:12:27 GMT  
		Size: 57.5 MB (57456465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b300a682ce8bcf6ab1ca7a3d241abb7170ecc083468b8a46226a995556f72eb`  
		Last Modified: Thu, 10 Sep 2020 04:17:40 GMT  
		Size: 203.1 MB (203074980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f433a75dda853e077e94d807f303b64c1824904e95cb835a6282e0b8cd5059`  
		Last Modified: Thu, 10 Sep 2020 10:57:16 GMT  
		Size: 6.9 MB (6893342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3e1fd8284a9cc21035b3d7f220f150246001d855e5f93737579f2b0c2a1ca5`  
		Last Modified: Thu, 10 Sep 2020 10:57:38 GMT  
		Size: 19.7 MB (19651110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b49c2620083a3e76084f3d60b2ef50234e9afcf495cb9f89d946736563884d6`  
		Last Modified: Thu, 10 Sep 2020 10:57:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20257a5361e4cb48902f9a4ebacecc9967f9eaab0ce1dd9ebc98742a90b1bfbf`  
		Last Modified: Thu, 10 Sep 2020 10:57:19 GMT  
		Size: 2.1 MB (2119956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; s390x

```console
$ docker pull python@sha256:77b624ec5986bcf75b8657117a8e06919af257507336d47c55cecaea5cbcbdcf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321416551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c50ce8fda9b14b73a3bea002856bdece7a114d352fb22129fc441777aa5e8a`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:11 GMT
ADD file:67eedff26215ed3c8100b93d0201c563ec8efe2af7bdfff5c7717037f95057af in / 
# Wed, 09 Sep 2020 23:42:15 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:06:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:07:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:08:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:03:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 02:03:32 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 02:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:03:38 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:03:38 GMT
ENV PYTHON_VERSION=3.9.0rc1
# Thu, 10 Sep 2020 02:08:14 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Thu, 10 Sep 2020 02:08:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:08:16 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:08:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:08:17 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:08:22 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:08:23 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:4c594945c9b37f16bdb296d1c06754e5bbcc3c28a736d7aa6091f61a081b3cfb`  
		Last Modified: Wed, 09 Sep 2020 23:46:12 GMT  
		Size: 49.0 MB (48966294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e127f29ba8a9174c7c67de6a285e78af9f06c2c36fed6521332d7854917d2782`  
		Last Modified: Thu, 10 Sep 2020 00:12:13 GMT  
		Size: 7.4 MB (7385208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e209a7f0db80455bc526e00593053bd27892e74f2f355899c7b05b2f8b74dce1`  
		Last Modified: Thu, 10 Sep 2020 00:12:13 GMT  
		Size: 9.9 MB (9882116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d094fc7b8815cbefc16bd1eb31d1052bf6fa6016dbaf460808e7a49665906c`  
		Last Modified: Thu, 10 Sep 2020 00:12:27 GMT  
		Size: 51.4 MB (51380064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e33435ff05b1d709e8481a768a66d731a33864eae8c67a15d4a79cc2d428e`  
		Last Modified: Thu, 10 Sep 2020 00:12:53 GMT  
		Size: 176.8 MB (176813448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ab9ac192e4bb5377d0add3dda1a1995f5199a3fd54b4d11322187ba2991db`  
		Last Modified: Thu, 10 Sep 2020 02:52:52 GMT  
		Size: 6.1 MB (6058102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd04f1c1086d81d3704acd8bbe81fa71b5c609359ac1bc4573a4dabe6b193f`  
		Last Modified: Thu, 10 Sep 2020 02:52:54 GMT  
		Size: 18.8 MB (18811067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628f74c25efe125182a74925f22f01857099866da6bcb86ba7886d6ec587691a`  
		Last Modified: Thu, 10 Sep 2020 02:52:51 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa290cdf81a62889fa46e788ebe7e7e02f340723f4896d57d65288a28ccb56d`  
		Last Modified: Thu, 10 Sep 2020 02:52:52 GMT  
		Size: 2.1 MB (2120019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
