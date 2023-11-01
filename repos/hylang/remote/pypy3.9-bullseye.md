## `hylang:pypy3.9-bullseye`

```console
$ docker pull hylang@sha256:9a1286a6edb9c70dd2077eb987be9ac81df14d983fa2e69c2ede246fa12bbb24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.9-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:814708c758046d93f67a59e3436dbfba63170b8450566a644fdbf0a2477beffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75495196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8974df62ac19b918ccba89e9f50bd6483da061e213e3c82f633d35a0ec7ad9e`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:59:11 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 02:59:11 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 02:59:11 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 03:02:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 03:02:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 03:02:16 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 03:02:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 03:02:28 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 18:25:36 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 18:25:36 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 18:26:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 18:26:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef2b30130a57efca31173eba0e2a0c72581f4d106a96241e4393caa34f8a17`  
		Last Modified: Wed, 01 Nov 2023 03:06:50 GMT  
		Size: 1.1 MB (1068483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e575aa1bbe94b13c24e18c02328fb8d64d9b21e1c6a68e9f6bad004b311c1b`  
		Last Modified: Wed, 01 Nov 2023 03:08:35 GMT  
		Size: 36.0 MB (35958940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811fd13b8aea3275bff14adc22b92999b5ecf6f0e7620ecbbc0ba4f0afc009a7`  
		Last Modified: Wed, 01 Nov 2023 03:08:30 GMT  
		Size: 3.1 MB (3131766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288927d273c2b28a77a40160778e07d3d0be0febc973ae027785ed86ac4c7423`  
		Last Modified: Wed, 01 Nov 2023 18:32:05 GMT  
		Size: 3.9 MB (3918092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:8f19a1eadc183ade2801646013038dc43cfd5c8535113f2d5327eddc3ac3b27b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71737061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f852011c8da3c1769c5da8b381ca9c3e20e36483a9499aced9cf140f5dbb7d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:33:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 11:33:01 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:33:01 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 11:35:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 11:35:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 11:35:46 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 11:35:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 11:35:57 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 16:36:16 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 16:36:16 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 16:36:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 16:36:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe440a5d75ca4a0dd3c95c44df16c78acb1db0649bf9cc2c2b42d2145ca7a85`  
		Last Modified: Wed, 01 Nov 2023 11:40:00 GMT  
		Size: 1.1 MB (1055762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8d28bda4547c0a83d230dd640af9b7ce5d2cecc1fd6c76ec06463952a9a476`  
		Last Modified: Wed, 01 Nov 2023 11:41:44 GMT  
		Size: 33.6 MB (33567602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b846992a12e29419af65829205fcdbfebfe936ebd16d1d3e34f804b65651fb39`  
		Last Modified: Wed, 01 Nov 2023 11:41:40 GMT  
		Size: 3.1 MB (3131701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb78ed1b6077f8765d43fd56babe2d4d4a75789a7c476b92ef3abc3cc3ca6bcb`  
		Last Modified: Wed, 01 Nov 2023 16:42:35 GMT  
		Size: 3.9 MB (3918091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:a73138fa072abf97b2340a9c5c8213475075c03fdc3bb1ebfce2419d59927798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74890419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b45b35975413794a800a58988b2e494a988ad9aae37c5c923c3c61fda24b37`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:18 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Wed, 01 Nov 2023 00:39:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:34:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:34:37 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 13:34:37 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 13:34:37 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 13:37:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 13:37:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 13:37:17 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 13:37:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 13:37:32 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 17:47:46 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 17:47:46 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 17:48:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 17:48:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c02d1b0e4ef370478856af1c8a52a346f41a1a2941092f3f2d134729d60d9d`  
		Last Modified: Wed, 01 Nov 2023 13:40:33 GMT  
		Size: 1.1 MB (1080422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf55705dd83680766bf584df425754daa593c38b396c891602cb008746c7937f`  
		Last Modified: Wed, 01 Nov 2023 13:41:57 GMT  
		Size: 34.4 MB (34357418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4291d0b898dc7db18eaf67b430aff95f25f9c941d1f9887f203e3c903fa729dd`  
		Last Modified: Wed, 01 Nov 2023 13:41:50 GMT  
		Size: 3.1 MB (3131561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08dae1bb71d63a9f537231bbe50a582f797168d6aa8122ab3f62433ad9ba377`  
		Last Modified: Wed, 01 Nov 2023 17:54:40 GMT  
		Size: 3.9 MB (3918326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
