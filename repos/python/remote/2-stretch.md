## `python:2-stretch`

```console
$ docker pull python@sha256:c9d47fb72a54268a33a577798f2291a3ebca1408f646ef10e091f4b0eb7bed6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `python:2-stretch` - linux; amd64

```console
$ docker pull python@sha256:97e366231a9643a9ab4576133d5c9bfcb74986f0eaef8056248e3d9ebd6855f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.3 MB (355279540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e525a2edc46457b7561ad1bac69abf12544fc009ed516b9457b86478d83e695`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:34:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:35:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:50:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:50:17 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 10:52:31 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 10:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:52:38 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 10:52:38 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 10:58:28 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 10:58:28 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:41:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:41:48 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:41:53 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:41:55 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 06 Feb 2020 01:41:56 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c160265e75550c2ed099aa7d3906b3fef0bf046a2aeead136f8e587a015159`  
		Last Modified: Sun, 02 Feb 2020 00:42:04 GMT  
		Size: 10.8 MB (10797219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4fe40d0e618e3319afb689c3570bb87e8e8cf51bca080364d1552317bc66c2`  
		Last Modified: Sun, 02 Feb 2020 00:42:02 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d647f502a07e6daaee43c23cfac9399501b1d7f55fb4c60d56307e23f0ed5a5`  
		Last Modified: Sun, 02 Feb 2020 00:42:26 GMT  
		Size: 50.1 MB (50073989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bd59397b26db56ddd19f152a7095a91795cf4af7f144ebc4dae741df451039`  
		Last Modified: Sun, 02 Feb 2020 00:43:16 GMT  
		Size: 214.8 MB (214840255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d1dd25b949aeb1625cbada7c5201848a22972b5ad4df451075a59a816f7ce`  
		Last Modified: Sun, 02 Feb 2020 11:09:59 GMT  
		Size: 5.7 MB (5747384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78bca6caced0daa13ad1322a8918d6841ae7f8d5b174114bbc309e1f1a057c4`  
		Last Modified: Sun, 02 Feb 2020 11:10:03 GMT  
		Size: 17.0 MB (17041171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e244c95364ac9f83eedd0dd44102b5cd50d5308fe94285ce815f3c098f8eb60c`  
		Last Modified: Thu, 06 Feb 2020 01:46:06 GMT  
		Size: 1.9 MB (1888364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b837be8f329e970136aff30f9670c06fe56fdbe1ebff5387c94d6e25392f2`  
		Last Modified: Thu, 06 Feb 2020 01:46:06 GMT  
		Size: 5.2 MB (5170284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; arm variant v5

```console
$ docker pull python@sha256:a181a1d00dfa6ea9fb9e6053ff5347efc2290ff8aa4f399545ca1542a9f3d1a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.0 MB (338025908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f70ab96c0d935a3df1f5c81829b811916735b145823c3a44eeb60df7ca98ad9`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:39 GMT
ADD file:f229f8ad575dbe0eecebbaa4c410371dbbaf8a20b6dccecb7a73b2cfb6706372 in / 
# Sat, 01 Feb 2020 16:53:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:39:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:43:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:37:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 23:37:21 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 01:33:56 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 01:34:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:34:14 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 01:34:14 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 01:44:02 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 01:44:04 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:02:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:02:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:02:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:02:34 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 06 Feb 2020 01:02:35 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:4a136771265373b04f705abd2c190724eab8195169bce62483ae7ccf66454fbd`  
		Last Modified: Sat, 01 Feb 2020 17:00:43 GMT  
		Size: 44.1 MB (44073363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737ede4867d27cb17990eb627f00e8c022e69b04e5abcf499619938bb7acea1`  
		Last Modified: Sat, 01 Feb 2020 17:49:27 GMT  
		Size: 9.9 MB (9866296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a23044dd3f88be1b32a8d6c055ee1b6ae0aa0cef40a6949663b4a21797cd2a`  
		Last Modified: Sat, 01 Feb 2020 17:49:25 GMT  
		Size: 4.2 MB (4159202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7489f293feb0958fb3e65740f118783e63eaad1ecb6ba3cdd94bad6f2f52af7d`  
		Last Modified: Sat, 01 Feb 2020 17:49:49 GMT  
		Size: 48.3 MB (48283756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881cc46722a2965e498ab9d380e9d9c2a7535fefa9391bea6e471ef0813a5e29`  
		Last Modified: Sat, 01 Feb 2020 17:50:52 GMT  
		Size: 203.0 MB (203038040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6c455712c216a437f17ac496922ea917e97779f009f6423af6264b9bb1e7cf`  
		Last Modified: Sun, 02 Feb 2020 02:03:12 GMT  
		Size: 5.5 MB (5531221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09c49aed1fd1e556b7f962b1b7d43ee1ac38ad72b273ab11877bfb9e2d1e70`  
		Last Modified: Sun, 02 Feb 2020 02:03:16 GMT  
		Size: 16.0 MB (16014678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b25352ff3c612b9dcd4240dfa8274e74098e9cb3f566300cd95482c251cbc9`  
		Last Modified: Thu, 06 Feb 2020 01:09:02 GMT  
		Size: 1.9 MB (1888526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a5242e51144bb099dad6da5aeacb0697f201005c319160ee53c1fbe7bc08b8`  
		Last Modified: Thu, 06 Feb 2020 01:09:02 GMT  
		Size: 5.2 MB (5170826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; arm variant v7

```console
$ docker pull python@sha256:1b9a6dc74f39e568b2b4a69a9eda2a4b1985a8348ee246a3b577a4ac634d7e42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325345034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b326c266a93bb620b7826d277c74109d4734965d7a35b622805a5f5f8771f2fa`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:23:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 05:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 05:52:23 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 08:00:11 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 08:00:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:00:24 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 08:00:25 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 08:08:55 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 08:08:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Sun, 02 Feb 2020 08:08:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sun, 02 Feb 2020 08:08:58 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sun, 02 Feb 2020 08:09:09 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 02 Feb 2020 08:09:16 GMT
RUN pip install --no-cache-dir virtualenv
# Sun, 02 Feb 2020 08:09:17 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854dcba3350bdff3f923ff69f2dec445f47ef5726d3d15bde4242c2ff122aabc`  
		Last Modified: Sat, 01 Feb 2020 18:32:28 GMT  
		Size: 195.5 MB (195523495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f22abb8c3de6c7076d0950f7b80c4676e09808b1b6e4d85594aff19d669108d`  
		Last Modified: Sun, 02 Feb 2020 08:26:56 GMT  
		Size: 5.2 MB (5197171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddc79480a7270a853505c244f2aa3493733440f800a15eaa94491f6177ce3aa`  
		Last Modified: Sun, 02 Feb 2020 08:27:00 GMT  
		Size: 15.6 MB (15639520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc46d07c0472d4e751d557fb1592ec073ad4b22ce17624cea1defc884413b4a`  
		Last Modified: Sun, 02 Feb 2020 08:26:55 GMT  
		Size: 1.9 MB (1888504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a843cd1f4b44cbf5e275f62834370fe99c30fa7c8e21a906a6a6b7944fd382`  
		Last Modified: Sun, 02 Feb 2020 08:26:55 GMT  
		Size: 5.2 MB (5170888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; arm64 variant v8

```console
$ docker pull python@sha256:ff04f7267460adcac8d35b89c7893f2cf543dde19d08573b31bc28b908153bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.3 MB (336291540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e231702e90d4442e3858352bcea612e890b50b08f8d2f038418ba614fb6ec0e6`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:30:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:32:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 04:09:46 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 04:09:47 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 07:12:40 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 07:12:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 07:12:52 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 07:12:54 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 07:20:54 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 07:20:55 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Sun, 02 Feb 2020 07:20:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sun, 02 Feb 2020 07:20:56 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sun, 02 Feb 2020 07:21:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 02 Feb 2020 07:21:14 GMT
RUN pip install --no-cache-dir virtualenv
# Sun, 02 Feb 2020 07:21:15 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf173a01baf7d45b479bb380ece219cbf0ea52178e9b8cdc5b87891759d1122`  
		Last Modified: Sat, 01 Feb 2020 17:39:19 GMT  
		Size: 9.7 MB (9748586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3392eac7bc27f3bd5fcb024413ca55ec4115c22da3e229567d5fc03cd4ff4e4`  
		Last Modified: Sat, 01 Feb 2020 17:39:18 GMT  
		Size: 4.1 MB (4094322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a82fc9ca296b095585ba7f3f6d83566428dbefcbfd284e242039aba97840b2`  
		Last Modified: Sat, 01 Feb 2020 17:39:40 GMT  
		Size: 48.0 MB (48024205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a981e1269e4bf23132efb6a90365b5d82020f20a2ae5252c2d7c3b9ad7f48`  
		Last Modified: Sat, 01 Feb 2020 17:40:34 GMT  
		Size: 202.2 MB (202233524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab3a9215947fa354fa4e9188eb5cba28725752cd02b056c632c8d589ca52e49`  
		Last Modified: Sun, 02 Feb 2020 07:37:46 GMT  
		Size: 5.5 MB (5501112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1521e512478a6db0973d849449ff03496aec4f6bb70e7527b42da40f6f1e35b`  
		Last Modified: Sun, 02 Feb 2020 07:37:50 GMT  
		Size: 16.5 MB (16463990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d29c26d55c854f24fc5e5949b9a629dfc64190971479ebf551fd17cf24bb2`  
		Last Modified: Sun, 02 Feb 2020 07:37:45 GMT  
		Size: 1.9 MB (1888528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae60a7d05e999a9d27053298ccf7ea93663f9ca35666ba3080d3d5747a88a2f`  
		Last Modified: Sun, 02 Feb 2020 07:37:45 GMT  
		Size: 5.2 MB (5170524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; 386

```console
$ docker pull python@sha256:86686e7ee1b9da5fc4861616d72c3e2e05f50ee93fb566e216ccfb89bac94fcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362068140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28fee41abff95789af4e53da04ff4693cfcc7fc3db4a745030230f42a5b8114`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:45:48 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 00:50:00 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 00:50:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:50:08 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 00:50:08 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 00:58:37 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 00:58:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:53:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:53:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:53:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:53:59 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 06 Feb 2020 00:53:59 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac9b89be3409f23bc9ac380bcfd9f28e0cc2e52b69b8706e0b102211c83abf4`  
		Last Modified: Sat, 01 Feb 2020 17:47:03 GMT  
		Size: 219.9 MB (219925297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b069519c0b5eb3eaf23000fcb44bc06506fafa6c2c14231a6a89b8f2875b0940`  
		Last Modified: Sun, 02 Feb 2020 01:14:50 GMT  
		Size: 6.1 MB (6062016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba9c1693b9f2e5731521b717178c47f1493f612def169744f234534eac9758`  
		Last Modified: Sun, 02 Feb 2020 01:14:53 GMT  
		Size: 15.9 MB (15947113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02676abe08d607c314eabe4a8c71925a9c61423d87416535376d33d23c61b1a3`  
		Last Modified: Thu, 06 Feb 2020 00:58:22 GMT  
		Size: 1.9 MB (1888378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3aacfec47e10cc205e7d51f1f3d6cf89e9dda975ed91a8e1dfeac8aeb3c2`  
		Last Modified: Thu, 06 Feb 2020 00:58:24 GMT  
		Size: 5.2 MB (5170699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; ppc64le

```console
$ docker pull python@sha256:fae4d24a40ae8b6517c0b3b4f0d3dc7ec0841834d601129dbdfe85f1367476e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350370314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:253a80a883e0d7ba639dfa9d7f99760aee708f116d27b5d4bea8693983e13b61`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:12 GMT
ADD file:ebcf4b112436fa7be8efa5ef204cc174c0d1af648c6ab4af968a71aa2ab2cf4a in / 
# Sat, 01 Feb 2020 17:20:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:06:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:13:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:22:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:22:29 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:20:04 GMT
ENV PYTHONIOENCODING=UTF-8
# Sun, 02 Feb 2020 06:20:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:20:48 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sun, 02 Feb 2020 06:20:59 GMT
ENV PYTHON_VERSION=2.7.17
# Sun, 02 Feb 2020 06:27:57 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sun, 02 Feb 2020 06:28:01 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Sun, 02 Feb 2020 06:28:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sun, 02 Feb 2020 06:28:03 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sun, 02 Feb 2020 06:28:22 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 02 Feb 2020 06:28:30 GMT
RUN pip install --no-cache-dir virtualenv
# Sun, 02 Feb 2020 06:28:33 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:072f803f12e35b1a40604b6081cb448d46529e3eb1d453ebbf56850c211f5bdb`  
		Last Modified: Sat, 01 Feb 2020 17:30:44 GMT  
		Size: 45.7 MB (45652299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738f3141f5288b7d088c111ef5c0250cf1779363648e4abd0a2fa786691279a`  
		Last Modified: Sat, 01 Feb 2020 19:25:20 GMT  
		Size: 10.0 MB (10002083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a959eee44d8ac35abe99ef74efe938d0f14c75e8ba029451e3bb2f3c594206`  
		Last Modified: Sat, 01 Feb 2020 19:25:18 GMT  
		Size: 4.3 MB (4296690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c05296e9b4c4e064ac637742557d903aff58a97639760bb778595e90492a8f`  
		Last Modified: Sat, 01 Feb 2020 19:26:08 GMT  
		Size: 50.1 MB (50086371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0053e8ab1908886809e0b53ed05d1644123e096ed152bef227af4bdd63d04506`  
		Last Modified: Sat, 01 Feb 2020 19:28:13 GMT  
		Size: 210.5 MB (210480034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de5fedc72c5e1b64bd59a44c09ae2fd7b84a36fab9054f3d9b53b3194e11264`  
		Last Modified: Sun, 02 Feb 2020 06:50:24 GMT  
		Size: 5.8 MB (5781347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc8ef11cdad79fb342bee13cbbb17ef91e8d0e91e542c3caf9d548134b9f3c5`  
		Last Modified: Sun, 02 Feb 2020 06:50:27 GMT  
		Size: 17.0 MB (17012648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7442029f16ae112ae247f91e283515d012da132b241bd7b8b2173efeadd83226`  
		Last Modified: Sun, 02 Feb 2020 06:50:23 GMT  
		Size: 1.9 MB (1888499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5d8195377f00619775a684551f6013667a89a00ca545d1273857ceebdaae8e`  
		Last Modified: Sun, 02 Feb 2020 06:50:24 GMT  
		Size: 5.2 MB (5170343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-stretch` - linux; s390x

```console
$ docker pull python@sha256:cb32e36a38a95ecd607d93e1be15b0d97b44fb540444c561b4929a0996ce0770
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.1 MB (348065379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9023150f5ccb90ba2c95422ea636e72d77b14b106b12008de02d3b065944c015`
-	Default Command: `["python2"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:43 GMT
ADD file:17af4834ca99365d5ecf14eb938572689bd3c3ad5fd8a88da12c4c3474975771 in / 
# Sat, 01 Feb 2020 16:43:45 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:00:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:01:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:28:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 21:28:15 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 23:54:01 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 01 Feb 2020 23:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:54:06 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Sat, 01 Feb 2020 23:54:06 GMT
ENV PYTHON_VERSION=2.7.17
# Sat, 01 Feb 2020 23:57:56 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Sat, 01 Feb 2020 23:57:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:52:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:52:46 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:52:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:52:55 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 06 Feb 2020 00:52:56 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:fb54e9d54b34d992a5c6582a6fe3836692cce3589a408748090bbb916a4cc63d`  
		Last Modified: Sat, 01 Feb 2020 16:47:28 GMT  
		Size: 45.2 MB (45241584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d13d85604945e95d31c38d488a822d8e0b84e7548a10db0c89115cca1887aa`  
		Last Modified: Sat, 01 Feb 2020 18:06:29 GMT  
		Size: 10.3 MB (10325358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b324848b1286794120fbcb3c696328dd955db597ec3e70840b5dc97d794db`  
		Last Modified: Sat, 01 Feb 2020 18:06:33 GMT  
		Size: 4.4 MB (4372596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38645e5b0e6402c091627176f5aed8b9d434ccf323ecc4ca2c66f934acc1a11a`  
		Last Modified: Sat, 01 Feb 2020 18:06:45 GMT  
		Size: 50.5 MB (50499891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6815a6a287c8fc9388e7131e2c39538e99952d5f119a9d0778399e162143aa71`  
		Last Modified: Sat, 01 Feb 2020 18:07:33 GMT  
		Size: 206.9 MB (206870838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7479224bb3afe52203d11f85b79c52466658d64f25af44ab37571465e013270`  
		Last Modified: Sun, 02 Feb 2020 00:01:08 GMT  
		Size: 5.8 MB (5811615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f4ae737c471376a75e06726c948be9ccbef0b1c5a8c5ecd4bff60e723afcb5`  
		Last Modified: Sun, 02 Feb 2020 00:01:15 GMT  
		Size: 17.9 MB (17884784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfb744f762773e1408154a53c3759eb09eba7335f168bd1a8703e022b71b3d6`  
		Last Modified: Thu, 06 Feb 2020 00:57:19 GMT  
		Size: 1.9 MB (1888511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854df11a85e285cbd340cdb22db52a09c91152db9268b836631408072f10495a`  
		Last Modified: Thu, 06 Feb 2020 00:57:18 GMT  
		Size: 5.2 MB (5170202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
