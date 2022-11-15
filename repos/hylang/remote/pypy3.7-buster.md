## `hylang:pypy3.7-buster`

```console
$ docker pull hylang@sha256:d3aab88e55a55e06f82cf42b971f22b3a99efeeaa83595962bb8f6de7d1eed91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:139d89d54d473ddadfec17d7a7f3a0b978ca7f52f591c00811b7f8d04e8cc631
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74187953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e954b10696b5acec6d91159dc308e63c604d9af3e7e9140f17a8fe5cea90db0`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:37:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:37:22 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:37:22 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:37:22 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 25 Oct 2022 04:41:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 25 Oct 2022 04:41:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 25 Oct 2022 04:41:24 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 25 Oct 2022 04:41:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 25 Oct 2022 04:41:36 GMT
CMD ["pypy3"]
# Wed, 09 Nov 2022 00:40:55 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:40:55 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:41:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:41:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18430058c533991af161a65e3a9459d90db65fd9b126e29dd85b94907dcb9f5b`  
		Last Modified: Tue, 25 Oct 2022 04:45:17 GMT  
		Size: 2.8 MB (2767945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fe8a4a3f97c49c2eea8516b957ccb95b7e3dcc85b5971b86c175fc1b4f0174`  
		Last Modified: Tue, 25 Oct 2022 04:47:47 GMT  
		Size: 37.3 MB (37303781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153baf36f33bf42aba49a316bf3d500a2490c2ddc26b439b0a4306b530a3fb3`  
		Last Modified: Tue, 25 Oct 2022 04:47:40 GMT  
		Size: 3.0 MB (2967829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bfeda219ff485d21cdafdcae632b6348f4208a3c50fc557298822bbf49d404`  
		Last Modified: Wed, 09 Nov 2022 00:52:41 GMT  
		Size: 4.0 MB (4007566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:991eb1cf49bbb68edf5aa6e43960dbc41b34d1ca9cbf8a4cc622ba09641e9886
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69948051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89bb2db70a19175560d54e2e2e1461fa8b94c1766617d8d9f255de36952c15fc`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:28:30 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:28:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 20:28:30 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 25 Oct 2022 20:34:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 25 Oct 2022 20:34:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 25 Oct 2022 20:34:01 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 25 Oct 2022 20:34:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 25 Oct 2022 20:34:12 GMT
CMD ["pypy3"]
# Wed, 09 Nov 2022 01:01:12 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 01:01:12 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 01:01:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 01:01:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5786fa89de23b3e97290e2d1f540aec191e8adc21b59675865b0f0085dc8c6b`  
		Last Modified: Tue, 25 Oct 2022 20:39:04 GMT  
		Size: 2.6 MB (2636501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5e6c26b9e4f57032ca317046a565d286c93741019802ade40ad39cc68d08b0`  
		Last Modified: Tue, 25 Oct 2022 20:43:02 GMT  
		Size: 34.4 MB (34421432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c678c0e4a94ced55b34a41d892fa8dc2beb680d8e0cda62a6b30202fc9eea8ee`  
		Last Modified: Tue, 25 Oct 2022 20:42:58 GMT  
		Size: 3.0 MB (2967415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799acb9dc5807f7d51069c365ed269462178b72e1519e72a3546f89dee017db`  
		Last Modified: Wed, 09 Nov 2022 01:13:13 GMT  
		Size: 4.0 MB (4007818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:e348f8f0598e20ec11bcdf0b30ba5631b84208682e59f52513ce134bf2fe8e9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76571920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8872c6efe4867737413a182ccb798fc80ada992d19ef56b4360c745ead80f3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:54 GMT
ADD file:0d8bf61c363b36e7073c9fd91c34181d2b278068a38749faee0d3c7ec654bda6 in / 
# Tue, 15 Nov 2022 01:41:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 09:25:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:25:49 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 09:25:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 09:25:51 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 09:33:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 09:33:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 09:33:37 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 09:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 09:33:52 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 19:49:37 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 19:49:37 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 19:50:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 19:50:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f3d13e168342b55b3a1ab5df56e84f077449ec7563d80bd1eca07424d641822e`  
		Last Modified: Tue, 15 Nov 2022 01:47:52 GMT  
		Size: 27.8 MB (27798392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a38cf7e91a298930e80da6fc2435f36ddace5e838b17cea181e8c4369d7a0`  
		Last Modified: Tue, 15 Nov 2022 09:42:13 GMT  
		Size: 2.8 MB (2781063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799ea09e1999b63d5f9bc72ad1ae738c64a1c9cb2ccac76f0ab97dbf24e87b04`  
		Last Modified: Tue, 15 Nov 2022 09:46:30 GMT  
		Size: 39.2 MB (39191286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613776c1a58170a37fd12b94543b1a69db1b02a8d419737d253d1e4d316b138`  
		Last Modified: Tue, 15 Nov 2022 09:46:23 GMT  
		Size: 2.7 MB (2748998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46c5bf5fe93b861249000f597681c8db50090bf546a6648f9ce4286c7cff413`  
		Last Modified: Tue, 15 Nov 2022 20:02:15 GMT  
		Size: 4.1 MB (4052181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
