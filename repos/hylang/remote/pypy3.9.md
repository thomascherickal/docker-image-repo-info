## `hylang:pypy3.9`

```console
$ docker pull hylang@sha256:4cf0f2eb1490de5cba24624a238d827216e17f5ba36d7abfb817f707378ecdf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1906; amd64
	-	windows version 10.0.17763.4737; amd64

### `hylang:pypy3.9` - linux; amd64

```console
$ docker pull hylang@sha256:d3e8dfc8f4682a7f1dd7aa1051902d3f53b85726ddbe8a70de6ec55f87a7dbd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76216675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c34d0d499f8ad43fa416a9308a5efc48ea55d71a19950a9de387c6069dfcad1`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:31:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:31:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:31:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 10:31:31 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 16 Aug 2023 10:35:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 16 Aug 2023 10:35:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 16 Aug 2023 10:35:07 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 16 Aug 2023 10:35:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 16 Aug 2023 10:35:18 GMT
CMD ["pypy3"]
# Thu, 17 Aug 2023 02:59:08 GMT
ENV HY_VERSION=0.27.0
# Thu, 17 Aug 2023 02:59:08 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 17 Aug 2023 02:59:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Aug 2023 02:59:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a72649acb39c388918aa15e01bb40af874f5740fd074baf9ffa60afbb2d0712`  
		Last Modified: Wed, 16 Aug 2023 10:39:45 GMT  
		Size: 3.5 MB (3485427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef286781c7d3dd3c0360b6b38154c8a18659cd0790003669d0bbd85b4d45179`  
		Last Modified: Wed, 16 Aug 2023 10:41:43 GMT  
		Size: 36.6 MB (36566841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b0cf5572ef4f9256c38450e906dc26ac742bbb6e68cc6ac1ca0a59d27e4a79f`  
		Last Modified: Wed, 16 Aug 2023 10:41:38 GMT  
		Size: 3.1 MB (3123905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180ef4960834b14f58d7dd974435567553d00a6054a41a157b6819115ddab09b`  
		Last Modified: Thu, 17 Aug 2023 03:05:37 GMT  
		Size: 3.9 MB (3915939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d8f845538b92484c1b9cad32c39a99abd8a5b59d740412f842933ad745eb6478
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73375472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d532263f5ec9aa57fd7817f2112782156c622522b602633a9669cbfe4623e248`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:39 GMT
ADD file:fb5c8f411c4a1e06c25ac32455221938386907d0b4782fc228ca67de63a7e9de in / 
# Thu, 07 Sep 2023 00:39:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:24:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:24:09 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:24:09 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 02:24:09 GMT
ENV PYPY_VERSION=7.3.12
# Thu, 07 Sep 2023 02:26:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 07 Sep 2023 02:26:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 07 Sep 2023 02:26:12 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 07 Sep 2023 02:26:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Sep 2023 02:26:23 GMT
CMD ["pypy3"]
# Thu, 07 Sep 2023 10:08:15 GMT
ENV HY_VERSION=0.27.0
# Thu, 07 Sep 2023 10:08:15 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 07 Sep 2023 10:08:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 07 Sep 2023 10:08:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:155eab17d86c47443adc8cebe7fc62c847c03db8cfb1ca53aa6276564fff23ef`  
		Last Modified: Thu, 07 Sep 2023 00:43:02 GMT  
		Size: 29.2 MB (29157149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450177799d94d0e15598ad58df1aac449e9fb7b62946be3b09a6a44b243bdf7`  
		Last Modified: Thu, 07 Sep 2023 02:28:58 GMT  
		Size: 3.3 MB (3311913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263305ebf1a9eb6a6ee75219d6a8ee76f3083aafa3795f6e738830a38d0319eb`  
		Last Modified: Thu, 07 Sep 2023 02:30:15 GMT  
		Size: 33.9 MB (33866619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa6b554a97a8c82f18edb2c876b236b2174b4dae7ea0588f15d2c8c9a9592fc`  
		Last Modified: Thu, 07 Sep 2023 02:30:10 GMT  
		Size: 3.1 MB (3123920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f4b9268470783381f32c0beb0a913668ca5e2ad35922923a9d9ac5349469b0`  
		Last Modified: Thu, 07 Sep 2023 10:14:42 GMT  
		Size: 3.9 MB (3915871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; 386

```console
$ docker pull hylang@sha256:51cb6646d572813632fdf7e8dd81ddab69ef598fbe73554fc4de38f880d3678f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73197337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5d40630dbcba0830a381218f3b89c938bf3e91e06d5664e1a36d4ad833d088`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:47:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 07:47:15 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 07:47:15 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 07:47:15 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 16 Aug 2023 07:51:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux64.tar.bz2'; 			sha256='84c89b966fab2b58f451a482ee30ca7fec3350435bd0b9614615c61dc6da2390'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-aarch64.tar.bz2'; 			sha256='e9327fb9edaf2ad91935d5b8563ec5ff24193bddb175c1acaaf772c025af1824'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-linux32.tar.bz2'; 			sha256='aa04370d38f451683ccc817d76c2b3e0f471dbb879e0bd618d9affbdc9cd37a4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.12-s390x.tar.bz2'; 			sha256='20d84658a6899bdd2ca35b00ead33a2f56cff2c40dce1af630466d27952f6d4f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 16 Aug 2023 07:51:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 16 Aug 2023 07:51:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 16 Aug 2023 07:51:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 16 Aug 2023 07:51:33 GMT
CMD ["pypy3"]
# Wed, 16 Aug 2023 16:48:23 GMT
ENV HY_VERSION=0.27.0
# Wed, 16 Aug 2023 16:48:23 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 16 Aug 2023 16:48:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Aug 2023 16:48:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2219e3eeb706ebd934e6fe4fcd4428f6931908beb1fc6be6aa12fcb077d46b`  
		Last Modified: Wed, 16 Aug 2023 07:56:34 GMT  
		Size: 3.5 MB (3492671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b89a0544799540dda6fa86f57d5d112d292d714fb96fdbab9c91ebc174486`  
		Last Modified: Wed, 16 Aug 2023 07:58:46 GMT  
		Size: 32.5 MB (32523683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f74ada2e2f8a47849735583d71e46d89e53791d26e3963e3a2950bc9477fd8`  
		Last Modified: Wed, 16 Aug 2023 07:58:39 GMT  
		Size: 3.1 MB (3123325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb55131f335aafdcc0c4e4b0dfabc2c98e1666d0315085a5beb97e1b9653cd1`  
		Last Modified: Wed, 16 Aug 2023 16:52:38 GMT  
		Size: 3.9 MB (3915835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.20348.1906; amd64

```console
$ docker pull hylang@sha256:576cc86d2fb0eb3e5b6987151b2ee03bf67bd6ca44c45469abcb08406516c3db
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1847757218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e3acc4b45ce75503db2fb2188cdca7390c6950f9a9d577da916f46d7964729`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 05:22:27 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:22:58 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:22:59 GMT
ENV PYPY_VERSION=7.3.12
# Thu, 10 Aug 2023 05:32:10 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.12-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0996054207b401aeacace1aa11bad82cfcb463838a1603c5f263626c47bbe0e6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.12-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:32:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 10 Aug 2023 05:32:12 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 10 Aug 2023 05:33:22 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:33:23 GMT
CMD ["pypy"]
# Thu, 10 Aug 2023 06:10:39 GMT
ENV HY_VERSION=0.27.0
# Thu, 10 Aug 2023 06:10:40 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 10 Aug 2023 06:12:50 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 10 Aug 2023 06:12:51 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415a6fbf8e55472821900ce6c840525e1f358b82286ea29ad7e1a506e6e64ff`  
		Last Modified: Thu, 10 Aug 2023 05:46:03 GMT  
		Size: 450.4 KB (450422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efafffd12f3ea787c1eaf80bf8d2bf659ff854b59a0f4b02c313c6a7ed9979a`  
		Last Modified: Thu, 10 Aug 2023 05:46:04 GMT  
		Size: 15.5 MB (15451502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632655f71273e7a184ddcb5c8632ed8ce1cf82a522c6f174a0c1705e1b5e3977`  
		Last Modified: Thu, 10 Aug 2023 05:46:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199a0948cf4bda754d6d4e1188d5f94403bf4522c8d5ba0238ec1a5376541e4f`  
		Last Modified: Thu, 10 Aug 2023 05:47:11 GMT  
		Size: 26.5 MB (26496913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcaeef4d4ec9ce224144d963d9c51420196d6852d3fed1d2f6c7e2befb3ded`  
		Last Modified: Thu, 10 Aug 2023 05:47:04 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9b5faa104a6584a229c2aaa839ab879dfc637dac7aec4107f2e9aae445484a`  
		Last Modified: Thu, 10 Aug 2023 05:47:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fdf50bedc49a31c23c7f8a7d342b48ceab348905855baadec83adfef0cf2f2`  
		Last Modified: Thu, 10 Aug 2023 05:47:06 GMT  
		Size: 3.4 MB (3437988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380592aaa70529f07d257a05223300105fd3bce578f2c7b28d2ad165c1761917`  
		Last Modified: Thu, 10 Aug 2023 05:47:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15e6a1c6aaf87c7ad657b1a4e65d6c7b1d3ba55847cc35c40c02f730acb47f0`  
		Last Modified: Thu, 10 Aug 2023 06:16:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4769a7c0419ac4f2f78b90d738c3e09c5fd234e26ecebed9f870d8e5259c66d9`  
		Last Modified: Thu, 10 Aug 2023 06:16:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff66494003ae4ec7c0066cfe529045b5f2597e7e184d5224284a842b9f6f5e4`  
		Last Modified: Thu, 10 Aug 2023 06:16:07 GMT  
		Size: 4.5 MB (4545163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6846d31333d0ad8e5c55778ceb61a094613e9d8ef56b9f7307a01c22ed517608`  
		Last Modified: Thu, 10 Aug 2023 06:16:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.17763.4737; amd64

```console
$ docker pull hylang@sha256:e7ab6dbf15e3f855dce98c92391a864c3cc7409ae6e8d8cc9ee77c6a98999afe
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2046326155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ee8faffc94fb8386e08954f75e98dbbc6b5d7a687673b862218f2e1ed3c0da`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 05:26:17 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:27:26 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:27:26 GMT
ENV PYPY_VERSION=7.3.12
# Thu, 10 Aug 2023 05:35:03 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.12-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0996054207b401aeacace1aa11bad82cfcb463838a1603c5f263626c47bbe0e6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.12-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:35:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 10 Aug 2023 05:35:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 10 Aug 2023 05:36:47 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 10 Aug 2023 05:36:48 GMT
CMD ["pypy"]
# Thu, 10 Aug 2023 06:13:08 GMT
ENV HY_VERSION=0.27.0
# Thu, 10 Aug 2023 06:13:09 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 10 Aug 2023 06:15:45 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 10 Aug 2023 06:15:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1bc20c9343735e8436617bc0e77797769bbe283f316e2914637152114c2a02`  
		Last Modified: Thu, 10 Aug 2023 05:46:34 GMT  
		Size: 247.2 KB (247168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60903cc4c73c3184760d5318d9d1564dd4c49288cd6a586335588d7a6ba6234`  
		Last Modified: Thu, 10 Aug 2023 05:46:36 GMT  
		Size: 15.6 MB (15623738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60407c31843c441aeebfbeacbf654386dc9484c3bef7973ce56242b11814661`  
		Last Modified: Thu, 10 Aug 2023 05:46:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454282df7db1a037a81c2764639c71fe1497038f35cb8d2ddbb90bbd4de30f60`  
		Last Modified: Thu, 10 Aug 2023 05:47:31 GMT  
		Size: 26.5 MB (26489449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a3169ad938b3a67f1d08cb3651ae92a1ad0a5cdfb4f4d2702ba5919e023de9`  
		Last Modified: Thu, 10 Aug 2023 05:47:24 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1d290aa4681896b8753bd3bccfd4e3a5ba771723d5da4b946a53a75803a1f0`  
		Last Modified: Thu, 10 Aug 2023 05:47:24 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881793767bde9f797f558712bd3537bb91604a7eb5c0332815661c83b45f419a`  
		Last Modified: Thu, 10 Aug 2023 05:47:26 GMT  
		Size: 3.4 MB (3440755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b71082a9445a1c0abc6062a6050a2d6dfe9d69a1a5904a74056e8b3fb308f`  
		Last Modified: Thu, 10 Aug 2023 05:47:24 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4779252671027e62347ef71ecc8e19edba998ae1ad3bf75c71db588091538a3`  
		Last Modified: Thu, 10 Aug 2023 06:16:23 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1df62a1a949236a531e9da96da305c0108cb4ad4c57e6f1a49d43430074a85b`  
		Last Modified: Thu, 10 Aug 2023 06:16:23 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905fd6a5c68848def39901a0ae11f2ffd5a8a27a34c6a48c31896271bf19c4c`  
		Last Modified: Thu, 10 Aug 2023 06:16:25 GMT  
		Size: 4.6 MB (4558633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ad51bd34eaf6d6eecb51e381a7c90e821c01d4ee9e584e10dedd1e414647f`  
		Last Modified: Thu, 10 Aug 2023 06:16:23 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
