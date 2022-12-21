## `pypy:2-7-slim-bullseye`

```console
$ docker pull pypy@sha256:b94b68df5102ac92b99e4818e13a023e3b2c8a3fadca497b762982acf9419b2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-7-slim-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:9a799d0782064470d64a3cf58694c329ac389f63f7f89a197b148145011d6488
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65683461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa2671cf9ef808bbe8de8dd207165f5d5f1dd3b194295b1b0b78345c6acdc24`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 11:48:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 11:48:29 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 11:48:29 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:35:02 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 07 Dec 2022 02:40:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux64.tar.bz2'; 			sha256='461fb6df524208af9e94ffb16989f628b585bdb4b9e97d81e668899fc3a064a3'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-aarch64.tar.bz2'; 			sha256='274342f0e75e99d60ba7a0cfb0e13792e7664163e01450d2f7f2f7825603a0ae'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux32.tar.bz2'; 			sha256='0b17132f62d2a0c3c4572c57eb53820f25611afad71f3d6a310202942baed6e1'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-s390x.tar.bz2'; 			sha256='0fac1ec1e05c70941f758be05d40ce7ffe6a42c0416e70b55d40a7523e3e70ae'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 07 Dec 2022 02:40:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 07 Dec 2022 02:40:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 07 Dec 2022 02:40:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 07 Dec 2022 02:40:44 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51466f3f8a8b55ab274f39a90e1dee7c042198a1e3c8c487a2dcb277d863ddf3`  
		Last Modified: Tue, 06 Dec 2022 12:00:36 GMT  
		Size: 1.1 MB (1067963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb46b7fbfd82bdff414ae9a19fb142ea0b3a3765b6d39b512db185f722b703`  
		Last Modified: Wed, 07 Dec 2022 02:47:26 GMT  
		Size: 31.0 MB (31030740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b25ffff5d7c30f855c30225f315e17e301fb23f064f5ad81e8ba0a02fc89886`  
		Last Modified: Wed, 07 Dec 2022 02:47:21 GMT  
		Size: 2.2 MB (2171906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:ce2d85a6f228989cb96d96a06fdfb0c043fa1e333b7e9ead78d76cac2f269fb1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62334240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2d1e8fadbd2b42054438539c97ea61581152626acbebacefb9543097d65579`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:41:39 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 06:41:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:13:26 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 07 Dec 2022 02:18:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux64.tar.bz2'; 			sha256='461fb6df524208af9e94ffb16989f628b585bdb4b9e97d81e668899fc3a064a3'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-aarch64.tar.bz2'; 			sha256='274342f0e75e99d60ba7a0cfb0e13792e7664163e01450d2f7f2f7825603a0ae'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux32.tar.bz2'; 			sha256='0b17132f62d2a0c3c4572c57eb53820f25611afad71f3d6a310202942baed6e1'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-s390x.tar.bz2'; 			sha256='0fac1ec1e05c70941f758be05d40ce7ffe6a42c0416e70b55d40a7523e3e70ae'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 07 Dec 2022 02:18:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 07 Dec 2022 02:18:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 07 Dec 2022 02:18:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 07 Dec 2022 02:18:19 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10899d04f0abe7df84b5d209e23478deeda253b78e63b28797c2c513ee13c8b0`  
		Last Modified: Tue, 06 Dec 2022 06:52:42 GMT  
		Size: 1.1 MB (1055302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabaf3f13502f71482cd6978aa612871bdaf3f3d78f098faad327a185d8dea44`  
		Last Modified: Wed, 07 Dec 2022 02:24:54 GMT  
		Size: 29.0 MB (29046894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d052ad9eb7ab8db559c5ba95e252a6b993b3889d1e594a76b22ce7f58e90d2f9`  
		Last Modified: Wed, 07 Dec 2022 02:24:50 GMT  
		Size: 2.2 MB (2171724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:da4c3b19e566fc96eb653db92107f96c47c8425a2e2cc31fe3626cb01f66f510
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62289749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd3654656d76acde8dcacbba4934cabe75ca0e00b02a7fb77a07012f0d3aa2d`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 06:22:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 06:22:48 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 06:22:49 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 06:22:50 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 21 Dec 2022 06:27:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux64.tar.bz2'; 			sha256='461fb6df524208af9e94ffb16989f628b585bdb4b9e97d81e668899fc3a064a3'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-aarch64.tar.bz2'; 			sha256='274342f0e75e99d60ba7a0cfb0e13792e7664163e01450d2f7f2f7825603a0ae'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-linux32.tar.bz2'; 			sha256='0b17132f62d2a0c3c4572c57eb53820f25611afad71f3d6a310202942baed6e1'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.10-s390x.tar.bz2'; 			sha256='0fac1ec1e05c70941f758be05d40ce7ffe6a42c0416e70b55d40a7523e3e70ae'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 21 Dec 2022 06:27:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 21 Dec 2022 06:27:41 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 21 Dec 2022 06:27:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 21 Dec 2022 06:27:53 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941f456ea08ae7e340ba6a224752f1ded93f0629c538040f1eb604dd321c990a`  
		Last Modified: Wed, 21 Dec 2022 06:32:27 GMT  
		Size: 1.1 MB (1078741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53152eb2f7a5d44cce3294c9203ad7d271fe4a2e2b27a09c5f2c99b8b5a8e17b`  
		Last Modified: Wed, 21 Dec 2022 06:35:16 GMT  
		Size: 26.9 MB (26880772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e227ef917034150b2229886289357da2db48b91630009aa0d657551309b1175d`  
		Last Modified: Wed, 21 Dec 2022 06:35:12 GMT  
		Size: 2.0 MB (1954491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
