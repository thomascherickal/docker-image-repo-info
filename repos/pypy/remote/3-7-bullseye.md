## `pypy:3-7-bullseye`

```console
$ docker pull pypy@sha256:f906393bb3658aaa544a71f6e7c4d86ec263128608e9fb9cdd2e439cc95e04e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:3-7-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:701d730eccece2f80759e801c8225629f7ec85aa019ce3f09371a2731289dea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357853162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31c95ba13ef81aabc6300e171e525a737317746e9003ade465cd6047655833a`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:25 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:05:25 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:05:25 GMT
ENV PYPY_VERSION=7.3.7
# Tue, 21 Dec 2021 03:10:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 21 Dec 2021 03:10:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 21 Dec 2021 03:10:16 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 21 Dec 2021 03:10:26 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Dec 2021 03:10:26 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9f74896dfa93fe0172f594faba85e0b4e8a0481a0fefd9112efc7e4d3c78f7`  
		Last Modified: Tue, 21 Dec 2021 02:02:33 GMT  
		Size: 196.5 MB (196510974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992152fe9d8d742097c12aff1df68f475e71a4cdde96311a5b827edfd224f7c0`  
		Last Modified: Tue, 21 Dec 2021 03:18:20 GMT  
		Size: 3.2 MB (3210066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b356ec08a845317e4e72a1bfba5d4606fad8b7fb368b0f7440c672175adf7bf8`  
		Last Modified: Tue, 21 Dec 2021 03:20:10 GMT  
		Size: 30.5 MB (30531271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f06075ebdfa182a59604c37292885e836cee79c27811ebeef8a189631a93b70`  
		Last Modified: Tue, 21 Dec 2021 03:20:04 GMT  
		Size: 2.1 MB (2090918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:e645aa952ddb5fd0b67e264b419fc8a75d5d02af0a9ad4e29ccbe7b3af88ca41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346444300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:373e32c3e8d8ee4ed08a54c69bb38d8039caf40d5cf4c7ab05969bfc5e91a7b9`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 08:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 08:30:48 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 08:30:49 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 08:30:50 GMT
ENV PYPY_VERSION=7.3.7
# Tue, 21 Dec 2021 08:34:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 21 Dec 2021 08:34:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 21 Dec 2021 08:34:55 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 21 Dec 2021 08:35:04 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Dec 2021 08:35:05 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb9078a4a2954fb77553c7f66912068fb62ff7cf431160389ebd36fab5c7ad`  
		Last Modified: Tue, 21 Dec 2021 02:23:30 GMT  
		Size: 189.4 MB (189424367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e132097b395c9373e4ee539eb76739088b50776e5316b72083fd32e3098b84`  
		Last Modified: Tue, 21 Dec 2021 08:43:45 GMT  
		Size: 3.0 MB (2973415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d59612135b0ff7e9aa0ff5f6723eac3c67f52b0e321a7ebd44b72d3f9e182f2`  
		Last Modified: Tue, 21 Dec 2021 08:45:31 GMT  
		Size: 27.9 MB (27884127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dc3f6edc16f56774192731f13fe7433c04401d3613fd53840804c82517eeed`  
		Last Modified: Tue, 21 Dec 2021 08:45:26 GMT  
		Size: 2.1 MB (2091460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:5fc7a22f92a3b9f33ee2db61be9467ddbc3ce16b6382e3d7db2d5bbe7db1c7a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.1 MB (361099782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09a3531d376071fbfb5923502cc7c7908ad6995a342af4f11ad54e0c2249785`
-	Default Command: `["pypy3"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:37 GMT
ADD file:0fd00a1dc1745744d1e95964f1f6fc73e016055aeec062f1946440b6ba68411d in / 
# Thu, 02 Dec 2021 02:39:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:10:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:11:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:12:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 15:06:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 15:06:49 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 15:06:49 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 15:06:50 GMT
ENV PYPY_VERSION=7.3.7
# Thu, 02 Dec 2021 15:12:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 02 Dec 2021 15:12:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 02 Dec 2021 15:12:02 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 02 Dec 2021 15:12:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 02 Dec 2021 15:12:10 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:3dfa4acb9eec45f56cd836373cf9bf145fb45d1ae4cbc3181c21d4d01d14037d`  
		Last Modified: Thu, 02 Dec 2021 02:47:22 GMT  
		Size: 55.9 MB (55937571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3245a08f8d7007d55bcf225301e2ba4bcbd38d83c944f9a0fe4ca5811ac6bf9f`  
		Last Modified: Thu, 02 Dec 2021 03:20:35 GMT  
		Size: 5.3 MB (5283147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff3b7dd8fe63a0512b577941dbb20701dc02abfdca700e55006d84c44cfc0e1`  
		Last Modified: Thu, 02 Dec 2021 03:20:35 GMT  
		Size: 11.3 MB (11250671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394078f1578cde892a871c190a95f65490ec769aa2c7aadf9d224b49f50f1a35`  
		Last Modified: Thu, 02 Dec 2021 03:21:05 GMT  
		Size: 55.9 MB (55917753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da24b680b80bb8e49e7a6655ea0c6a18d872049c9addcb70c96f44bb69190c`  
		Last Modified: Thu, 02 Dec 2021 03:21:57 GMT  
		Size: 199.4 MB (199412590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee406f69248eae98a834f4d4cf320850cda4940b8a069b608919118e2ce5051`  
		Last Modified: Thu, 02 Dec 2021 15:24:57 GMT  
		Size: 3.4 MB (3360216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b959155c71c5e1b5dc66070b4d2cc1b76c357232ad8f25989893c204f454f68c`  
		Last Modified: Thu, 02 Dec 2021 15:27:13 GMT  
		Size: 27.8 MB (27846908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb29653a3ed8c411cbe7cc965d2cb598864b34a1e67d9b97837ac6bbc4af27b`  
		Last Modified: Thu, 02 Dec 2021 15:27:06 GMT  
		Size: 2.1 MB (2090926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
