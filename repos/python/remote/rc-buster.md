## `python:rc-buster`

```console
$ docker pull python@sha256:303b4a9cbc9e8150ef8a98603caccf385c1574488f05c07b9dc578e407495449
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
$ docker pull python@sha256:e117536fad544577ff5f1c22108c15b2d08727041badbd9a8859f4f39622c4dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.1 MB (350122537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faab31e8b94de30239ed50e08bcf308522c63757fe4c211b34cb508680040dfc`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 13 May 2020 21:20:19 GMT
ADD file:a50affde4f5ccdfd6450a642199121ffc180bb8cace944a55fab7a78ea851199 in / 
# Wed, 13 May 2020 21:20:19 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:27:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:28:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:29:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:45:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 May 2020 03:45:31 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 22:21:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:21:29 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 14 May 2020 22:21:30 GMT
ENV PYTHON_VERSION=3.9.0a6
# Thu, 14 May 2020 22:32:38 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 14 May 2020 22:32:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 14 May 2020 22:32:40 GMT
ENV PYTHON_PIP_VERSION=20.1
# Thu, 14 May 2020 22:32:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Thu, 14 May 2020 22:32:40 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Thu, 14 May 2020 22:32:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 14 May 2020 22:32:52 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:be2ea06d55bb33c31098151d199a24029c4e0dd6bc5b3da9f617bb04e37d79d9`  
		Last Modified: Wed, 13 May 2020 21:26:07 GMT  
		Size: 50.4 MB (50387525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b353a80f0a7f8fad0ab9c83c30a335d821e084c20b62cf5ea881c00f5ee6aff6`  
		Last Modified: Wed, 13 May 2020 22:45:09 GMT  
		Size: 7.8 MB (7812385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f42905b195f8e4cad9788956a131dedb26c1be58f7e369ae2501e029fa863cb`  
		Last Modified: Wed, 13 May 2020 22:45:09 GMT  
		Size: 10.0 MB (9996250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c983e7b0e4d15e55eca9b2619b632703323413da9e3a2f4115776ddd2a5eb18a`  
		Last Modified: Wed, 13 May 2020 22:45:30 GMT  
		Size: 51.8 MB (51827301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393dca3cd7d4378d10f8f71dbff31fd73e185f2c66c8ec98136d4c12482901f4`  
		Last Modified: Wed, 13 May 2020 22:46:19 GMT  
		Size: 192.2 MB (192211292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb525d4b0a6e6b013aa266ded0239e565f17b07f5547944e1eb584649560eb18`  
		Last Modified: Fri, 15 May 2020 00:57:22 GMT  
		Size: 6.1 MB (6145236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbe2e96b272dd66bb411f5385d953e84445a9dbf2332e6be03323be7255c84f`  
		Last Modified: Fri, 15 May 2020 00:57:27 GMT  
		Size: 29.8 MB (29811176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3454bddf06280d09492befda387a50e244c8f4d44ce6c138da190458d134485`  
		Last Modified: Fri, 15 May 2020 00:57:21 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f628416cac4fdece3751f46b7850cae46e9dfeda4308411a42185a7a212b102c`  
		Last Modified: Fri, 15 May 2020 00:57:21 GMT  
		Size: 1.9 MB (1931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v5

```console
$ docker pull python@sha256:66d906bfcea77c4e4492accb0db43fd3c02465e6d0f3a23f8026b89fb199b226
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.1 MB (321056731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d78b4d238c667609f0e6f7bb448e28b28eb6a3e8c7e51128f1a701b9f59c1d`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 14 May 2020 22:37:33 GMT
ADD file:4c10ab201790c23b97915a6e841b9567581a4fbf17ffbfe84e980ca243a8467f in / 
# Thu, 14 May 2020 22:37:37 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:42:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:42:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:45:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:34:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 05:34:34 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 05:34:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:34:56 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 05:34:57 GMT
ENV PYTHON_VERSION=3.9.0a6
# Fri, 15 May 2020 05:47:32 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 05:47:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 05:47:38 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 05:47:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 05:47:40 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 05:47:53 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 05:47:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:fb15ddec83dc56686109e855646d15f68bcd184e7d41da9ccbd93503b895e080`  
		Last Modified: Thu, 14 May 2020 22:46:29 GMT  
		Size: 48.1 MB (48107469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c9c9c97e34eb4f2a81e603f898669fb24b84ad169c84d6a88c3cc6c80ec019`  
		Last Modified: Fri, 15 May 2020 04:01:55 GMT  
		Size: 7.4 MB (7359224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f1d00aaa84dd193d874cc9585feca69c6fa2d283d1fd8d030356afd24de516`  
		Last Modified: Fri, 15 May 2020 04:01:55 GMT  
		Size: 9.7 MB (9687067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc2154178d1d783f1d3d36ef36653de4543bcc6aa884be7b41ec5fb56c43545`  
		Last Modified: Fri, 15 May 2020 04:02:19 GMT  
		Size: 49.6 MB (49572197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd297adae8fa0fd0c3171f5c2e2a11b23638bf222f34239ab280c332b89c0e9`  
		Last Modified: Fri, 15 May 2020 04:03:17 GMT  
		Size: 171.2 MB (171166481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c28b9c1b235bb7e03d1476fc1252a0728d8de9adc748d104e0497111baca3e`  
		Last Modified: Fri, 15 May 2020 08:20:26 GMT  
		Size: 5.8 MB (5839990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7e12aea38375743859301c335786e65605013cc4d58af6ae35a75bc28b0972`  
		Last Modified: Fri, 15 May 2020 08:20:34 GMT  
		Size: 27.4 MB (27392709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8858decb7e1fcd396cc52d3d376d5460b87b87ddc8b8bba1033d4c3ec569a73a`  
		Last Modified: Fri, 15 May 2020 08:20:24 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2ea862689c47fe1b42ba6446864b6a2375f3193b42f7cc4fe22a4a323ed345`  
		Last Modified: Fri, 15 May 2020 08:20:24 GMT  
		Size: 1.9 MB (1931362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v7

```console
$ docker pull python@sha256:a8538c7e8ec0b8c33d08f0e16dc6a1cbad19fefeb450673aa5604cf6db64d88d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312622155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556999326f37b5d25e527189800131e725cd2b8b5bbfd2e9a7833ca99421b5b2`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 15 May 2020 00:59:31 GMT
ADD file:d3b126babe4f145c735dff1d1a8828e523967279b9f25d547fce6f4d5422d0a4 in / 
# Fri, 15 May 2020 00:59:33 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:34:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:34:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:35:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:37:07 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:36:24 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 19:36:25 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 19:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:36:41 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 19:36:41 GMT
ENV PYTHON_VERSION=3.9.0a6
# Fri, 15 May 2020 19:50:30 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 19:50:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 19:50:34 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 19:50:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 19:50:42 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 19:50:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 19:51:02 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:33f1e205e6f963868048d05375e218b5a53592240c265ac49b4860e141d25c66`  
		Last Modified: Fri, 15 May 2020 01:11:01 GMT  
		Size: 45.9 MB (45868629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83963556ddab1d93e22197bee7fc0d66da2f25f8ae77f4147c0ebee63db933e3`  
		Last Modified: Fri, 15 May 2020 10:57:21 GMT  
		Size: 7.1 MB (7096812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52e6e35f16ed7d977f73bf736fe9e27ba863d03fa402e68e53f187ae3c43123`  
		Last Modified: Fri, 15 May 2020 10:57:22 GMT  
		Size: 9.3 MB (9343333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf172e11e265992a6dffd35b590fb6e71abfee19640961a4b80f8e7f8280ce8b`  
		Last Modified: Fri, 15 May 2020 10:57:47 GMT  
		Size: 47.4 MB (47355661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3d123dcffed07078e9c806cf5b083caca65ee1ba452e2261dbe99b3f348c93`  
		Last Modified: Fri, 15 May 2020 10:58:41 GMT  
		Size: 168.4 MB (168419331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b28ed1a23ea95cc49fc5f0f080cb5d8eb21957b87a2214a3f55364234130f`  
		Last Modified: Fri, 15 May 2020 21:14:48 GMT  
		Size: 5.5 MB (5535905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6775a0289c6eff6326794f437ae995ce60823dc220781574adee7c6c2a70db4f`  
		Last Modified: Fri, 15 May 2020 21:14:57 GMT  
		Size: 27.1 MB (27070875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cbd762287d4bd31bdb1a80f3c2398e8778bda8ce455ebb0427e63d360a67de`  
		Last Modified: Fri, 15 May 2020 21:14:47 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976e10057b7a7c0a751f30d0612ef54a3936a31a24bea356c926d28dfc4521b0`  
		Last Modified: Fri, 15 May 2020 21:14:47 GMT  
		Size: 1.9 MB (1931379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:4ab9054a5678278c0f821892395790d2226b08b982e8e91e8f244ddd8d5d722b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339699616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c102af557b92ca0a0c6daff03f6c856a2e5026f46aec55bfabd9c03e596cf8e1`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 13 May 2020 21:43:08 GMT
ADD file:685903e2621502d2f743969aaf293a5feab58680a95cd93a5ebf2b07f3b5d358 in / 
# Wed, 13 May 2020 21:43:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:24:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:24:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:27:21 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 20:29:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 May 2020 20:29:36 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 20:30:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 20:30:03 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 14 May 2020 20:30:04 GMT
ENV PYTHON_VERSION=3.9.0a6
# Thu, 14 May 2020 20:40:18 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 14 May 2020 20:40:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 14 May 2020 20:40:22 GMT
ENV PYTHON_PIP_VERSION=20.1
# Thu, 14 May 2020 20:40:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Thu, 14 May 2020 20:40:27 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Thu, 14 May 2020 20:40:45 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 14 May 2020 20:40:46 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:0be831822ade5f87765ba6ff26243b12a3ecd4c379df96483549a7992c1fd35b`  
		Last Modified: Wed, 13 May 2020 21:52:50 GMT  
		Size: 49.2 MB (49168115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2879905fcfbdfe9945e6eb39396c6b52b929faf145449ab656f7b35bb6387a`  
		Last Modified: Wed, 13 May 2020 22:39:40 GMT  
		Size: 7.7 MB (7681618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2769f7d2af01c05219ba1529b243249dcedccd56fabeee3d41d792b819f494`  
		Last Modified: Wed, 13 May 2020 22:39:39 GMT  
		Size: 10.0 MB (9983943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e8c22f4290c6000d75544c42d271474d93302f7cd74ef79832ba3c93c962a`  
		Last Modified: Wed, 13 May 2020 22:40:02 GMT  
		Size: 52.2 MB (52155958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b85452f917a631debce0633df2f9e9a5ee7f79a4d2553949182ffd209a6f5`  
		Last Modified: Wed, 13 May 2020 22:40:54 GMT  
		Size: 183.7 MB (183741566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ec242a525b26acd13ada6ee2de1be6a48222caaf10992e98ea182de4f2094`  
		Last Modified: Thu, 14 May 2020 23:31:43 GMT  
		Size: 6.3 MB (6259391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5c1cc17572e2b650ba9d9009ceb69f07f8826c556fbebe65f53055a1ecc04b`  
		Last Modified: Thu, 14 May 2020 23:31:52 GMT  
		Size: 28.8 MB (28777386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5cb92552849d5e36fd179581105b2573601be999c80c1446e756a814215c35`  
		Last Modified: Thu, 14 May 2020 23:31:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0d63c0e187c09ead7b8835fc70a0750261666edef711d1a6279c608bc7b6de`  
		Last Modified: Thu, 14 May 2020 23:31:42 GMT  
		Size: 1.9 MB (1931406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; 386

```console
$ docker pull python@sha256:4bf806cb6b400840863210bf722c850fa7cb94d66d999d477b595cfa2f799a3a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.0 MB (357960224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2080d9bacc01bde59c2d67ad78f1114a8aa5ecfe77c7b37d46a7a936da8b80`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 15 May 2020 07:07:17 GMT
ADD file:8e3b513586e9ff0d65f88b3b2978986693585177fae673aa5432e2934e212cf1 in / 
# Fri, 15 May 2020 07:07:17 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:07:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:07:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:07:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:09:05 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 23:59:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 23:59:40 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 03:28:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:28:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 16 May 2020 03:28:06 GMT
ENV PYTHON_VERSION=3.9.0a6
# Sat, 16 May 2020 03:45:12 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 16 May 2020 03:45:13 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 16 May 2020 03:45:13 GMT
ENV PYTHON_PIP_VERSION=20.1
# Sat, 16 May 2020 03:45:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Sat, 16 May 2020 03:45:13 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Sat, 16 May 2020 03:45:21 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 16 May 2020 03:45:22 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:8f68852a383b581a180c01bf6d2f7039194fed91451d0686630c59cb80d321c3`  
		Last Modified: Fri, 15 May 2020 07:17:49 GMT  
		Size: 51.2 MB (51157846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126dd406c4f640ca6230b5a4b713a552e39df8129fac9f67e1c27bfa61d92953`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 8.0 MB (7981878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299696f31e375aea3d6d222d2ddd28b4972fc3855d3fa45ea032ffab0fd57dd`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 10.3 MB (10338576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae07435f995dcd7d000780f0887c530a2218056928cee15a21edf6940cbd9c`  
		Last Modified: Fri, 15 May 2020 17:26:48 GMT  
		Size: 53.4 MB (53428852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc0f92b2c8d8b3b838b176dbac16e8bf85eedb134e7df0761013b92f548cb8`  
		Last Modified: Fri, 15 May 2020 17:27:42 GMT  
		Size: 198.8 MB (198755024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a5d24459c46b500ac368fd1b476255158e1ab3be3c0c14915d2350c0a21238`  
		Last Modified: Sat, 16 May 2020 05:11:29 GMT  
		Size: 6.5 MB (6489122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07aa319bd0a542cf7d570d181f1c7131eae9172bebb894fbe45f6c2117ee9c7`  
		Last Modified: Sat, 16 May 2020 05:11:39 GMT  
		Size: 27.9 MB (27877504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4d838bca68557a8e1cf675b9e359aabc83db41a15a14e12e4277be4926e4e4`  
		Last Modified: Sat, 16 May 2020 05:11:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db17193008b9c3cd7d84a7e699d449b75a3d54045fd71387a345eaac9cc95e59`  
		Last Modified: Sat, 16 May 2020 05:11:27 GMT  
		Size: 1.9 MB (1931191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; mips64le

```console
$ docker pull python@sha256:2bd23d33d81ecdab84b7cbe46afdb00aab53074c024792d646f006817e026036
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.7 MB (334699957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53460fe47e51eb79b899abf626556d2e4ecc15961c18693faac1bf5882268c9c`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 15 May 2020 04:47:51 GMT
ADD file:0ddadadf9bac33aa2c030e9f35797265ae45bedabeeee3c1a7db17849db5d1f6 in / 
# Fri, 15 May 2020 04:47:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:37:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 14:38:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:40:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:45:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 17:45:08 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 17:45:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:45:26 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 17:45:26 GMT
ENV PYTHON_VERSION=3.9.0a6
# Fri, 15 May 2020 18:33:05 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 18:33:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 18:33:08 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 18:33:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 18:33:08 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 18:33:32 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 18:33:32 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:2d4d74c73ac68f6d7577b51be94381bbbbfec8dd4e7b329089ca42b7d41a75bf`  
		Last Modified: Fri, 15 May 2020 04:56:25 GMT  
		Size: 49.0 MB (49019343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404e44ede21b71fba958dcbf67f3e30056b14cfe75ac7c0edc7c26586310d2d`  
		Last Modified: Fri, 15 May 2020 14:51:07 GMT  
		Size: 7.2 MB (7229891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5107f44d6fb498f29d6e1695ffa66a63840c5c7d91adb30d6a538c8cb06b66`  
		Last Modified: Fri, 15 May 2020 14:51:00 GMT  
		Size: 10.0 MB (10015839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75e4e64bf83c899f8786006ad0ef0a1ec9df0a6cd3754a65c48cb5ac4382597`  
		Last Modified: Fri, 15 May 2020 14:52:07 GMT  
		Size: 50.8 MB (50839436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90090e9e3c0004f0b544497a3404c68963d6b681b3b4c69d66a3137fc56d67c`  
		Last Modified: Fri, 15 May 2020 14:54:34 GMT  
		Size: 179.7 MB (179749794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b93585e6873f0debf54fafae31d0d10f215111b50c520b30729668395fae8`  
		Last Modified: Fri, 15 May 2020 22:04:09 GMT  
		Size: 6.5 MB (6454865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475a3a0ab137de38efd88789a9ff09431b703d1bb77de0269e02c23c2c9caf1`  
		Last Modified: Fri, 15 May 2020 22:04:33 GMT  
		Size: 29.5 MB (29459368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e50fdd1526102840a66ad850773e252f1394cef67af30a2b22f14d73c09dcb`  
		Last Modified: Fri, 15 May 2020 22:04:02 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a7e91db58d0324efb1612710efd44b33661a4384711b090af116ef01bed5d5`  
		Last Modified: Fri, 15 May 2020 22:04:05 GMT  
		Size: 1.9 MB (1931189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; ppc64le

```console
$ docker pull python@sha256:a6156831958afd561d56365e1a9dd05e8ae5dc1272c6aae9a2abb921546ffd1d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.0 MB (373035893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24de1b376dd586e88e5c3d64915f3e9c89aeb08b01704d9b97791d14fc8f133`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 13 May 2020 22:20:32 GMT
ADD file:ed5dc7bd2c0c0dafef9ca4829cd89719c538cd23991fb941589e7fd3bf96b407 in / 
# Wed, 13 May 2020 22:20:38 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:43:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:44:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:54:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 17:01:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 May 2020 17:01:46 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 20:13:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 20:13:23 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 14 May 2020 20:13:32 GMT
ENV PYTHON_VERSION=3.9.0a6
# Thu, 14 May 2020 20:24:48 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 14 May 2020 20:25:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 14 May 2020 20:25:09 GMT
ENV PYTHON_PIP_VERSION=20.1
# Thu, 14 May 2020 20:25:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Thu, 14 May 2020 20:25:22 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Thu, 14 May 2020 20:25:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 14 May 2020 20:25:57 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:19aca0f2a5b89bbc37caa77bbd1612566fadbbce5c3381246fe356d7e5d14774`  
		Last Modified: Wed, 13 May 2020 22:57:18 GMT  
		Size: 54.1 MB (54142914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556cd6fadc0f341d090a18ecfc4b6aedccd3d99f6eb6a336e3bee33f096c095f`  
		Last Modified: Thu, 14 May 2020 00:28:57 GMT  
		Size: 8.3 MB (8252823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633177125031b056c9e79b442829845cc6886ad14d5de3cc2459317eaa054d94`  
		Last Modified: Thu, 14 May 2020 00:28:59 GMT  
		Size: 10.7 MB (10727164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762e21652d78f0bcf2f8011e2751e5d6be323a639e89c083f93a086fe1b6005`  
		Last Modified: Thu, 14 May 2020 00:30:19 GMT  
		Size: 57.5 MB (57459915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25daff9ab67476e2376e496ffe3b8ee9e8b1ce159afabc20b9925d9ffc106448`  
		Last Modified: Thu, 14 May 2020 00:33:04 GMT  
		Size: 203.0 MB (203016026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3574b232379c43a88ad5b06eab7012c39dc2730116496fb7539ea7393ddb854`  
		Last Modified: Fri, 15 May 2020 00:16:57 GMT  
		Size: 6.9 MB (6892251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38479e28aea4f19c832d5a5dbbb473bad13ad1b8895e9c9b8c2a649053d124fb`  
		Last Modified: Fri, 15 May 2020 00:17:13 GMT  
		Size: 30.6 MB (30613186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd2a72a1f5060476e9bb6068e8ddec6cbfb529d98b5e27b3963334766b8c758`  
		Last Modified: Fri, 15 May 2020 00:16:47 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfcda286cfb410be81e0491be629cceb0ce54eec8f8928a9ddd894de0f0e904`  
		Last Modified: Fri, 15 May 2020 00:16:51 GMT  
		Size: 1.9 MB (1931380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; s390x

```console
$ docker pull python@sha256:79ed64f2657029e307afa484c3e86e5c3a002969bf365aefd5be2d0d99e74efe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.0 MB (332042296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225b23d46fb2d0ed224573fccf6cd5cc99c13553084a2def95405914478225e5`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 14 May 2020 23:06:22 GMT
ADD file:3b65bac2545f5751eaa8e9967febbe18955f63efa32d5ca3f8bc209e1a8602de in / 
# Thu, 14 May 2020 23:06:24 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:00:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 05:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:02:18 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:37:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 07:37:14 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 08:32:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 08:32:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 15 May 2020 08:32:51 GMT
ENV PYTHON_VERSION=3.9.0a6
# Fri, 15 May 2020 08:37:44 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 15 May 2020 08:37:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 15 May 2020 08:37:47 GMT
ENV PYTHON_PIP_VERSION=20.1
# Fri, 15 May 2020 08:37:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1fe530e9e3d800be94e04f6428460fc4fb94f5a9/get-pip.py
# Fri, 15 May 2020 08:37:47 GMT
ENV PYTHON_GET_PIP_SHA256=ce486cddac44e99496a702aa5c06c5028414ef48fdfd5242cd2fe559b13d4348
# Fri, 15 May 2020 08:37:54 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 15 May 2020 08:37:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:070f0b30acfe8cf53f3aeaae5982c911acd4c4a652a456c849a94c66117d4067`  
		Last Modified: Thu, 14 May 2020 23:11:09 GMT  
		Size: 49.0 MB (48966486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db7092766f19f5c47b8a2388225b82a8d95d39c4e0ae321805e2a5cf0c8b961`  
		Last Modified: Fri, 15 May 2020 05:08:53 GMT  
		Size: 7.4 MB (7382266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643084632f50b88b1aea5263e63d7dff9175610fe2041ce83dcdbb3d926246d8`  
		Last Modified: Fri, 15 May 2020 05:08:59 GMT  
		Size: 9.9 MB (9882148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118b891b350fa9ce5f64fd71fe7161ade2a6f32705dbd623b014ff5198f96b0`  
		Last Modified: Fri, 15 May 2020 05:09:13 GMT  
		Size: 51.4 MB (51368440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c98f9d2d49b60131c8d94d20aefe521b7397fb01c63af9574b1cfdedec7d99`  
		Last Modified: Fri, 15 May 2020 05:09:50 GMT  
		Size: 176.8 MB (176763372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7c4952cb4277702446e14426a77da4cc1a7ab687e3755a403dd3e1e40ce80b`  
		Last Modified: Fri, 15 May 2020 09:12:56 GMT  
		Size: 6.1 MB (6058036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d08ce64f0d3ea7b603fc4afc4b8bf93ee15d58497ecde0e9b78d3cc607374b`  
		Last Modified: Fri, 15 May 2020 09:13:06 GMT  
		Size: 29.7 MB (29690127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42088743d828e4bb4cd191c4bc374c8459ec31d39954789a706511c3ed31e2f8`  
		Last Modified: Fri, 15 May 2020 09:13:00 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f2be96167bdc1f7235d609f907f874de04cacd1fdda72be0102ff37da3cfa`  
		Last Modified: Fri, 15 May 2020 09:13:11 GMT  
		Size: 1.9 MB (1931189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
