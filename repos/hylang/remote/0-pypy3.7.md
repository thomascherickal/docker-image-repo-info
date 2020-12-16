## `hylang:0-pypy3.7`

```console
$ docker pull hylang@sha256:359cb6d18732bf30682fc6cc646991e2bf51913d2d887219d940d30105cf32b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:0-pypy3.7` - linux; amd64

```console
$ docker pull hylang@sha256:45a491773bffd434966b11262af7e802f5deb86db8da2b55ac52ac977a0ee3b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73535769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9921c7b164012c8b6f13c501b931de08b14c0a82e225b964821ec34308674f5c`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:21:03 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 19:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:21:10 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 19:21:10 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 19:23:30 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 22:26:59 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:26:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:27:00 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:27:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:27:16 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 22:48:20 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 22:48:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 22:48:31 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862ff65907287da7787a1512d3d8837f7bea201508670fdaa8a0edbd815e629c`  
		Last Modified: Fri, 11 Dec 2020 19:25:08 GMT  
		Size: 2.7 MB (2742693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83859391cf7b2c2de532cf27acf6f75490dfaa8ca8a2b12107636c70a5c3f335`  
		Last Modified: Fri, 11 Dec 2020 19:26:21 GMT  
		Size: 38.1 MB (38052590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e065b4871017256400133a2e7c909b1431d67d0632e80a174858a089a54373`  
		Last Modified: Tue, 15 Dec 2020 22:30:43 GMT  
		Size: 2.6 MB (2564378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7225de16de7d16d748143e5d41bec418d2d70986acd9436ef7bfe9910ec3fe35`  
		Last Modified: Tue, 15 Dec 2020 22:52:13 GMT  
		Size: 3.1 MB (3076813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a22240478b34701b2aa2c0e4d47d97b8f5803e276eb31bde5368c088b4b2afbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65926322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cf91a301c773bebe4023f7b3fea12c0dde7ad38ea276a0443942dbd75b49c6`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:52:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:52:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:52:31 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 16:58:02 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 22:48:55 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:48:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:48:58 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:49:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:49:41 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 23:17:05 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:17:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:17:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f827548d2e9ffb879dc53392f8b6e3b31acc4faef6c0274f311cee165c7492f6`  
		Last Modified: Fri, 11 Dec 2020 17:00:07 GMT  
		Size: 2.6 MB (2606496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d2a3568588f414c8fc12cc4f6fd5f014d7e764adca66055acf25b29e82333b`  
		Last Modified: Fri, 11 Dec 2020 17:02:01 GMT  
		Size: 31.8 MB (31819922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0558efe3327bc9cb12b13c295c641fbf200cd14f4ba2e7238604aa6f9bfeafe1`  
		Last Modified: Tue, 15 Dec 2020 22:53:28 GMT  
		Size: 2.6 MB (2565634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237989ebcbc2258eb587652cd20028ccc48ca551ab621f879ccd6b7b0cdaf635`  
		Last Modified: Tue, 15 Dec 2020 23:22:24 GMT  
		Size: 3.1 MB (3078079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; 386

```console
$ docker pull hylang@sha256:c92a845f1bb973c5616f20c5b5d3e7a2868269f4b3cef177880e69f7a27af62f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76505155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1198e42ec0b6a98767ce9b63f2bd0a1fcc2c160014ff399f5166b3e179b184d4`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 22:18:45 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 22:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 22:18:55 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 22:18:55 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 22:23:26 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 23:03:50 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 23:03:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 23:03:51 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 23:04:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 23:04:09 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 23:46:20 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:46:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:46:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afc78f63aaea6458a1464eb07ba0cdb68d083175bebee11d5d502b846e12b1a`  
		Last Modified: Fri, 11 Dec 2020 22:25:40 GMT  
		Size: 2.8 MB (2752978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca50cd1e9ae97c73203c8992d37da329ae8617326d3fc8b5691a14858ac1efcf`  
		Last Modified: Fri, 11 Dec 2020 22:28:04 GMT  
		Size: 40.4 MB (40353572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c899c94458b0e0fc0530cdd6c54ab7925415547719cb48cc08850a19334becc7`  
		Last Modified: Tue, 15 Dec 2020 23:06:58 GMT  
		Size: 2.6 MB (2564116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666cc26301fca5a4b9eec5c8be9298c2fb3774c1ba2f2e499adf41d9b100f5f`  
		Last Modified: Tue, 15 Dec 2020 23:50:11 GMT  
		Size: 3.1 MB (3076905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; s390x

```console
$ docker pull hylang@sha256:568d9a953db1a790eef48625f533f7089fd30d54626a4f7c2df8fa3934531084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68827944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c989755040c0195e4541884716e32fa0e871cc3401b92c19a6ee27e1473402`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:19:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:20:01 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:20:02 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 16:23:11 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 21:44:33 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 21:44:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 21:44:34 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 21:44:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 21:44:49 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 22:03:41 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 22:03:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 22:03:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1873488019a5a723e31f96e4bfefafcfd2bf9df4c7cbd724308f1aaaa9205d3`  
		Last Modified: Fri, 11 Dec 2020 16:25:26 GMT  
		Size: 2.4 MB (2432982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889cd00615313a288f1af7c730a019b4fd04ad3da2906b5b3d3eb819926e660a`  
		Last Modified: Fri, 11 Dec 2020 16:26:35 GMT  
		Size: 35.0 MB (35038765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f501d9520ceb13d21d55b0b6d89eb55e570672cf93367e0c0f577a9d925b47`  
		Last Modified: Tue, 15 Dec 2020 21:47:09 GMT  
		Size: 2.6 MB (2564845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe48569b652bd324b65ed22fcdcbd90f00c5693b2d5468169a30fa0058ea71`  
		Last Modified: Tue, 15 Dec 2020 22:06:06 GMT  
		Size: 3.1 MB (3077395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
