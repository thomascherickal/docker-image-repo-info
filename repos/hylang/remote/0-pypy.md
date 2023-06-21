## `hylang:0-pypy`

```console
$ docker pull hylang@sha256:031cf0ff7d5b32006d53407c22fa5277b9b6c7138c6c00b8c85e8743c3cb014e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `hylang:0-pypy` - linux; amd64

```console
$ docker pull hylang@sha256:a08850ceef0a4cf1d82807a9157329d4083c7c2a4beedf140a531571760202c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76261261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d75a9449ec3c013cabf402038b7581bbaa8b568ddcf75423bb88a398dd99afc6`
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
# Wed, 21 Jun 2023 01:24:53 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 21 Jun 2023 01:25:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 21 Jun 2023 01:25:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 21 Jun 2023 01:25:24 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 21 Jun 2023 01:25:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 21 Jun 2023 01:25:36 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 01:55:00 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 01:55:00 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 01:55:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 01:55:30 GMT
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
	-	`sha256:153507968beca23ab4c1c52be98b70a65b6b1ce2f04ca4d4bae32b87110ca269`  
		Last Modified: Wed, 21 Jun 2023 01:30:38 GMT  
		Size: 36.6 MB (36565754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67988b90ccb1574647475841b6c619c48f84c263a5418a09c2e59c97edd72c29`  
		Last Modified: Wed, 21 Jun 2023 01:30:33 GMT  
		Size: 3.1 MB (3123443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6aea752bcb8f5dc3fccc42736efabc6135c6f03930139056e9fb05c71e370f`  
		Last Modified: Wed, 21 Jun 2023 01:57:54 GMT  
		Size: 4.0 MB (3961943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b3663032a56b487e9af9579ac9c5600020d22e0c3d84a57ec31d56f4d1b4e77d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73413859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b181e94a3261d745eed123a0a721722795f7c9fb390d49caea6575bb56518a`
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
# Wed, 21 Jun 2023 01:32:45 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 21 Jun 2023 01:33:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 21 Jun 2023 01:33:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 21 Jun 2023 01:33:12 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 21 Jun 2023 01:33:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 21 Jun 2023 01:33:24 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 01:57:10 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 01:57:10 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 01:57:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 01:57:40 GMT
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
	-	`sha256:7a4b50b1827d14b5e5cd7ee5f378399c10f5f32aa1f661e55f1879178b34c68b`  
		Last Modified: Wed, 21 Jun 2023 01:37:46 GMT  
		Size: 33.9 MB (33864426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b56a4b3c212bc9303654b02a122807f2441e2825f2ccdada31e1421a31b45d`  
		Last Modified: Wed, 21 Jun 2023 01:37:42 GMT  
		Size: 3.1 MB (3123377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223d2688e7a22b8ee030e23af79470034a325817535fd62ee66a8f1606f3236`  
		Last Modified: Wed, 21 Jun 2023 01:59:59 GMT  
		Size: 4.0 MB (3961727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy` - linux; 386

```console
$ docker pull hylang@sha256:7e8d2c3eb1255f8255efa0f704c8c4d9181452916e584b5c916bfca48f64f810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73240625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267efcdbcaf0d8dbef51abb416bea7899f44e8498ddeb90dd01f1c90a3d53973`
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
# Wed, 21 Jun 2023 00:56:10 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 21 Jun 2023 00:56:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 21 Jun 2023 00:56:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 21 Jun 2023 00:56:46 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 21 Jun 2023 00:57:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 21 Jun 2023 00:57:00 GMT
CMD ["pypy3"]
# Wed, 21 Jun 2023 01:22:10 GMT
ENV HY_VERSION=0.26.0
# Wed, 21 Jun 2023 01:22:10 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 21 Jun 2023 01:22:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 21 Jun 2023 01:22:46 GMT
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
	-	`sha256:e9f2c8386abfc3d3f065a71e404e424d70f7a39a0b4443751b90499269a18ac2`  
		Last Modified: Wed, 21 Jun 2023 01:02:24 GMT  
		Size: 32.5 MB (32522341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645a0684c1be8f2049565d6aef5e34893fe79474a0279fe6bacf2451ca60c0a1`  
		Last Modified: Wed, 21 Jun 2023 01:02:18 GMT  
		Size: 3.1 MB (3123037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7258a35b5637159c5843cab1a523baa4126a8b7060d4d36535cbb4a4049eca`  
		Last Modified: Wed, 21 Jun 2023 01:25:23 GMT  
		Size: 4.0 MB (3961879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy` - windows version 10.0.20348.1787; amd64

```console
$ docker pull hylang@sha256:bbbb57f903d918151046309076ec7477be3fb0fc6ca2996c9fd916abfa7225a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1439209594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2060b9188a7f045606c5b0ec7aacd845356e84a5ffe9a4198f75a18edfa243`
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
# Wed, 14 Jun 2023 22:50:50 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '57faad132d42d3e7a6406fcffafffe0b4f390cf0e2966abb8090d073c6edf405'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:50:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 22:50:52 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 22:52:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:52:02 GMT
CMD ["pypy"]
# Wed, 14 Jun 2023 23:58:58 GMT
ENV HY_VERSION=0.26.0
# Wed, 14 Jun 2023 23:58:59 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 15 Jun 2023 00:01:29 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 15 Jun 2023 00:01:30 GMT
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
	-	`sha256:0b3c182b43c5921d2ff3437b88a9e02514188a74f397fb025602b005fc9a5026`  
		Last Modified: Wed, 14 Jun 2023 23:39:49 GMT  
		Size: 26.6 MB (26552400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b13f7a514f8b0030a11ef008daa88a292181d619255e9d281fb9030bafc6c8c`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22951c8822da1115237b996f794344bb115bdce82f91c7400b5d9824a14891b1`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3419bf96ca065d4875e75a1ee086ffdb60018be7f3a24ad8f0bc686aca3aea`  
		Last Modified: Wed, 14 Jun 2023 23:39:44 GMT  
		Size: 3.5 MB (3504564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a459b1ff6fe48419d4987b434e68214f8e2cbfca1f5cc0ca397f43260b1e3a2`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de229f166b0be8658965957d48823da825915a5ed66b1050c7654119e28b7f4`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8017a3bf355322e16d31fe6cea33b8e0a581ccbd8aae9927ca666b0f9704b9`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037e2803d629a6d03d3538c5cd974d74a78a113cf92c4c64cf2f34f13997bbb1`  
		Last Modified: Wed, 21 Jun 2023 01:16:08 GMT  
		Size: 4.8 MB (4775066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc6153b74bc0fd37bfc798e892b87e4175d2986083d2a1d187fd8107387ebe6`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy` - windows version 10.0.17763.4499; amd64

```console
$ docker pull hylang@sha256:ed0e3667de7631681ef6c8155aca662d39384ed86a945a74f30e98bb68e24e25
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1701134772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:121e8b65b1e8d0af2b5e5e8ce1639e9611feb474fa091bcf08c0eb8ccd115720`
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
# Wed, 14 Jun 2023 22:54:16 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '57faad132d42d3e7a6406fcffafffe0b4f390cf0e2966abb8090d073c6edf405'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:54:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 22:54:17 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 22:55:36 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:55:37 GMT
CMD ["pypy"]
# Thu, 15 Jun 2023 00:01:42 GMT
ENV HY_VERSION=0.26.0
# Thu, 15 Jun 2023 00:01:42 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 15 Jun 2023 00:04:15 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 15 Jun 2023 00:04:16 GMT
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
	-	`sha256:280a22ea3ff988726cb4ae2f78c994b30e591fc2b72f413602740397b1d4d95d`  
		Last Modified: Wed, 14 Jun 2023 23:40:20 GMT  
		Size: 26.6 MB (26558965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4211b19fb202b31af3ab7dd7a8b0afdbc9224756a4d44bd6b1a44cf0f38d85e5`  
		Last Modified: Wed, 14 Jun 2023 23:40:13 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63d72b09dd95dc9cb75fe72456fee4fe66d0624f5573adb22d3bcfda4c76fe3`  
		Last Modified: Wed, 14 Jun 2023 23:40:13 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d208697c304d738943817590e88b769db176d2adda57a932c874e15f072574`  
		Last Modified: Wed, 14 Jun 2023 23:40:15 GMT  
		Size: 3.5 MB (3504296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31635b86d554b4e2a997f2541befa9a69ae38ea1bb42a0aae900454377040eed`  
		Last Modified: Wed, 14 Jun 2023 23:40:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b8e37ebe5c676f2e6a2e62d9c2a543f1212bbffd7f2b09eeb02e4fad2a5af`  
		Last Modified: Wed, 21 Jun 2023 01:16:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af7256a3b5c9714567f6633117841b527cd4460cc5ae569129ae54b7af34a4d`  
		Last Modified: Wed, 21 Jun 2023 01:16:33 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95990eee1b44a4ea451ec46492219cdfae0d91c031531fcad83bf7fc82bbe864`  
		Last Modified: Wed, 21 Jun 2023 01:16:36 GMT  
		Size: 4.7 MB (4691267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a475e8e94987a09f47d2945592cfa8b7f7fb4567c3cef0424d5b0010a328d26`  
		Last Modified: Wed, 21 Jun 2023 01:16:33 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
