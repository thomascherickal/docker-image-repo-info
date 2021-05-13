## `hylang:pypy3.7`

```console
$ docker pull hylang@sha256:e827ed48e046faf0ac3572434e28cd563796c63bccdfcca4e83c13ecd871b708
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64

### `hylang:pypy3.7` - linux; amd64

```console
$ docker pull hylang@sha256:53d9893252345283feac9a8e00eae297829a6cef747e66576d1327b87fef8dfd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74173545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e277a1709a148a69c6c5520389d7edf58e1b18dd5a2ab249603c52e59837ef`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:53:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:53:43 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 14:53:43 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:53:43 GMT
ENV PYPY_VERSION=7.3.4
# Sat, 10 Apr 2021 14:54:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 10 Apr 2021 14:54:10 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 10 Apr 2021 14:54:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 10 Apr 2021 14:54:10 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 10 Apr 2021 14:54:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 10 Apr 2021 14:54:23 GMT
CMD ["pypy3"]
# Tue, 20 Apr 2021 01:22:33 GMT
ENV HY_VERSION=1.0a1
# Tue, 20 Apr 2021 01:22:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 20 Apr 2021 01:22:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3da5fcf5fa7542a53548bf7e7c8a6b703cce1920fbfd5e30a79641a1047c04`  
		Last Modified: Sat, 10 Apr 2021 14:57:13 GMT  
		Size: 2.8 MB (2757654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71dcb35be3554efe9eb06a6058f7ab16efd20c2ebbdab0904f03dc179b70e58`  
		Last Modified: Sat, 10 Apr 2021 14:57:23 GMT  
		Size: 38.6 MB (38598611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e771f6c47637605bf43be1997efb24f0a4f76ba789042de94048eea563685`  
		Last Modified: Sat, 10 Apr 2021 14:57:13 GMT  
		Size: 2.6 MB (2565634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ca9d82001a935c99afa66bddfd7d317599f49be85e92dfec55d50710b490ee`  
		Last Modified: Tue, 20 Apr 2021 01:28:17 GMT  
		Size: 3.1 MB (3112273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:3f996fef980a55632477abdb43b36888a96b9dfcaf8f37e3a6206eccd59deea6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69572923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735a3e142df30794fa09aecd4b9214e99e43f9da7885c2e79c54745ce1aa4e24`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 10:59:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 10:59:31 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 10:59:31 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 10:59:32 GMT
ENV PYPY_VERSION=7.3.4
# Sat, 10 Apr 2021 11:00:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 10 Apr 2021 11:00:37 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 10 Apr 2021 11:00:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 10 Apr 2021 11:00:39 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 10 Apr 2021 11:01:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 10 Apr 2021 11:01:14 GMT
CMD ["pypy3"]
# Tue, 20 Apr 2021 01:50:46 GMT
ENV HY_VERSION=1.0a1
# Tue, 20 Apr 2021 01:51:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 20 Apr 2021 01:51:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33eeb66cbe9658b76a975f836346c35755c240ebca8217427c30173634860e16`  
		Last Modified: Sat, 10 Apr 2021 11:05:15 GMT  
		Size: 2.6 MB (2626374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab0ee42cb4a11e3e17422c825ccbc39df6b242599eba21cfe6e967484a3704`  
		Last Modified: Sat, 10 Apr 2021 11:05:26 GMT  
		Size: 35.4 MB (35363717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5666e8cc1941e207efae721881e8fe98ea0496bf008b64b51a82aa485511c`  
		Last Modified: Sat, 10 Apr 2021 11:05:15 GMT  
		Size: 2.6 MB (2565538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a558928dc3270ca4d9cc7ae24c4b03871d41387397715d713c323ca787df6a`  
		Last Modified: Tue, 20 Apr 2021 01:55:28 GMT  
		Size: 3.1 MB (3112712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; 386

```console
$ docker pull hylang@sha256:441bbf31bc3815cee562244719f5eded806a28f042ed86f64e4bec0f582df7e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76848043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6f9bdf9d3967e5783e9bf84877e66aee75ffeea740877b6e8d238d55df7f5d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 12:38:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 12:38:40 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 12:38:41 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 12:38:41 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 12:39:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 12:39:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 12:39:25 GMT
CMD ["pypy3"]
# Wed, 12 May 2021 19:21:07 GMT
ENV HY_VERSION=1.0a1
# Wed, 12 May 2021 19:21:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 12 May 2021 19:21:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb63b37fe34f2cd5f37adaacc9536932e1923c91535448092ffc5ffcc0d19bb`  
		Last Modified: Wed, 12 May 2021 12:44:01 GMT  
		Size: 2.8 MB (2769460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140de4b878d8cf1b24ae54ce98ccf0f9791927177a904b5f66c16b580f4f6559`  
		Last Modified: Wed, 12 May 2021 12:44:16 GMT  
		Size: 40.6 MB (40605139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add89bd2f94ae5e2d48399acafa4c1724f536282ded7bd4c79a46fa098041878`  
		Last Modified: Wed, 12 May 2021 12:44:01 GMT  
		Size: 2.6 MB (2565766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84e413f0e98e790391ee3869973b78b34bf3001f70c2e7732cb91ac90353b0d`  
		Last Modified: Wed, 12 May 2021 19:26:25 GMT  
		Size: 3.1 MB (3112604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; s390x

```console
$ docker pull hylang@sha256:5b4ee55ad1d4435e5eedf21db6a023c1423c8af8016cf7c945b470545984b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69473409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff020b4af23350249a8809179ec992a97f9a5544cfa3136babe64da8bb9bdf`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:02 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:13:02 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:13:03 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 06:13:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 06:14:04 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 06:14:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 06:14:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 06:14:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 06:14:31 GMT
CMD ["pypy3"]
# Wed, 12 May 2021 21:57:45 GMT
ENV HY_VERSION=1.0a1
# Wed, 12 May 2021 21:58:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 12 May 2021 21:58:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb18f5c9b647c5730f0ed0acea816dc6504113efcc15f2b461b4959b4470bc`  
		Last Modified: Wed, 12 May 2021 06:15:48 GMT  
		Size: 2.5 MB (2452407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4572a6625dfad1d2e1321c81085e284ec00994ea434cfc1f27f78c687c286e`  
		Last Modified: Wed, 12 May 2021 06:15:57 GMT  
		Size: 35.6 MB (35581814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc39c4eacd9dae67c1a3cbe3f612c721538fc86504b57de9ba85f6690fa6a4`  
		Last Modified: Wed, 12 May 2021 06:15:48 GMT  
		Size: 2.6 MB (2566210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1970da7e2ff0630d4e83d4b9d4f11d088824c081565def1bcad096913b4e0b2d`  
		Last Modified: Wed, 12 May 2021 22:00:14 GMT  
		Size: 3.1 MB (3112807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - windows version 10.0.17763.1935; amd64

```console
$ docker pull hylang@sha256:5dbf893722b4242e006952513b0beb9ce76afdbeaa218c5aa5d8a47df9ec642b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2528806629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826956fd48d9755832d7fc336c6ee7778872e3cf6128120988f23af0261ba951`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:11:29 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 12 May 2021 12:12:07 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 12 May 2021 12:12:08 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 12:13:11 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0ff4e4653f1ff0653f105680eb101c64c857fa8f828a54a61b02f65c94b5d262'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.4-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 12 May 2021 12:13:13 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 12:13:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 12:13:15 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 12:15:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 12 May 2021 12:15:03 GMT
CMD ["pypy3"]
# Wed, 12 May 2021 16:29:35 GMT
ENV HY_VERSION=1.0a1
# Wed, 12 May 2021 16:30:41 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 12 May 2021 16:30:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646d0b1f5b2de003e7020ff1d5159bdda97a41947bc8ea1f0462695be1954832`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 5.1 MB (5095334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5660485e40f20eb051915b07c98bbea7a0251908408aedb487ec0cc4de228afa`  
		Last Modified: Wed, 12 May 2021 12:20:49 GMT  
		Size: 15.5 MB (15482514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab72861d4181ae7cfc020ba097cb2253a1702478e0d7f5f20982e162ab08e599`  
		Last Modified: Wed, 12 May 2021 12:20:30 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26a24b8dafc4d3221e206b58f54a9a95f408822c886357fdb7d033e4bd516e1`  
		Last Modified: Wed, 12 May 2021 12:20:38 GMT  
		Size: 26.9 MB (26922970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c022078e9fb6e2a17272ebf52e549ec2dd6b315d8160f77a291eb322b884356`  
		Last Modified: Wed, 12 May 2021 12:20:28 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af180e039a0ed206591e2525438f4bd2e6464be796d222c5028b759fb635e0e5`  
		Last Modified: Wed, 12 May 2021 12:20:28 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68aed7ad8327b382722052574fa1526f82a6ffc0aee98241be0de0a354f0fbb`  
		Last Modified: Wed, 12 May 2021 12:20:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f6ac9b0a6e60da6c11709657d49a754879426ca855cce315100b937190b862`  
		Last Modified: Wed, 12 May 2021 12:20:29 GMT  
		Size: 2.9 MB (2896217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ebbff15b8ca8057773d26cce86ab855233caffe8a0440443f99c4110dd3e5`  
		Last Modified: Wed, 12 May 2021 12:20:28 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b57c5b7505a15beafec8127f84fbf393aca9afd4650343eecaa78990870ee56`  
		Last Modified: Wed, 12 May 2021 16:33:41 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23f4eafe5efc7e6f949bbf2b442396071146fd1ad57f826caeb75d2e63a379b`  
		Last Modified: Wed, 12 May 2021 16:33:41 GMT  
		Size: 3.9 MB (3909099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d7b9618b4f136c40e67c0cf7a32f385dfe83fa9d6ffec7744bc7a420a47ee1`  
		Last Modified: Wed, 12 May 2021 16:33:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
