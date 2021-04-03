## `hylang:pypy3.6`

```console
$ docker pull hylang@sha256:d7babdaf43c0deb783d4acafab3704955fabf5dc933baba50428115555908a02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64

### `hylang:pypy3.6` - linux; amd64

```console
$ docker pull hylang@sha256:d4249e3850279ca510265d5cfdecb8e37c57c8aee40bf3ab63f20835db9f8fe3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71024036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61011311a865b03bd384d0bc82f4b76c1ecd3e9fbb661746e01cf3e8a9b4204`
-	Default Command: `["hy"]`

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
# Thu, 01 Apr 2021 11:33:43 GMT
ENV HY_VERSION=0.20.0
# Thu, 01 Apr 2021 11:33:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 01 Apr 2021 11:33:52 GMT
CMD ["hy"]
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
	-	`sha256:01545d5b6b3c7a52306040f8a788f4cf2c9a29bccd5f19e2e2aef99ded0c4e6f`  
		Last Modified: Thu, 01 Apr 2021 11:39:24 GMT  
		Size: 3.0 MB (3017579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:64a26361dad73989bc0267efaab42252a6678f669a842a7bc305fbc0b18cf627
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63435300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2849c29164d434da02cc84bc2610454faeccc9d1ba1615a37b032d1a0523284`
-	Default Command: `["hy"]`

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
# Thu, 01 Apr 2021 08:28:39 GMT
ENV HY_VERSION=0.20.0
# Thu, 01 Apr 2021 08:29:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 01 Apr 2021 08:29:01 GMT
CMD ["hy"]
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
	-	`sha256:c4a42f9434846a211ec502e423539ecf0b2047801619e3eb2531a5f24474b31d`  
		Last Modified: Thu, 01 Apr 2021 08:32:40 GMT  
		Size: 3.0 MB (3017649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; 386

```console
$ docker pull hylang@sha256:7f3bd36a48f1ea76d7320ab08d540afa71671a399cb1eeed16be91e0c8895248
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73958963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821313d359d60552811e63cc4fd4dfb415bec09435b248f5d9a04561a7a85fc3`
-	Default Command: `["hy"]`

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
# Sat, 13 Mar 2021 00:29:06 GMT
ENV HY_VERSION=0.20.0
# Sat, 13 Mar 2021 00:29:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 13 Mar 2021 00:29:21 GMT
CMD ["hy"]
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
	-	`sha256:de9535174d1b3a2b8199519d39eb7e23009f8381cc5ff2ca6a8b626e58d7f7fd`  
		Last Modified: Sat, 13 Mar 2021 00:41:10 GMT  
		Size: 3.0 MB (3017685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - linux; s390x

```console
$ docker pull hylang@sha256:95f16bd05dfaf621073c95f5ef44c3ba4d95cc780d656394cc030c591a57451c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66283346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed578e87065f574b34d9886c9374f2695b5ebe793ab5851fc9d61064091f4ca6`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 01:39:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:39:06 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 01:39:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 01:39:06 GMT
ENV PYPY_VERSION=7.3.3
# Sat, 03 Apr 2021 01:40:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux64.tar.bz2'; 			sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-aarch64.tar.bz2'; 			sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-linux32.tar.bz2'; 			sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.6-v7.3.3-s390x.tar.bz2'; 			sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O import.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/16faa2be85839e6ab4fb8ee09298a4d934aab81f.patch'; 	echo '2d4bcc434077685a4ff26c1c1f28109ff67ef7e68f1f831ce0f2d9ddd6a194d0 *import.patch' | sha256sum --check --strict -; 	wget -O crypt-utf8.patch 'https://foss.heptapod.net/pypy/pypy/-/commit/c63da169246ed972fe90e1c289fc2378236fa852.patch'; 	echo 'ab1529948c49fd29fb76b3c20ec7d3d9c50603aa0c549a8a31339eb940e0f4d3 *crypt-utf8.patch' | sha256sum --check --strict -; 	patch --input="$PWD/import.patch" --directory=/opt/pypy --strip=1; 	patch --input="$PWD/crypt-utf8.patch" --directory=/opt/pypy --strip=1; 	rm import.patch crypt-utf8.patch; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 03 Apr 2021 01:40:48 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 03 Apr 2021 01:40:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 03 Apr 2021 01:40:49 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 03 Apr 2021 01:41:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 03 Apr 2021 01:41:00 GMT
CMD ["pypy3"]
# Sat, 03 Apr 2021 02:09:17 GMT
ENV HY_VERSION=0.20.0
# Sat, 03 Apr 2021 02:09:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 03 Apr 2021 02:09:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737bb147c3c4de2c05698743622eadc50f90a2f106053a20c0db215b0f8374e0`  
		Last Modified: Sat, 03 Apr 2021 01:41:56 GMT  
		Size: 2.5 MB (2452353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c41bc1f3550beb92aed64ce60ddcfb5d867f37194fc8522c000c233f5b1dbb`  
		Last Modified: Sat, 03 Apr 2021 01:42:47 GMT  
		Size: 32.6 MB (32644994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae10b94ac11ff6feb640d500f85afde5e8e28dd321af58cc2d18505143878541`  
		Last Modified: Sat, 03 Apr 2021 01:42:40 GMT  
		Size: 2.4 MB (2414683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08708810d8ed3b19b5ae735ea6d7ba68a1b3702f5c5892698abe039f9cff04a`  
		Last Modified: Sat, 03 Apr 2021 02:11:09 GMT  
		Size: 3.0 MB (3017561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6` - windows version 10.0.17763.1817; amd64

```console
$ docker pull hylang@sha256:b4522f34e1f60b7d77f8a932b44f1281db1e7a283dd92125d8962baa5a530a82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2552118578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f6bf4844b92c7829233f996dc1d94c3f3b62789e919cb35524ba3b7cdbc954`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:09:43 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 10 Mar 2021 13:10:18 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = '12a69af8623d70026690ba14139bf3793cc76c865759cad301b207c1793063ed'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Mar 2021 13:10:19 GMT
ENV PYPY_VERSION=7.3.3
# Wed, 10 Mar 2021 13:14:07 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.6-v7.3.3-win32.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'b935253877b703d29b1b11f79e66944f1f88adb8a76f871abf765d4de9d25f8a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.6-v7.3.3-win32 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 10 Mar 2021 13:14:08 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 10 Mar 2021 13:14:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 10 Mar 2021 13:14:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 10 Mar 2021 13:15:38 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 10 Mar 2021 13:15:40 GMT
CMD ["pypy3"]
# Wed, 10 Mar 2021 17:36:12 GMT
ENV HY_VERSION=0.20.0
# Wed, 10 Mar 2021 17:37:14 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 10 Mar 2021 17:37:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa06ae93a71781008a718e572b4c76dd2b31ee79e2f7f1ce9863e7e5639208`  
		Last Modified: Wed, 10 Mar 2021 13:21:17 GMT  
		Size: 9.5 MB (9455936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d3265096084ca6994fcec09ef2856f30b1036dfdc247085b755c7e0c546587`  
		Last Modified: Wed, 10 Mar 2021 13:21:27 GMT  
		Size: 18.2 MB (18209911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaafd9fbf3c517b4c98f99f8fedfcabe333fc50a1a0cbca1078bb015a2f718c0`  
		Last Modified: Wed, 10 Mar 2021 13:21:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2246c7b28fbf25b08af34f2db342a0c4627389cd0428c4cdc365df02e86834`  
		Last Modified: Wed, 10 Mar 2021 13:22:38 GMT  
		Size: 47.5 MB (47542698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ab2e02e0e887f1ef2bb62033b35d3ca0a87aa471b61a01424507ecd538777f`  
		Last Modified: Wed, 10 Mar 2021 13:22:23 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d28ddec7d656706b2307935f0c1ea9d51d85a52eeb095dbd0bc213832c4fc54`  
		Last Modified: Wed, 10 Mar 2021 13:22:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a6d4bdfc69a07e22ed6050da6ab49c7345a0de529586f7b1b7c25b89e2516c`  
		Last Modified: Wed, 10 Mar 2021 13:22:23 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea39a5787172f39ddc5fdb2d057b612430bdbca881b428503810d7dd2ebef75`  
		Last Modified: Wed, 10 Mar 2021 13:22:31 GMT  
		Size: 7.2 MB (7155491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a77c1afcac5262f934c9c83e699ef082ac154faee5f227db447057c2562082`  
		Last Modified: Wed, 10 Mar 2021 13:22:23 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd0196372483a3085516669f4f7980043d7d4ad4beb4e010b6e83562ce7dbb`  
		Last Modified: Wed, 10 Mar 2021 17:41:06 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f36c5e2f427759ed8f56992a7a4e25c44a2818c1f20db67ff58623b7b9d867a`  
		Last Modified: Wed, 10 Mar 2021 17:41:09 GMT  
		Size: 8.2 MB (8208801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085f4801b52d546994a574eb714fc1af8e6c5a09544d69a9543da1e73df7ac8c`  
		Last Modified: Wed, 10 Mar 2021 17:41:06 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
