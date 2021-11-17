## `pypy:2-7-slim-bullseye`

```console
$ docker pull pypy@sha256:7ca2ea44df338d9bfd4bcdfa33836e424a8e60fa2e02446bee1d8f4790e656bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-7-slim-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:88828ea4f56a3e526acecc77d5120e79608dbc5d4a6fef5dbf42cfe2ae5aec51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67465442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733471f9569065a833e7e950339ce07f128307bf8a59d72b2d035c641774d9c6`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 22:07:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:07:23 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 22:07:23 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 22:13:25 GMT
ENV PYPY_VERSION=7.3.6
# Wed, 17 Nov 2021 22:13:41 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux64.tar.bz2'; 			sha256='82127f43fae6ce75d47d6c4539f8c1ea372e9c2dbfa40fae8b58351d522793a4'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-aarch64.tar.bz2'; 			sha256='90e9aafb310314938f54678d4d6d7db1163b57c9343e640b447112f74d7f9151'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux32.tar.bz2'; 			sha256='7a1145f3a278ffab4da0e2d4c4bd024ab8d67106a502e4bb7f6d67337e7af2b7'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 22:13:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 22:13:41 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 22:13:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 22:13:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36ae8d36378f766e4bf6e364331a337e34f5a881b61993b8ca9baf2a7743e49`  
		Last Modified: Wed, 17 Nov 2021 22:17:25 GMT  
		Size: 1.1 MB (1065971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910da97ea11f27c7f88c4a6b5e339985b304b0a2766fd816ff54b6d6053ebd50`  
		Last Modified: Wed, 17 Nov 2021 22:22:13 GMT  
		Size: 32.9 MB (32858325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04797c84838ebf3a16c7bd4a0468e5d3c5ce361067829382a52ea8b5d88ac51d`  
		Last Modified: Wed, 17 Nov 2021 22:22:07 GMT  
		Size: 2.2 MB (2170879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:42fee096a45d71851d5e4c2357702a8ed182f70b49312424723d2c7bd9e54094
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63077327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cca0fe0c51322d6351f5b5e4a0becbe2dd01f32ec7cbe226d967a033414a8ea`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:02:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:02:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:02:44 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:07:36 GMT
ENV PYPY_VERSION=7.3.6
# Wed, 17 Nov 2021 09:07:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux64.tar.bz2'; 			sha256='82127f43fae6ce75d47d6c4539f8c1ea372e9c2dbfa40fae8b58351d522793a4'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-aarch64.tar.bz2'; 			sha256='90e9aafb310314938f54678d4d6d7db1163b57c9343e640b447112f74d7f9151'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux32.tar.bz2'; 			sha256='7a1145f3a278ffab4da0e2d4c4bd024ab8d67106a502e4bb7f6d67337e7af2b7'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 09:07:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 09:07:54 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 09:08:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 09:08:06 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e797d4308920fd5d5fa51c95d7155e468a717663a520a5e494d39b94b187d0a`  
		Last Modified: Wed, 17 Nov 2021 09:12:48 GMT  
		Size: 849.8 KB (849811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6a8095e93edd5ff5f7a2e8fa64589eb077aa81d238c6aa9b372198097266da`  
		Last Modified: Wed, 17 Nov 2021 09:16:06 GMT  
		Size: 30.2 MB (30216688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ff6676747c3a4528e3b576f41b8f0bdf2dca6f2c4e3e934c9a9adb579e879c`  
		Last Modified: Wed, 17 Nov 2021 09:16:01 GMT  
		Size: 2.0 MB (1954307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:59ac2ec12f279099b38a541ec018d6f4d5a777c920709a9c2a7781c9727af1b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65915193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5165d04286d22b1167a492fd37e94c58b1ec8508ac42e5a5b7fe1700ef47530b`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:55:24 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 19:55:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 20:04:44 GMT
ENV PYPY_VERSION=7.3.6
# Wed, 17 Nov 2021 20:05:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux64.tar.bz2'; 			sha256='82127f43fae6ce75d47d6c4539f8c1ea372e9c2dbfa40fae8b58351d522793a4'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-aarch64.tar.bz2'; 			sha256='90e9aafb310314938f54678d4d6d7db1163b57c9343e640b447112f74d7f9151'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.6-linux32.tar.bz2'; 			sha256='7a1145f3a278ffab4da0e2d4c4bd024ab8d67106a502e4bb7f6d67337e7af2b7'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 20:05:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 20:05:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 20:05:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 20:05:28 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3612a2d42ac8871dbb97f355e86cdfdc929b333c15e0ff44e596a30b9242d80`  
		Last Modified: Wed, 17 Nov 2021 20:13:07 GMT  
		Size: 1.1 MB (1078398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309f73e56e6be9ffdd91316165cd737a9185c4454f27cc2ad899f5aaa0493e1`  
		Last Modified: Wed, 17 Nov 2021 20:20:02 GMT  
		Size: 30.3 MB (30285351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9d62616e19c968113228b5c091745bc48ae75e731dfd625b724901a6d644ce`  
		Last Modified: Wed, 17 Nov 2021 20:19:50 GMT  
		Size: 2.2 MB (2170761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
