## `pypy:3-7-slim`

```console
$ docker pull pypy@sha256:0d9ff5aaeb4ee2450d928daed62e9bc5afc728bfa6276e5532d25827ad6ba976
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `pypy:3-7-slim` - linux; amd64

```console
$ docker pull pypy@sha256:4a98a532c18d59d3c2ecd5bee25f3fce8112d8b39303ed206c6a45c2c64a6d2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68006457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eba8130d64cbc544b93e0b31c45174acde48fb1a0db4b631462c1ca22dbb1e`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:50:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:50:33 GMT
ENV LANG=C.UTF-8
# Tue, 30 Mar 2021 22:50:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 22:50:34 GMT
ENV PYPY_VERSION=7.3.3
# Wed, 31 Mar 2021 22:21:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 31 Mar 2021 22:21:56 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 31 Mar 2021 22:21:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 31 Mar 2021 22:21:57 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 31 Mar 2021 22:22:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 31 Mar 2021 22:22:10 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f7a54e58461c3962f5ab9b1da47b2e5f4d723d35580eec0dfeb97f00de3ff`  
		Last Modified: Tue, 30 Mar 2021 22:55:31 GMT  
		Size: 2.8 MB (2757692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eb2231abc25b724d8b80edf81811b3add69f1c3b23d3f91b85ec1006a9a3d`  
		Last Modified: Wed, 31 Mar 2021 22:25:51 GMT  
		Size: 35.7 MB (35694611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebd42f26e247748f2315965c840c05a2dcc08b40980624d94199ea62f8ecc75`  
		Last Modified: Wed, 31 Mar 2021 22:25:45 GMT  
		Size: 2.4 MB (2414861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-slim` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:b3462ff24946a022f7b4f9dc2d8476e558ea06a4e3e054f3795688890a5cfd9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60417651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539113c4408c6a44ec6389e8adf8f5ac2ad1c130b149e9f854283f20de866d9a`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 09:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:59:34 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 09:59:35 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 09:59:36 GMT
ENV PYPY_VERSION=7.3.3
# Thu, 01 Apr 2021 08:20:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 01 Apr 2021 08:20:35 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 01 Apr 2021 08:20:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 01 Apr 2021 08:20:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 01 Apr 2021 08:21:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 01 Apr 2021 08:21:09 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ba70755e64dfb8d4099343e2946351934314c3618d872775391f47d804c8eb`  
		Last Modified: Wed, 31 Mar 2021 10:06:49 GMT  
		Size: 2.6 MB (2626375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71edca1faacbc40e9f75e65a307a95934959b6a808663d64df32ff2e14515797`  
		Last Modified: Thu, 01 Apr 2021 08:23:59 GMT  
		Size: 29.5 MB (29471317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b610c4f8c6a80fbab09eb4421f49950f5dc7f57dc48cf24bda6fdca05673695f`  
		Last Modified: Thu, 01 Apr 2021 08:23:49 GMT  
		Size: 2.4 MB (2415446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-slim` - linux; 386

```console
$ docker pull pypy@sha256:60e391c5e215211e831e55eafdb45a99d547a1f6673e6ffd64cec5414bc68de5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70941278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2027b771c2b4b05c8193f4b83c22a27ffc886da02f2a2c52e10e2aecfb98943`
-	Default Command: `["pypy3"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 21:18:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 21:18:54 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:18:54 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 21:18:54 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 12 Mar 2021 21:21:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 12 Mar 2021 21:21:44 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Fri, 12 Mar 2021 21:21:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 12 Mar 2021 21:21:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 12 Mar 2021 21:22:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 12 Mar 2021 21:22:03 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c875064fad6d2298c98cda6cc9ae19e78ba1d8bcc7a895090af0b1e99f522f`  
		Last Modified: Fri, 12 Mar 2021 21:27:50 GMT  
		Size: 2.8 MB (2769467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac110df9efcf7fcb3bde998b985fb2719117566db417a6c91af7e95723403c81`  
		Last Modified: Fri, 12 Mar 2021 21:29:57 GMT  
		Size: 38.0 MB (37996391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bca94bc60d68a4f11fd795b540264a293de1e4d354b7113bdb0d9d0ebbd045`  
		Last Modified: Fri, 12 Mar 2021 21:29:46 GMT  
		Size: 2.4 MB (2414472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-slim` - linux; s390x

```console
$ docker pull pypy@sha256:11127fc77cc6ae2714ba5e530509fff623069f66fd8fcbcc3dcd5a73a5bd6dcc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63228028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e0f3604a2f17e9501459993a4f474073feb6912d1ee86d9cb540a0655ff09a`
-	Default Command: `["pypy3"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 04:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:53:27 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 04:53:28 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 04:53:28 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 12 Mar 2021 04:55:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 12 Mar 2021 04:55:49 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Fri, 12 Mar 2021 04:55:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 12 Mar 2021 04:55:50 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 12 Mar 2021 04:56:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 12 Mar 2021 04:56:04 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d910d2cdc8d3e1f74022262fc8995940046c1397abb26a9436ae0e942f198f`  
		Last Modified: Fri, 12 Mar 2021 04:57:02 GMT  
		Size: 2.5 MB (2452237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f001ce4b32dc0671b7fef517bc4db120652128e4857e0ac620d2a9c8be42a207`  
		Last Modified: Fri, 12 Mar 2021 04:57:49 GMT  
		Size: 32.6 MB (32644835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34500713d6916510a8fd6daee05f0354f2f09cf5894bd0ddd7b22609acba406`  
		Last Modified: Fri, 12 Mar 2021 04:57:43 GMT  
		Size: 2.4 MB (2414662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
