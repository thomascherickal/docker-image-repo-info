## `hylang:pypy3.10-bullseye`

```console
$ docker pull hylang@sha256:76a848b7484efaf1ee59f636d47f89b882c3213e5f6ede3001da55a22ecaf7e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.10-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:a51da364f58fa79e2968ecdef1d735e30169d9268df4785d6f03be709acf0000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.0 MB (77990013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f68fc95d6b5a2ec3cb52c116016dfd1e12c14860230ad73fa4414502ef3112`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:42:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:42:39 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 20:42:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 20:42:39 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 20 Sep 2023 20:43:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Sep 2023 20:43:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Sep 2023 20:43:10 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Sep 2023 20:43:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Sep 2023 20:43:22 GMT
CMD ["pypy3"]
# Thu, 21 Sep 2023 05:48:41 GMT
ENV HY_VERSION=0.27.0
# Thu, 21 Sep 2023 05:48:41 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 21 Sep 2023 05:49:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 21 Sep 2023 05:49:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f7206a1bfbed6df27ad7aa8d9528a3303c6b4547a02835275fbac87392f0bb`  
		Last Modified: Wed, 20 Sep 2023 20:50:27 GMT  
		Size: 1.1 MB (1066707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d799412f584f4ec8008f57ab547594a80c4147d36a3f85b62215594a6e694d`  
		Last Modified: Wed, 20 Sep 2023 20:50:33 GMT  
		Size: 35.7 MB (35675187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b17aed11b25c8c58c826bfff8f505550c22d8eb5b2b66a3dc6b6dea5526bb6`  
		Last Modified: Wed, 20 Sep 2023 20:50:27 GMT  
		Size: 3.5 MB (3517835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f806b1c07f25fffc6c8ea4b8c15155750cd1239e8e161112497cfd879dcc083d`  
		Last Modified: Thu, 21 Sep 2023 05:54:54 GMT  
		Size: 6.3 MB (6312573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.10-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:cb23b86a71734a333a8df8511ca95e441dc532b2b3b8e92fd2ae73d93e11c4ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74198254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f086f5200021c7424f9ea1b084e262be0ca8ef6f374b129b3639d92bc1ec34`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 16:20:01 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 16:20:02 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 20 Sep 2023 16:20:27 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Sep 2023 16:20:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Sep 2023 16:20:28 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Sep 2023 16:20:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Sep 2023 16:20:40 GMT
CMD ["pypy3"]
# Wed, 20 Sep 2023 22:05:10 GMT
ENV HY_VERSION=0.27.0
# Wed, 20 Sep 2023 22:05:10 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 20 Sep 2023 22:05:41 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Sep 2023 22:05:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f15a7e7343010645ed1e4024ce0d80b6d82a0278c01cbbe9d764a18df93`  
		Last Modified: Wed, 20 Sep 2023 16:26:54 GMT  
		Size: 1.1 MB (1054117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2b4f6302bb56ed090b3550a9cadd73191e7e27e5a388d969e0da9ca034cf33`  
		Last Modified: Wed, 20 Sep 2023 16:26:59 GMT  
		Size: 33.3 MB (33251413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55922bda9eba3394e574facc77b1d7a1ea5b76182c802aa5efaec0ebfe0d6396`  
		Last Modified: Wed, 20 Sep 2023 16:26:54 GMT  
		Size: 3.5 MB (3517388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baecdb4de08dd3f9adf375a90b1e45b2701fde5efd0df6582f11114e90e4588e`  
		Last Modified: Wed, 20 Sep 2023 22:12:11 GMT  
		Size: 6.3 MB (6312467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.10-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:58f44cfdd662162d59f093e9111cb2078aa6d5dbb88388f4ea57462e78896341
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77289797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0499ff7a88ab7075cc09f1f0bc7a18454faed4bb8ed0ae90b71d5e9cd03113`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:23 GMT
ADD file:7da3a32fda5f1208b9e4a0151bc02b156c151608c0a2c17b70ca382b4446d87f in / 
# Thu, 07 Sep 2023 00:39:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 19:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:48:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 19:48:07 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 19:48:07 GMT
ENV PYPY_VERSION=7.3.12
# Thu, 07 Sep 2023 19:48:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 07 Sep 2023 19:48:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 07 Sep 2023 19:48:44 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 07 Sep 2023 19:48:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Sep 2023 19:49:00 GMT
CMD ["pypy3"]
# Fri, 08 Sep 2023 06:49:17 GMT
ENV HY_VERSION=0.27.0
# Fri, 08 Sep 2023 06:49:17 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 08 Sep 2023 06:50:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 08 Sep 2023 06:50:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2508d8884943a2a8ff1cc6a8264b3085b7d7637e9de43269faf016019de5c311`  
		Last Modified: Thu, 07 Sep 2023 00:44:37 GMT  
		Size: 32.4 MB (32397335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a7832f66f10dfb3794f5b288633a114ca9d23b79c182a98fb6290c7b13caeb`  
		Last Modified: Thu, 07 Sep 2023 19:57:43 GMT  
		Size: 1.1 MB (1079103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910ca28a26b2bd9c5f774b6837256a80cee4484e1e1ad437c8194a7a77b49b15`  
		Last Modified: Thu, 07 Sep 2023 19:57:51 GMT  
		Size: 34.0 MB (33983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0495dd16ac773e4a8e4ed8f92578638f450f213bd01f1c43f7411add59498202`  
		Last Modified: Thu, 07 Sep 2023 19:57:44 GMT  
		Size: 3.5 MB (3517428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af0c6937f5af01c73c9a8b9acb3e8047c2669fee7253e5f91014cf892f775f`  
		Last Modified: Fri, 08 Sep 2023 06:56:43 GMT  
		Size: 6.3 MB (6312333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
