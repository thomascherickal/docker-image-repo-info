## `pypy:2-buster`

```console
$ docker pull pypy@sha256:18fe5b9c63921e79e4294f1dd7d62fb200e3ccc4b9044483247825a45e298f9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-buster` - linux; amd64

```console
$ docker pull pypy@sha256:f44c1d83951571f2e8d53311180aa1261b61e87f6e02f118212e434e97644c66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.5 MB (348503487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05f3d0a8be80f11df2069d266fc762cdc35fc02c4dff704e41ff795a79bd03b`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:30:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:31:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:32:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:33:48 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 16:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:33:54 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Nov 2020 00:56:11 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 24 Nov 2020 00:56:34 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1' ;; 		arm64) pypyArch='aarch64'; sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8' ;; 		i386) pypyArch='linux32'; sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 03 Dec 2020 22:33:22 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Thu, 03 Dec 2020 22:33:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Thu, 03 Dec 2020 22:33:22 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Thu, 03 Dec 2020 22:33:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 03 Dec 2020 22:33:34 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77915b4e630d47296770ce4cf481894885978072432456615172af463433cc5`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 7.8 MB (7811717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37a0a41b6b03489dd7de0aa2a79e369fd8b219bbc36b52f3f9790dc128e74b`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 10.0 MB (9996233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b2c1e36db5f5910f58da2ca4f9311b0690810c7107fb055ee1541498b5061f`  
		Last Modified: Wed, 18 Nov 2020 00:50:25 GMT  
		Size: 51.8 MB (51829318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c495e8de12d26c9843a7a2bf8c68de1e5652e66d80d9bc869279f9af6f86736a`  
		Last Modified: Wed, 18 Nov 2020 00:51:17 GMT  
		Size: 192.3 MB (192280841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8a1caff507f3f24faec8c88f34d8ba885acd8d0959647d3a2f984e2280a4f0`  
		Last Modified: Wed, 18 Nov 2020 16:39:51 GMT  
		Size: 3.2 MB (3188694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acee308ebbe2c347594b549e623f5ad8ab69d086328f90a6732a555c65c1b505`  
		Last Modified: Tue, 24 Nov 2020 01:01:54 GMT  
		Size: 31.0 MB (31035285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a983e51fa2ec81f140dfcbd54311f44cf60f678adfc0ba1631229d3fd44f329`  
		Last Modified: Thu, 03 Dec 2020 22:36:00 GMT  
		Size: 2.0 MB (1963674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-buster` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:73390932298a06f6e126a6a154f0e1fbba081f612d37a908582122d1c0ade685
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333924106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8653739172add391164f6ca451e5a79f8e49eb724369590878f0a90d2ab4b12d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:04 GMT
ADD file:28343d2066831f0ffb2002914f158698f92b4af6dc16ac22e3d8e9c388c688bb in / 
# Tue, 17 Nov 2020 20:23:05 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:20:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:21:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:24:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:12:40 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:12:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:12:52 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Nov 2020 01:00:33 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 24 Nov 2020 01:01:29 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1' ;; 		arm64) pypyArch='aarch64'; sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8' ;; 		i386) pypyArch='linux32'; sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 02 Dec 2020 00:26:19 GMT
ENV PYTHON_PIP_VERSION=20.3
# Wed, 02 Dec 2020 00:26:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2357a5f805565496648ebf597bcffe9e2d9ce379/get-pip.py
# Wed, 02 Dec 2020 00:26:21 GMT
ENV PYTHON_GET_PIP_SHA256=7f28b41ce236af61a00dfcbd6fd38c52d46488ece91fb4585b95775b076bbc85
# Wed, 02 Dec 2020 00:26:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 02 Dec 2020 00:26:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:22518ad4a7da48a5acd01946dad2fbee99e4fca910d23b78cd7e4a16c3bd1e5b`  
		Last Modified: Tue, 17 Nov 2020 20:31:35 GMT  
		Size: 49.2 MB (49179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed68dbf09ea059b44b3e1013706c78f868e5f07beb5f16780ca8f52aa9594a`  
		Last Modified: Tue, 17 Nov 2020 22:36:39 GMT  
		Size: 7.7 MB (7681805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeb09cb5ac2e2a9553920a21389f08df1b6b08c816ae4b8e60866d84119492`  
		Last Modified: Tue, 17 Nov 2020 22:36:38 GMT  
		Size: 10.0 MB (9984036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff17ea9ada38fca6de6d6808558e3c10793b90c2331b3481ad81f7c62293d8e6`  
		Last Modified: Tue, 17 Nov 2020 22:37:04 GMT  
		Size: 52.2 MB (52164616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dea92ecae615cf4291c3db4250413456b07575391a5e2b6db5ddfec7ce7a98`  
		Last Modified: Tue, 17 Nov 2020 22:37:59 GMT  
		Size: 183.8 MB (183814833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4ed184615d14415c5a5375bc214e087b000530fa003e0bbaf7083a8a741633`  
		Last Modified: Wed, 18 Nov 2020 06:23:31 GMT  
		Size: 3.2 MB (3195928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565582694b815ff90b82242278912f34a69471f144404367f2b916504bee280f`  
		Last Modified: Tue, 24 Nov 2020 01:11:28 GMT  
		Size: 25.9 MB (25939932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06da28548f68b9c7825c4a0d661c3c86d2041101d213cad81b6e702d927fb`  
		Last Modified: Wed, 02 Dec 2020 00:32:14 GMT  
		Size: 2.0 MB (1963741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-buster` - linux; 386

```console
$ docker pull pypy@sha256:b4b9aa11bd2b4d974975ea8e4e557f2e701c516e4e08bbc622d37fce367df859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355571887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3669ef59e1dbfa9f98342f999fae410ae3bbc4606629dd3508d86ded8b265cdf`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:39 GMT
ADD file:4805e11ec22df9454eb4759523111e031e84c8078bcaef178f089baca9e83cdb in / 
# Tue, 17 Nov 2020 20:19:40 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:06:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 03:11:42 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 03:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 03:11:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Nov 2020 00:49:20 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 24 Nov 2020 00:49:48 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1' ;; 		arm64) pypyArch='aarch64'; sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8' ;; 		i386) pypyArch='linux32'; sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy' '/usr/local/bin/pypy'; 		pypy --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		pypy _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 02 Dec 2020 00:06:41 GMT
ENV PYTHON_PIP_VERSION=20.3
# Wed, 02 Dec 2020 00:06:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2357a5f805565496648ebf597bcffe9e2d9ce379/get-pip.py
# Wed, 02 Dec 2020 00:06:42 GMT
ENV PYTHON_GET_PIP_SHA256=7f28b41ce236af61a00dfcbd6fd38c52d46488ece91fb4585b95775b076bbc85
# Wed, 02 Dec 2020 00:06:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 02 Dec 2020 00:06:55 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:21c39c42a8e082b1b164b44e463e4752c74821dbc51451f2ac2518ae6f29dff3`  
		Last Modified: Tue, 17 Nov 2020 20:26:25 GMT  
		Size: 51.2 MB (51159492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afab7b21aa8cddd140983ed21a34965621db1efb35f635bc756479b30c3deaf3`  
		Last Modified: Tue, 17 Nov 2020 21:23:47 GMT  
		Size: 8.0 MB (7981231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a1ce1fcda982662c6c9be38bac7b53e9fd405b0b367fa902cfd957be683731`  
		Last Modified: Tue, 17 Nov 2020 21:23:46 GMT  
		Size: 10.3 MB (10338498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a190a57cc81d3d40833225fd0b5e6bf1d793a9c09ba842367e28f584fc4ab5e7`  
		Last Modified: Tue, 17 Nov 2020 21:24:09 GMT  
		Size: 53.4 MB (53433407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc286fe391b261bbe537e32cbd0af32f46ca3385b255004c032a0f243990cb02`  
		Last Modified: Tue, 17 Nov 2020 21:25:08 GMT  
		Size: 198.8 MB (198839681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d5e40f61612fb86d43e02667465d35d51bdc4a5d8c09d702cc3431b6e1dd4e`  
		Last Modified: Wed, 18 Nov 2020 03:20:37 GMT  
		Size: 3.3 MB (3328684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3458a944b5f8c7551fa5d1f50c29912ed84eb2fdc7d71830ac2e4a420343884a`  
		Last Modified: Tue, 24 Nov 2020 00:56:13 GMT  
		Size: 28.5 MB (28527440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8cd3e87753597ce821378f7939c42b99b7d45154b23cd16e3bc27b72f2e3d`  
		Last Modified: Wed, 02 Dec 2020 00:09:39 GMT  
		Size: 2.0 MB (1963454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
