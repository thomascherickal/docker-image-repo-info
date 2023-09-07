## `hylang:pypy3.9-bookworm`

```console
$ docker pull hylang@sha256:6aad18e30308e5cc0877fc7e6e2723791390b487522ba5752558521a5e0b0327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.9-bookworm` - linux; amd64

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

### `hylang:pypy3.9-bookworm` - linux; arm64 variant v8

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

### `hylang:pypy3.9-bookworm` - linux; 386

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
