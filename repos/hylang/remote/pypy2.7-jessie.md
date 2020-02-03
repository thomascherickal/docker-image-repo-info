## `hylang:pypy2.7-jessie`

```console
$ docker pull hylang@sha256:d58c1259b850c34c371693a29661dbf010bf278ebecbf3647e5f40a077f5efe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `hylang:pypy2.7-jessie` - linux; amd64

```console
$ docker pull hylang@sha256:7b1239450894d9b6e41a2f2bfb5099efff0f041bcfebc958cef2d45aa78ed965
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72515998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b7637b48f1a65a21e113072ede32ab45340417bc0a6ba407c19995deec618c5`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:22 GMT
ADD file:7bddae780bfc4ce751148aec0e77e665e08c4c031b4e054a9f6b0e9920498285 in / 
# Sat, 01 Feb 2020 17:21:22 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:41:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:41:12 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:43:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:43:03 GMT
ENV PYPY_VERSION=7.3.0
# Sun, 02 Feb 2020 06:47:33 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f4950a54378ac637da2a6defa52d6ffed96af12fcd5d74e1182fb834883c9826' ;; 		arm64) pypyArch='aarch64'; sha256='a3dd8d5e2a656849fa344dce4679d854a19bc4a096a0cf62b46a1be127a5d56c' ;; 		i386) pypyArch='linux32'; sha256='eac1308b7d523003a5f6d20f58406d52ab14611bcec750122ae513a5a35110db' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		cd /usr/local/lib_pypy; 		pypy _ssl_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sun, 02 Feb 2020 06:47:34 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Sun, 02 Feb 2020 06:47:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sun, 02 Feb 2020 06:47:34 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sun, 02 Feb 2020 06:50:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 02 Feb 2020 06:50:11 GMT
CMD ["pypy"]
# Sun, 02 Feb 2020 22:55:52 GMT
ENV HY_VERSION=0.17.0
# Sun, 02 Feb 2020 22:55:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sun, 02 Feb 2020 22:55:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6f2295d35e78f75bc28bbc7b81c7a49bcc54eea446127fc14035418dd3d32456`  
		Last Modified: Sat, 01 Feb 2020 17:26:47 GMT  
		Size: 30.2 MB (30159539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd6b2a8a21502c7db0a2909ec8d9f240cd32b9abe839e6fbfd415ab3d11be15`  
		Last Modified: Sun, 02 Feb 2020 06:53:40 GMT  
		Size: 2.8 MB (2811858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d75e6a0ad096240d08d2281327e8dcd4d0a608ca84317331e2c653b81012d5`  
		Last Modified: Sun, 02 Feb 2020 06:53:50 GMT  
		Size: 34.8 MB (34833855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fb5bc444423164615ee05a14ba82b233cb36b705c13fb8c47cb1c07ca23e31`  
		Last Modified: Sun, 02 Feb 2020 06:53:40 GMT  
		Size: 2.2 MB (2183507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c470c608c4607cbe0a716391c29f5ea3d97b3c42514dc6e18983c2a01d239a`  
		Last Modified: Sun, 02 Feb 2020 22:57:23 GMT  
		Size: 2.5 MB (2527239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy2.7-jessie` - linux; 386

```console
$ docker pull hylang@sha256:cdf0d5eeb7fe760c780daad40ec72439c4331a6e0d36b6ff9b8ef06de59c2c58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74724171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f0ef7758ea14de268eb627e74d692314175fb18df018346562c30de18a75a05`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:59 GMT
ADD file:a8397e82c28512af775407c4f2370040b396f90e7de9b2d0eee7115b55903558 in / 
# Sat, 01 Feb 2020 16:39:59 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 04:35:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 04:35:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 04:38:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 04:38:41 GMT
ENV PYPY_VERSION=7.3.0
# Sun, 02 Feb 2020 04:45:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f4950a54378ac637da2a6defa52d6ffed96af12fcd5d74e1182fb834883c9826' ;; 		arm64) pypyArch='aarch64'; sha256='a3dd8d5e2a656849fa344dce4679d854a19bc4a096a0cf62b46a1be127a5d56c' ;; 		i386) pypyArch='linux32'; sha256='eac1308b7d523003a5f6d20f58406d52ab14611bcec750122ae513a5a35110db' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		cd /usr/local/lib_pypy; 		pypy _ssl_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sun, 02 Feb 2020 04:45:39 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Sun, 02 Feb 2020 04:45:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sun, 02 Feb 2020 04:45:39 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sun, 02 Feb 2020 04:49:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 02 Feb 2020 04:49:36 GMT
CMD ["pypy"]
# Sun, 02 Feb 2020 11:17:05 GMT
ENV HY_VERSION=0.17.0
# Sun, 02 Feb 2020 11:17:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sun, 02 Feb 2020 11:17:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3d294f17d11f8a748c70456b50961ca0b6b088d8a042fc72d556228e232aaa28`  
		Last Modified: Sat, 01 Feb 2020 16:45:04 GMT  
		Size: 30.3 MB (30304698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208a5790dd0801e3be21b4a4bbb450a26e96986fb9e0ef5d67f535538c28ed9c`  
		Last Modified: Sun, 02 Feb 2020 04:53:49 GMT  
		Size: 4.9 MB (4919991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b90b372fead610d33f30084830c7243864c1015a7dc902ee06e11d623d5248`  
		Last Modified: Sun, 02 Feb 2020 04:54:03 GMT  
		Size: 34.8 MB (34788697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4153661e6a27c02511bb4bafdad4defdb7d42ee74414dffef31b301d407f80`  
		Last Modified: Sun, 02 Feb 2020 04:53:48 GMT  
		Size: 2.2 MB (2183515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c9063eee0209c356dd29369bc4ccf9043747e4ceec4b02121bf50deb5a1e03`  
		Last Modified: Sun, 02 Feb 2020 11:18:54 GMT  
		Size: 2.5 MB (2527270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
