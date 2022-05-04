## `hylang:pypy3.7`

```console
$ docker pull hylang@sha256:32489a3be5f1b367e3a60a4f7750f11dfdd31056acd11980930af3165811b86c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `hylang:pypy3.7` - linux; amd64

```console
$ docker pull hylang@sha256:9732b2f1f777595d7d95c735b3c56e97e40355574d36f99814154c9ef7db04ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74961249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55eae770537936c606923ed3c79077c9ef04b4539853de1e99b1a336e39e230f`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:04:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:04:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 13:04:20 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 13:04:20 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 20 Apr 2022 13:10:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Apr 2022 13:10:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Apr 2022 13:10:40 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Apr 2022 13:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Apr 2022 13:10:51 GMT
CMD ["pypy3"]
# Wed, 20 Apr 2022 19:20:31 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 19:20:31 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 19:20:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 19:20:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af090b5809ccdd741dfa2864f8b438bf453379e96e1faf8cc1dddc5724faf087`  
		Last Modified: Wed, 20 Apr 2022 13:16:29 GMT  
		Size: 1.1 MB (1066195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a79cf9baf345cf2065c75fe0962e90957bd397fd521e86ec9e6e8939af8e8b`  
		Last Modified: Wed, 20 Apr 2022 13:21:10 GMT  
		Size: 36.4 MB (36374158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc52a2542416a1e73da3d96706c988efa6b66139b52e18863f753e1963821f07`  
		Last Modified: Wed, 20 Apr 2022 13:21:03 GMT  
		Size: 3.0 MB (2970374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8831be233fc5d1eb814f48056d3809d4e1a031fb5b13c7ebfe5c471a04f3b2e1`  
		Last Modified: Wed, 20 Apr 2022 19:23:12 GMT  
		Size: 3.2 MB (3171543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b64ae05e6a77fd2c98d3b081799cc962a2dc647f72ded98560210dc94f9bd4d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70542799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0196e30d4925cabe08e740540281bfd3a89b4b31ad1107332b3323c4d03b45`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:33:33 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 11:33:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 11:33:35 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 20 Apr 2022 11:41:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Apr 2022 11:41:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Apr 2022 11:41:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Apr 2022 11:41:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Apr 2022 11:41:25 GMT
CMD ["pypy3"]
# Wed, 20 Apr 2022 19:12:06 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 19:12:07 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 19:12:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 19:12:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ef7b1773d7fbd647820466c9c16d4ef789627841311f8a7eedbc6edade9e9b`  
		Last Modified: Wed, 20 Apr 2022 11:50:10 GMT  
		Size: 849.4 KB (849438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b0763f257e9a9004aecf53e6d353e267413300bb893685afece68b93e24921`  
		Last Modified: Wed, 20 Apr 2022 11:55:07 GMT  
		Size: 33.7 MB (33706535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fe2d7fedde70346cae7e0393d5321117635cda1a11987d32c061f2c2325977`  
		Last Modified: Wed, 20 Apr 2022 11:55:02 GMT  
		Size: 2.7 MB (2749638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135c3307805b92791f535077948f48d86f3c3eeb737d024bfdb903973d5b76cc`  
		Last Modified: Wed, 20 Apr 2022 19:16:26 GMT  
		Size: 3.2 MB (3171387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; 386

```console
$ docker pull hylang@sha256:3757322a74c53e4ec59d6e438d4e1be3f421c3de21dc8ab3b586315add4239e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74695209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0096c58dc54a9eb28befd72bc229348ebfe3f5cfe0db16c4cf001dcf12208ae0`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 15:54:31 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 15:54:32 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 15:54:33 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 20 Apr 2022 16:02:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Apr 2022 16:02:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Apr 2022 16:02:29 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Apr 2022 16:02:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Apr 2022 16:02:44 GMT
CMD ["pypy3"]
# Wed, 20 Apr 2022 22:01:37 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 22:01:37 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 22:01:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 22:01:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8dbba903d3b66c7c29ee4f4f98982d17c18deda3c8218fb81a534d950a9324`  
		Last Modified: Wed, 20 Apr 2022 16:11:59 GMT  
		Size: 873.8 KB (873833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516f2ddefee528c57151812f5a638affb98ccbbb87a897e18fd944ced5ff644`  
		Last Modified: Wed, 20 Apr 2022 16:17:01 GMT  
		Size: 35.5 MB (35510901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9cb2ce6a69324161fb7e37ac9aa6d9d217c6578e6f6dddc8dfa44945edfd59`  
		Last Modified: Wed, 20 Apr 2022 16:16:55 GMT  
		Size: 2.7 MB (2749543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd39cae91fd8ef43b846763b8d8c26e23c24ec465cb52dbeba16c8d28b64e582`  
		Last Modified: Wed, 20 Apr 2022 22:06:12 GMT  
		Size: 3.2 MB (3171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - windows version 10.0.20348.643; amd64

```console
$ docker pull hylang@sha256:b5f5013cc19196672570d020dde82b03179630957ced3fc27ee6e3484586b386
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2277698532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1daf993612020cc3cd0e0fdc3c8e599a62be1f963f88d694ba51ed398208ec0`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 12:03:22 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:03:51 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:03:52 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 13 Apr 2022 12:18:22 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '8acb184b48fb3c854de0662e4d23a66b90e73b1ab73a86695022c12c745d8b00'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:18:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 13 Apr 2022 12:18:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 13 Apr 2022 12:19:40 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:19:41 GMT
CMD ["pypy3"]
# Wed, 27 Apr 2022 12:35:12 GMT
ENV HY_VERSION=1.0a4
# Wed, 27 Apr 2022 12:35:13 GMT
ENV HYRULE_VERSION=0.1
# Wed, 27 Apr 2022 12:36:01 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 27 Apr 2022 12:36:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ac23d5eccd67c034cb6932c218fb1737e542524efd6238e082ecdf54ae0ea`  
		Last Modified: Wed, 27 Apr 2022 12:07:12 GMT  
		Size: 627.8 KB (627831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc394bd04379f4961d1bd7dfb6e6b46f9617d3017c8b96a74b98e6166f48441`  
		Last Modified: Wed, 27 Apr 2022 12:07:29 GMT  
		Size: 15.8 MB (15750648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19529246a74ac80fe7f83fab4502ebf427265a76e628f281889a92fef1373d6`  
		Last Modified: Wed, 27 Apr 2022 12:07:11 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2456c0ae7f3d75b2e8750fb8b8d16a96831aa4ff323aac357f163b6153048f`  
		Last Modified: Wed, 27 Apr 2022 12:09:52 GMT  
		Size: 26.5 MB (26485169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a1a0cd95edc78e7d2a50ee54e1b9ff924a3cd54433018f69f0572d1c9d9a34`  
		Last Modified: Wed, 27 Apr 2022 12:09:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302d5dde9cd3316640f8503cb16ef39c7a79708595352f3edc2ce77c679f92f0`  
		Last Modified: Wed, 27 Apr 2022 12:09:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f5852e0be03d858cc4d799d5dd40f64e4402aa613517e8db74e965f5ead67f`  
		Last Modified: Wed, 27 Apr 2022 12:09:45 GMT  
		Size: 3.7 MB (3676120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3781d18b87af34372258b80b330d06b0e0745aa486357a74481c181b03a786`  
		Last Modified: Wed, 27 Apr 2022 12:09:42 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02df05d65923d1f4d5c60b9e0628c33330a3de055b47aaca98e5983bd71f016`  
		Last Modified: Wed, 04 May 2022 12:04:21 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8636c2f4f75e4c529c854fd2d62adf13ab3786b1a045c0086b2d5e97e0e877b`  
		Last Modified: Wed, 04 May 2022 12:04:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3015118beaba0c69f7ff9b369864606d2b99e03ae3b70763ed4c4f56963b4a1e`  
		Last Modified: Wed, 04 May 2022 12:04:26 GMT  
		Size: 4.2 MB (4192728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40300ad8649a0486465572aecd72b186fc084405862a14c73cbf72c5f5fbc84`  
		Last Modified: Wed, 04 May 2022 12:04:21 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - windows version 10.0.17763.2803; amd64

```console
$ docker pull hylang@sha256:ccacd1c626e50e659f89a3a6fca6c3b899f05bdeead21d3128da0e3a354acfd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2765418430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99124550c64914f824ec691a8525816570babf429bb96e2af0a615f80f1fa0d`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 12:07:17 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:08:21 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:08:22 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 13 Apr 2022 12:21:21 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '8acb184b48fb3c854de0662e4d23a66b90e73b1ab73a86695022c12c745d8b00'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:21:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 13 Apr 2022 12:21:24 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 13 Apr 2022 12:23:05 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:23:06 GMT
CMD ["pypy3"]
# Wed, 27 Apr 2022 12:36:14 GMT
ENV HY_VERSION=1.0a4
# Wed, 27 Apr 2022 12:36:14 GMT
ENV HYRULE_VERSION=0.1
# Wed, 27 Apr 2022 12:37:45 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 27 Apr 2022 12:37:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6280e5e39ac4a14fa88f197abb20b1fc792cc9c6d6d2fd44085bd53a539bafc4`  
		Last Modified: Wed, 27 Apr 2022 12:07:46 GMT  
		Size: 363.8 KB (363767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b7088285e3e1f7b7b482c1a8e109fce6cfeee3d2981fb3f4317f3e912ecd9a`  
		Last Modified: Wed, 27 Apr 2022 12:08:05 GMT  
		Size: 15.5 MB (15500317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f781342cd47f2f4c4b6da48009e296bb0054b18573d08b443a158ee688372e81`  
		Last Modified: Wed, 27 Apr 2022 12:07:46 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29d40942a373d4837beaee6ed71ded8170b9aeb5965199e52e82e0e884db037`  
		Last Modified: Wed, 27 Apr 2022 12:10:37 GMT  
		Size: 26.2 MB (26246697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778532f7592b09d2b8f8e6f5447d8ff12ac0d1f2b873ebb64c0716edf1eb4e8c`  
		Last Modified: Wed, 27 Apr 2022 12:10:07 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3cc3e713ee25058afc5413ef373529c22cc4a8d07061aa336fdefc33d78e3e`  
		Last Modified: Wed, 27 Apr 2022 12:10:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05bc4232fba508253e5af9b0e16f8702cc64af094f8dec9844bf87796f4024c`  
		Last Modified: Wed, 27 Apr 2022 12:10:11 GMT  
		Size: 3.4 MB (3425795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14cd7b9ff8e220e6e1ef3b7e2e4ead1ea2961c2deb9d8437bbbca95d932ddfb`  
		Last Modified: Wed, 27 Apr 2022 12:10:07 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536518e4374b1895474e5f61876629f0c6acc3095d22f7ec302e18562cd024cb`  
		Last Modified: Wed, 04 May 2022 12:04:36 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c377b369a85fc67b9bc3a02bcb1cb060d1bf553c443f3bc9e85745bc4cc361`  
		Last Modified: Wed, 04 May 2022 12:04:36 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a7fd471b1927564eb4f75a2d2504a432a556d6c2c69995996b2d09702b957`  
		Last Modified: Wed, 04 May 2022 12:04:40 GMT  
		Size: 4.0 MB (3950648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b889dcdc97f6b8b12e944c1f2bc0ddeb5ea117a47675997d72b99b7a6024e9a7`  
		Last Modified: Wed, 04 May 2022 12:04:36 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
