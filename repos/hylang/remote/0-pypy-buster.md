## `hylang:0-pypy-buster`

```console
$ docker pull hylang@sha256:7459113ac32b570ce5f9c9a950d5941bda5adb0204a6e9f34bf1f32d7787ba09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:0-pypy-buster` - linux; amd64

```console
$ docker pull hylang@sha256:540c02f726df13d6093ab1369dd81b1c263a20ea36a00684d86beccda6078c02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73549472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1e01f36e676146bee66adc70cf50cf257c865588b77bfb06654c1a1e421c92`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:36:28 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:36:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:36:36 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:36:36 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 12 Jan 2021 03:39:32 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 28 Jan 2021 22:44:53 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 28 Jan 2021 22:44:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 28 Jan 2021 22:44:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 28 Jan 2021 22:45:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 28 Jan 2021 22:45:11 GMT
CMD ["pypy3"]
# Thu, 28 Jan 2021 23:03:43 GMT
ENV HY_VERSION=0.20.0
# Thu, 28 Jan 2021 23:03:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Jan 2021 23:03:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197c25cb54733e53444257a84b7f8e2d7f246ebb208ccaeafdb0633999216d29`  
		Last Modified: Tue, 12 Jan 2021 03:41:36 GMT  
		Size: 2.7 MB (2742622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d44e7338b26e24af80ebe90b8b7f424d544f8642a03577f90da997a59def57`  
		Last Modified: Tue, 12 Jan 2021 03:43:29 GMT  
		Size: 38.1 MB (38052593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d96d976f39ada06011e9ac3968d5f4b51771a30f7038b70c497221e7bddcb`  
		Last Modified: Thu, 28 Jan 2021 22:47:22 GMT  
		Size: 2.6 MB (2564642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79802541a4c8aeec34de166daf30dcf6add39ac819b93fdc2daedb146958747c`  
		Last Modified: Thu, 28 Jan 2021 23:05:59 GMT  
		Size: 3.1 MB (3081546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:6964a11cb3f2dbdfe4c191343243b981178d0e8e0c9d3c0090853dfea4d66c68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65939192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fe35a6738d3d3ffa56b5015a1dd41fcad8a8d9363373b204a771833fbe8677`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:50:20 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:50:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:50:42 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 01:50:44 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 12 Jan 2021 01:57:47 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 28 Jan 2021 22:58:44 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 28 Jan 2021 22:58:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 28 Jan 2021 22:58:46 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 28 Jan 2021 22:59:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 28 Jan 2021 22:59:24 GMT
CMD ["pypy3"]
# Thu, 28 Jan 2021 23:19:43 GMT
ENV HY_VERSION=0.20.0
# Thu, 28 Jan 2021 23:20:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Jan 2021 23:20:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6c3568f616f90cc607df59faff41e552ae184ed16e25ebf7f6e7e4570c3edc`  
		Last Modified: Tue, 12 Jan 2021 02:00:59 GMT  
		Size: 2.6 MB (2606519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9dc218b30efc8365244544e5651fb5f8a1750b4da2960144b1f5a2a4fd3413`  
		Last Modified: Tue, 12 Jan 2021 02:04:12 GMT  
		Size: 31.8 MB (31819929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d2c6daa707081c6b33072f3fe87614ec57befe1e05e37556acf1083a9b4a5e`  
		Last Modified: Thu, 28 Jan 2021 23:02:55 GMT  
		Size: 2.6 MB (2565664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8993207a8449bab6db30570f2aa02d56038700a4c49e4dd9b6c160be2e130a`  
		Last Modified: Thu, 28 Jan 2021 23:22:31 GMT  
		Size: 3.1 MB (3082588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; 386

```console
$ docker pull hylang@sha256:c058ba1af222a7d86588fc5342684dcee521e63e2391ab71028f7aa5f41ce357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76520766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef19dad4f6c0c80599e98959a00706c36e6bd37e458a42000e7aa6cabbc0a4c1`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 11:48:33 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 11:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 11:48:46 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 11:48:47 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 12 Jan 2021 11:53:55 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 28 Jan 2021 22:42:52 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 28 Jan 2021 22:42:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 28 Jan 2021 22:42:52 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 28 Jan 2021 22:43:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 28 Jan 2021 22:43:11 GMT
CMD ["pypy3"]
# Thu, 28 Jan 2021 23:04:58 GMT
ENV HY_VERSION=0.20.0
# Thu, 28 Jan 2021 23:05:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Jan 2021 23:05:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b130eaa32a01790379a6c29b8975a689d1fe7ae060e921a32ed35d2d01b0bcf0`  
		Last Modified: Tue, 12 Jan 2021 11:57:05 GMT  
		Size: 2.8 MB (2752977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c2770c0baf80f6a878f8be18ea4c11a3256220550b04e049f501fd5cceb5a`  
		Last Modified: Tue, 12 Jan 2021 12:00:23 GMT  
		Size: 40.4 MB (40353816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2439369a7b20e40b2e4899045f2d478be2f8f6b0fa53a5d81ef48bbc23270b08`  
		Last Modified: Thu, 28 Jan 2021 22:45:33 GMT  
		Size: 2.6 MB (2564366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5208a6733f5b650ad7d8ef9f5ce0912a3922e9967f6a071e9c7ca525f2099746`  
		Last Modified: Thu, 28 Jan 2021 23:07:08 GMT  
		Size: 3.1 MB (3081616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; s390x

```console
$ docker pull hylang@sha256:e7f490dc5bd99136ea765cee18934f3e106ddc4a1a5280f4cae76648a0e27982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68842147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b9ce31727205d7bb228a7c998620477a8916355b274a7e37addf9718a296ce`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:56:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 09:56:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:56:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:56:30 GMT
ENV PYPY_VERSION=7.3.3
# Tue, 12 Jan 2021 09:58:48 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 28 Jan 2021 22:46:52 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 28 Jan 2021 22:46:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 28 Jan 2021 22:46:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 28 Jan 2021 22:47:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 28 Jan 2021 22:47:12 GMT
CMD ["pypy3"]
# Thu, 28 Jan 2021 23:15:13 GMT
ENV HY_VERSION=0.20.0
# Thu, 28 Jan 2021 23:15:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Jan 2021 23:15:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7277412244faf657e0387f2a8b82b450cb6bc8123401b24ef4bf19b7a71b95d6`  
		Last Modified: Tue, 12 Jan 2021 10:09:49 GMT  
		Size: 2.4 MB (2433038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6835ba59fe8e369c43982003f3ff176cc32178b488905caf7a2ced5e64409358`  
		Last Modified: Tue, 12 Jan 2021 10:22:16 GMT  
		Size: 35.0 MB (35038651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ae8df7a204c39046c10076565ec463a600c2dab01e547fcdec5cf828e05873`  
		Last Modified: Thu, 28 Jan 2021 22:49:17 GMT  
		Size: 2.6 MB (2564966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b05bbf21cd28edf4886b68e0c978a689f7f619fc71f99c6db94b56f41ca8f2`  
		Last Modified: Thu, 28 Jan 2021 23:17:46 GMT  
		Size: 3.1 MB (3082086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
