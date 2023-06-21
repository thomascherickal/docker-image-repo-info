## `hylang:pypy3.8`

```console
$ docker pull hylang@sha256:ddddd364819190a04be4135b28631237846f64f1aa71f62c740d6327ada9b2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `hylang:pypy3.8` - linux; amd64

```console
$ docker pull hylang@sha256:355b69586435efb3666549d182abf884436a29c5b20241237b8b871809a6117c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76378202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d8647b30a6792d045a5f342b0fe63affcea871bd39d4880132ec21adaac32c`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:55:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:55:15 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 20:55:15 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 20:55:15 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 14 Jun 2023 20:58:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 14 Jun 2023 20:58:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 20:58:30 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 20:58:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 14 Jun 2023 20:58:41 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 00:55:11 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 00:55:11 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 00:55:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 00:55:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300d2277cd75a1d6b904cd75deb1cd324e9951dfe2703c2d2b9b9650325efed2`  
		Last Modified: Wed, 14 Jun 2023 21:03:29 GMT  
		Size: 3.5 MB (3485377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b311c27a25d088c22b856176830a88bb98224018eb399ad0822c29b72c7ebeb`  
		Last Modified: Wed, 14 Jun 2023 21:05:34 GMT  
		Size: 36.4 MB (36422526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a78797110a36f4f2f00a71dfcb3c710f748f144191366ee36cac522ac0b6ae`  
		Last Modified: Wed, 14 Jun 2023 21:05:29 GMT  
		Size: 3.2 MB (3187811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c4f968f5efaae15af386c578bc6679c800bc31b2fe10d7767338a45c8402e0`  
		Last Modified: Wed, 21 Jun 2023 00:59:51 GMT  
		Size: 4.2 MB (4157744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a89b42e508665c71f59318d9e2f4f32dfaf7550a40aa6313c1480c51e82fc4de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73495116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e065e9206b563a6cbb6f0f6aa59f69857d2e3ab7ec7d378b825973388f2d7f9b`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 21:37:54 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 21:37:54 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 21:37:54 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 14 Jun 2023 21:40:58 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 14 Jun 2023 21:40:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 21:40:59 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 21:41:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 14 Jun 2023 21:41:10 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 00:56:21 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 00:56:21 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 00:56:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 00:56:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71529976e8b0cd7b9e5e20b5f6a18c7985df33fcbd850418bb8c62d3c08db365`  
		Last Modified: Wed, 14 Jun 2023 21:45:16 GMT  
		Size: 3.3 MB (3311795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c925fddc4f8d6815ab7394ac44b1033e86a0a6425b3c8c7dc036f216c7a2add`  
		Last Modified: Wed, 14 Jun 2023 21:47:09 GMT  
		Size: 33.7 MB (33685247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3078ba59c410c395f0323d29810bfbbf790757e6b0e3bc1d23d792895365118`  
		Last Modified: Wed, 14 Jun 2023 21:47:05 GMT  
		Size: 3.2 MB (3187587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0e65de42ea31d4ac4379028bca3e91ad3bc35377bd1e8a7fa6647f4ef430d1`  
		Last Modified: Wed, 21 Jun 2023 01:00:52 GMT  
		Size: 4.2 MB (4157953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; 386

```console
$ docker pull hylang@sha256:19083c862e313b2c8c094e7adbbc71e5c60c75ba929c49eb96d284c2115f783c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73329132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a02ad20eb9059823fbe9b4dce61640414fafd3ee4caeb7b88a83d20e3f0c07`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 01:30:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 15 Jun 2023 01:30:34 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 01:30:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 01:30:34 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 15 Jun 2023 01:34:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 15 Jun 2023 01:34:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 15 Jun 2023 01:34:30 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 15 Jun 2023 01:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 15 Jun 2023 01:34:44 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 00:41:16 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 00:41:16 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 00:41:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 00:41:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb43f3f858bc03cbd60af609f87d15e19c451bfa296f791a956bee0ad15c25f`  
		Last Modified: Thu, 15 Jun 2023 01:39:58 GMT  
		Size: 3.5 MB (3492627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c6554dccf2085963898d2b84553e78f6e289bc815009486f4541fd1e7aaea9`  
		Last Modified: Thu, 15 Jun 2023 01:42:10 GMT  
		Size: 32.4 MB (32351041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc380aed151f040d1215a227852b7787a2e1d8419dfbb0ab8c84b61c495a3886`  
		Last Modified: Thu, 15 Jun 2023 01:42:01 GMT  
		Size: 3.2 MB (3187300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eaa7cd2869b37575e6282b02c48e993521cdda89db33780dfc37253baedb863`  
		Last Modified: Wed, 21 Jun 2023 00:46:06 GMT  
		Size: 4.2 MB (4157423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.20348.1787; amd64

```console
$ docker pull hylang@sha256:d40604727deb57ea9ecf81f0505def6aaced64bde0263da966ed2b07d1945ac0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1438998644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd0bfba1f9b2f95d957660a77694a6e7fed303574d3dddeee93dc9d3aa593c5`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 22:49:27 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:49:59 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:50:00 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 14 Jun 2023 22:56:38 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0f46fb6df32941ea016f77cfd7e9b426d5ac25a2af2453414df66103941c8435'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:56:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 22:56:39 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 22:57:52 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:57:53 GMT
CMD ["pypy3"]
# Thu, 15 Jun 2023 00:04:26 GMT
ENV HY_VERSION=0.26.0
# Thu, 15 Jun 2023 00:04:27 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 15 Jun 2023 00:06:43 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 15 Jun 2023 00:06:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494928dc22760e844729c73d3630dffe1d8a58b5cb4f07f51aa050220ccbb022`  
		Last Modified: Wed, 14 Jun 2023 23:39:45 GMT  
		Size: 315.4 KB (315438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47cea0a370519618fc87381c6251f61791e86d8479636a8d529614016877f8d`  
		Last Modified: Wed, 14 Jun 2023 23:39:48 GMT  
		Size: 15.5 MB (15452954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb49b84e7d71577b27e21ef90de124e68b909b72f4e03f0a281c84cdf165d0a0`  
		Last Modified: Wed, 14 Jun 2023 23:39:45 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f89cc18ebc214a4e1357b4b265ea0f73014ae564b120b3576ad3463694e13ce`  
		Last Modified: Wed, 14 Jun 2023 23:40:57 GMT  
		Size: 26.3 MB (26329135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a416f139e46a10f2db3bfcfe8b8725b5dc3f23826942e07f802f07429223cc39`  
		Last Modified: Wed, 14 Jun 2023 23:40:50 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4639ba2efe66bacf495704afb5c7ef210209731947450dab1f719f9c694ef393`  
		Last Modified: Wed, 14 Jun 2023 23:40:50 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffca86fa62615aea61331972b5a419691018b8e87bb684b9c836e93221238be`  
		Last Modified: Wed, 14 Jun 2023 23:40:52 GMT  
		Size: 3.5 MB (3504792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390c105f6573274592735bda080e9be560abfea595cc905d0c394ad14918613d`  
		Last Modified: Wed, 14 Jun 2023 23:40:50 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9f2dc139bb89a6e971140914925304625a0616eb7056a88cb30e9510b1268`  
		Last Modified: Wed, 21 Jun 2023 01:17:02 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df3adfc723c323c862dc14ce89aaac947d92a162705fe749c211a44e5fe5361`  
		Last Modified: Wed, 21 Jun 2023 01:17:02 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd97cd2c6ddc6ebd785c336e19e1ceaca787e9105628031285d35f3d7a8905f`  
		Last Modified: Wed, 21 Jun 2023 01:17:04 GMT  
		Size: 4.8 MB (4786834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512525827cbacfbed0b53d3f502c9ee7be5d78678482b589c951c3fa9d4ca13`  
		Last Modified: Wed, 21 Jun 2023 01:17:02 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.17763.4499; amd64

```console
$ docker pull hylang@sha256:fe9d0685bee59189524478a92616316d3e95eec77c8b46a023c7127c6f2e88a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1700985469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d224249ea1844602a3d524a6c92a918438e0796d7981fd950a5faaceb7e814`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 22:52:43 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:53:17 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:53:18 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 14 Jun 2023 22:59:13 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0f46fb6df32941ea016f77cfd7e9b426d5ac25a2af2453414df66103941c8435'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:59:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 22:59:14 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 23:00:35 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 23:00:36 GMT
CMD ["pypy3"]
# Thu, 15 Jun 2023 00:06:55 GMT
ENV HY_VERSION=0.26.0
# Thu, 15 Jun 2023 00:06:55 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 15 Jun 2023 00:09:15 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 15 Jun 2023 00:09:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd8bba71467317133b651d8ced8232817e9aa21925796df61a723a189e4d345`  
		Last Modified: Wed, 14 Jun 2023 23:40:17 GMT  
		Size: 308.5 KB (308462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239faf32d496ebb6cd7586e3e2144029298236c13845400a487856b7c4c6bfa5`  
		Last Modified: Wed, 14 Jun 2023 23:40:27 GMT  
		Size: 15.4 MB (15440399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f32884c9d9d9b0a842390f04b9842838c373ba536ac22e7b56461f4fe8b6e8`  
		Last Modified: Wed, 14 Jun 2023 23:40:16 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e61d162fbbd4e9f31b8f03115db296c2de8400a5edc294576582f0c1e35726`  
		Last Modified: Wed, 14 Jun 2023 23:41:16 GMT  
		Size: 26.3 MB (26331048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa98f82646aa193f13e6615158d172c2d837f79b39978e6af78488bca81c590b`  
		Last Modified: Wed, 14 Jun 2023 23:41:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a59135c43d841ffcc88d09e56a729c79f22d2c2c68d7c94d11fb6ebab7e5d53`  
		Last Modified: Wed, 14 Jun 2023 23:41:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21572a0e995eb62735b70c4f2ce3c37a1da898b6638ab020762984c0668c5b3`  
		Last Modified: Wed, 14 Jun 2023 23:41:11 GMT  
		Size: 3.5 MB (3504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752aff2d31733e850f6eed57b4be4509ea2869410a7c820454868598cdb29324`  
		Last Modified: Wed, 14 Jun 2023 23:41:10 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d79df005b917eb4b74c920f063c75c027ceb62475d17f3607929575c8a3468`  
		Last Modified: Wed, 21 Jun 2023 01:17:18 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f822515e9fa903a07451623e069c78a93d11e813647a4159564022d6dbe9a0a5`  
		Last Modified: Wed, 21 Jun 2023 01:17:19 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f941eb5aab8d3f7e3726dc17fac3824f3d1123ac269134fd24744e119284b3fc`  
		Last Modified: Wed, 21 Jun 2023 01:17:21 GMT  
		Size: 4.8 MB (4770032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2cb583e4922c32ce54d6d03bdc8feeb6b1b3e335bf877b44edb5f47614867e`  
		Last Modified: Wed, 21 Jun 2023 01:17:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
