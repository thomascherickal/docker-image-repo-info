## `hylang:pypy3.6`

```console
$ docker pull hylang@sha256:dad8f9386bbdb9120576119095c29e74835af089b085ebf8320374e66853eedf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64

### `hylang:pypy3.6` - linux; amd64

```console
$ docker pull hylang@sha256:4d8cbc320474d8a3ac66465feabf477facacbc9e89268fd5a3134dc578782faf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70977071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd148acc2ef618fb0aa0bc0cbfdde00efb4a2965eb8f07aa4e794b2d52ab638`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Thu, 18 Feb 2021 23:33:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Feb 2021 23:33:06 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:33:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:33:07 GMT
ENV PYPY_VERSION=7.3.3
# Thu, 18 Feb 2021 23:35:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 18 Feb 2021 23:35:24 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 18 Feb 2021 23:35:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 18 Feb 2021 23:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 18 Feb 2021 23:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 18 Feb 2021 23:35:41 GMT
CMD ["pypy3"]
# Fri, 19 Feb 2021 00:19:27 GMT
ENV HY_VERSION=0.20.0
# Fri, 19 Feb 2021 00:19:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 19 Feb 2021 00:19:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fadefae635d359139799f191ef45075984b7d362e8fdc80a531ff11a7c8ee7`  
		Last Modified: Thu, 18 Feb 2021 23:38:26 GMT  
		Size: 2.8 MB (2757361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668e8200b845c483fb3bfdbb2230fd15432bb3407b3d2ca9e1b641c341f27726`  
		Last Modified: Thu, 18 Feb 2021 23:39:24 GMT  
		Size: 35.7 MB (35694188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d39972baf4a495a516457b695a58374cf79c72d00324257e62a06d49eedcf2f`  
		Last Modified: Thu, 18 Feb 2021 23:39:16 GMT  
		Size: 2.4 MB (2413893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0dbd8bddda5244deb407360052c659aa3dfb437748786d7e127446ffd57c42`  
		Last Modified: Fri, 19 Feb 2021 00:21:33 GMT  
		Size: 3.0 MB (3016487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:08ebb94868b0299c05ad40910c939602504c5cc52c1bbaaae1256f4d8a18c6c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63381058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:171f829b267b335c9a0be2e702d6e1016b3b697627689d9d59489c2645e5c784`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Thu, 18 Feb 2021 23:53:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Feb 2021 23:53:44 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:53:44 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:53:45 GMT
ENV PYPY_VERSION=7.3.3
# Thu, 18 Feb 2021 23:57:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 18 Feb 2021 23:58:00 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 18 Feb 2021 23:58:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 18 Feb 2021 23:58:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 18 Feb 2021 23:58:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 18 Feb 2021 23:58:55 GMT
CMD ["pypy3"]
# Fri, 19 Feb 2021 00:30:28 GMT
ENV HY_VERSION=0.20.0
# Fri, 19 Feb 2021 00:30:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 19 Feb 2021 00:30:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7cd30fd6fbf960ed5ca54de088439f4fe0d462e29a54f58353e1308ba44097`  
		Last Modified: Fri, 19 Feb 2021 00:03:31 GMT  
		Size: 2.6 MB (2626140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3450b410eb1baeb15192a35b854eab5c9ad18af6b1d8c986ab3d5bb6b090e60`  
		Last Modified: Fri, 19 Feb 2021 00:04:45 GMT  
		Size: 29.5 MB (29471388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681e9b099e9fde9601640bceae3de582a69e443537741e462fb1bb0cb3ba952b`  
		Last Modified: Fri, 19 Feb 2021 00:04:35 GMT  
		Size: 2.4 MB (2415045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648f67bff269afde6daea908df9f22ab89b35c55eb86db5dcfa344aa9da6ca8e`  
		Last Modified: Fri, 19 Feb 2021 00:33:29 GMT  
		Size: 3.0 MB (3017036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; 386

```console
$ docker pull hylang@sha256:309d7dd8df68af61a3c6b89a13eccbcca83ed16ac99960ebef7cf12c5c16c320
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73947757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8efb4dec457de102d9170f1c9af72d90ed2eb86022c17400d0af6eb3599d957`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Thu, 18 Feb 2021 23:39:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Feb 2021 23:39:55 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:39:55 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:39:55 GMT
ENV PYPY_VERSION=7.3.3
# Thu, 18 Feb 2021 23:42:27 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 18 Feb 2021 23:42:27 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 18 Feb 2021 23:42:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 18 Feb 2021 23:42:28 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 18 Feb 2021 23:42:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 18 Feb 2021 23:42:45 GMT
CMD ["pypy3"]
# Fri, 19 Feb 2021 00:04:12 GMT
ENV HY_VERSION=0.20.0
# Fri, 19 Feb 2021 00:04:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 19 Feb 2021 00:04:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6f64dc70898e3d1b0a2893a17cb9b35505dd9b72d8dea0519f161a1f90382a`  
		Last Modified: Thu, 18 Feb 2021 23:45:37 GMT  
		Size: 2.8 MB (2769461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8817aa53af65a2f2173f0cc31dbc610acb38bf7b205e1f2bd4f039f178018c5`  
		Last Modified: Thu, 18 Feb 2021 23:46:38 GMT  
		Size: 38.0 MB (37995486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d1e73183f94e50e45c4ab94bf79b8604e6ab9ef53668b7d908d3333b3c121c`  
		Last Modified: Thu, 18 Feb 2021 23:46:27 GMT  
		Size: 2.4 MB (2413618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bbd1a0d43ae023f0aaf1123494ebd80418c06781dac9d631d37f3f052286b9`  
		Last Modified: Fri, 19 Feb 2021 00:06:24 GMT  
		Size: 3.0 MB (3016461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; s390x

```console
$ docker pull hylang@sha256:4ada392e108bbc6ed3626ffd8de54f8dba89b2e5190a54b590d9a44a8f1ba4a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66238129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b68a448c0ab9b2c801e65df3c799e6827f409eecfd6bcbe45619a365afa33f4`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Thu, 18 Feb 2021 23:43:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Feb 2021 23:43:48 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:43:49 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:43:49 GMT
ENV PYPY_VERSION=7.3.3
# Thu, 18 Feb 2021 23:45:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 18 Feb 2021 23:45:28 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 18 Feb 2021 23:45:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 18 Feb 2021 23:45:28 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 18 Feb 2021 23:45:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 18 Feb 2021 23:45:39 GMT
CMD ["pypy3"]
# Fri, 19 Feb 2021 00:04:04 GMT
ENV HY_VERSION=0.20.0
# Fri, 19 Feb 2021 00:04:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 19 Feb 2021 00:04:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf478751642e7524ba282283fd2578e663e65f395a8c6074c8b654862b03fe`  
		Last Modified: Thu, 18 Feb 2021 23:46:38 GMT  
		Size: 2.5 MB (2452228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eea6cef85af45bd69b94d512126a13075dfd489b009eee8fdb7c8657a23232f`  
		Last Modified: Thu, 18 Feb 2021 23:47:31 GMT  
		Size: 32.6 MB (32644869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9b28c36dd5eb710184a45f506ba70869bcae3eb02b3dc5fd876f25b419c47`  
		Last Modified: Thu, 18 Feb 2021 23:47:25 GMT  
		Size: 2.4 MB (2414098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09d11cbbea6cee11f9975ee86bd815cc1307f2d02d727b956785bf9e3b846a8`  
		Last Modified: Fri, 19 Feb 2021 00:05:57 GMT  
		Size: 3.0 MB (3016913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - windows version 10.0.17763.1757; amd64

```console
$ docker pull hylang@sha256:3f5aced6fafc1380b373f0e90c3d5655c7cb72a422aefc819b2173ae39ce5374
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2529818740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97116a5e4b33e68ef394b47dc901e6e17eb3cd0fc790eb9c1d549efd647b10f`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 26 Feb 2021 21:35:17 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:35:50 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = '12a69af8623d70026690ba14139bf3793cc76c865759cad301b207c1793063ed'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:35:51 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 26 Feb 2021 21:39:36 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.6-v7.3.3-win32.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'b935253877b703d29b1b11f79e66944f1f88adb8a76f871abf765d4de9d25f8a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.6-v7.3.3-win32 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:39:38 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Fri, 26 Feb 2021 21:39:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 26 Feb 2021 21:39:40 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 26 Feb 2021 21:41:00 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:41:01 GMT
CMD ["pypy3"]
# Tue, 02 Mar 2021 00:16:45 GMT
ENV HY_VERSION=0.20.0
# Tue, 02 Mar 2021 00:17:41 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 02 Mar 2021 00:17:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa33adbddd2e748e6b74e4adfd962ff90ea325ee1855aa526419b7d06043e132`  
		Last Modified: Fri, 26 Feb 2021 21:46:52 GMT  
		Size: 9.4 MB (9436033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b7e0ec23c257582c7dc16b6f75fc0963fef731973b27ff3f38db1606b1f9b4`  
		Last Modified: Fri, 26 Feb 2021 21:47:08 GMT  
		Size: 18.2 MB (18195523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0bb215c93560d1ce5ecd3d1b38692f86d3e57c5182666004ad8bb3b6ea5f`  
		Last Modified: Fri, 26 Feb 2021 21:46:46 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3886d9a01a962ba5efa30e50ea1f9fe57fb65664ce143dbfb5bbbb2adbaedb8`  
		Last Modified: Fri, 26 Feb 2021 21:47:42 GMT  
		Size: 47.5 MB (47544345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674112ba13f8bc10d42b9aaef40ca2f235cbeea3eb0aca367346b04316b21aaf`  
		Last Modified: Fri, 26 Feb 2021 21:47:27 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61050e8b89c58bae88cc73c5b322d0727a1bb2377fab5872520023c9abb64bad`  
		Last Modified: Fri, 26 Feb 2021 21:47:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46899c08be774e78f03a878854c9f707c4b4c7e9d9fb5b0b52230325cbcb7e01`  
		Last Modified: Fri, 26 Feb 2021 21:47:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847be602cbd12c81de7ac800ac43c1541aad30850bdcd5b86efa37e2070e9885`  
		Last Modified: Fri, 26 Feb 2021 21:47:30 GMT  
		Size: 7.2 MB (7151348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387f71100d1748cab584b651428c4bd9c7e176bc3d93dc78a00e13eb18628575`  
		Last Modified: Fri, 26 Feb 2021 21:47:27 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd29b6439495ac8cb5841475def51be60fa0405714a94452598e513232f00f4`  
		Last Modified: Tue, 02 Mar 2021 00:19:58 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6932b379b7b230ce89a093a71e0aa35e5e6a3d7a5404e23042585d1b943b1813`  
		Last Modified: Tue, 02 Mar 2021 00:19:59 GMT  
		Size: 8.2 MB (8213755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2002376652b536ec308289f79f6371b0860913f974458b2134e58194a2cc807d`  
		Last Modified: Tue, 02 Mar 2021 00:19:58 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
