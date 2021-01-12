## `hylang:0-pypy3.7`

```console
$ docker pull hylang@sha256:ac2cda3d9811cedfaa552c631f8b3daca1e51727f948099cb58a1b3599b0407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:0-pypy3.7` - linux; amd64

```console
$ docker pull hylang@sha256:8a1b06690b6860e18076d93f25fc7a663fcf9eeb315bd0f9a7e3dfa3046848e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73544313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3c5852e7f5c673f924b1d2bb0820d470040c563d0a463617db85682c04f35b`
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
# Tue, 12 Jan 2021 03:39:33 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 03:39:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 03:39:34 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 03:39:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 03:39:58 GMT
CMD ["pypy3"]
# Tue, 12 Jan 2021 23:06:19 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 23:06:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 23:06:30 GMT
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
	-	`sha256:ed5c485159d2760252631a6781b44f226cee6947b612381aa9c9ac396111488a`  
		Last Modified: Tue, 12 Jan 2021 03:43:22 GMT  
		Size: 2.6 MB (2564271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e223ee94c2f1a54a2970c4eb06ed5380c0f63d50913d1c8ea8a77dc1574a361`  
		Last Modified: Tue, 12 Jan 2021 23:09:49 GMT  
		Size: 3.1 MB (3076758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a22240478b34701b2aa2c0e4d47d97b8f5803e276eb31bde5368c088b4b2afbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65926322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cf91a301c773bebe4023f7b3fea12c0dde7ad38ea276a0443942dbd75b49c6`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:52:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:52:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:52:31 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 16:58:02 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='37e2804c4661c86c857d709d28c7de716b000d31e89766599fdf5a98928b7096' ;; 		arm64) pypyArch='aarch64'; sha256='ee4aa041558b58de6063dd6df93b3def221c4ca4c900d6a9db5b1b52135703a8' ;; 		i386) pypyArch='linux32'; sha256='7d81b8e9fcd07c067cfe2f519ab770ec62928ee8787f952cadf2d2786246efc8' ;; 		s390x) pypyArch='s390x'; sha256='92000d90b9a37f2e9cb7885f2a872adfa9e48e74bf7f84a8b8185c8181f0502d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 22:48:55 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:48:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:48:58 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:49:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:49:41 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 23:17:05 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:17:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:17:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f827548d2e9ffb879dc53392f8b6e3b31acc4faef6c0274f311cee165c7492f6`  
		Last Modified: Fri, 11 Dec 2020 17:00:07 GMT  
		Size: 2.6 MB (2606496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d2a3568588f414c8fc12cc4f6fd5f014d7e764adca66055acf25b29e82333b`  
		Last Modified: Fri, 11 Dec 2020 17:02:01 GMT  
		Size: 31.8 MB (31819922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0558efe3327bc9cb12b13c295c641fbf200cd14f4ba2e7238604aa6f9bfeafe1`  
		Last Modified: Tue, 15 Dec 2020 22:53:28 GMT  
		Size: 2.6 MB (2565634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237989ebcbc2258eb587652cd20028ccc48ca551ab621f879ccd6b7b0cdaf635`  
		Last Modified: Tue, 15 Dec 2020 23:22:24 GMT  
		Size: 3.1 MB (3078079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; 386

```console
$ docker pull hylang@sha256:f52bbc583863a01ace3e9ac515bae3586db9c9fb1c215860410a778b40982d77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76515656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfdbb167a8301398f927dd0c01b5a501c5dcd4a90cd6dd8bc109c89e489cd257`
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
# Tue, 12 Jan 2021 11:53:56 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 11:53:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 11:53:56 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 11:54:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 11:54:18 GMT
CMD ["pypy3"]
# Tue, 12 Jan 2021 21:49:19 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 21:49:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 21:49:31 GMT
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
	-	`sha256:cea6fb972811c44d371e4b5bdee0ab5b5d33c8535d9c1a4ae943c8058877e0a6`  
		Last Modified: Tue, 12 Jan 2021 12:00:11 GMT  
		Size: 2.6 MB (2563946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02491b565d6bb00a49c03b5dc618748785415d8b25e3fa85d152b3386f7d3350`  
		Last Modified: Tue, 12 Jan 2021 21:53:09 GMT  
		Size: 3.1 MB (3076926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.7` - linux; s390x

```console
$ docker pull hylang@sha256:6b5088e9575d37a51eb973f74212772cf2299fd3e1af011f1bd7211af31a5fa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68837250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9864a805cdd0b5b17fc4337be9dc1764761dcaf79fb01dc543040c0e5b80d5b1`
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
# Tue, 12 Jan 2021 09:58:51 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 12 Jan 2021 09:58:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 12 Jan 2021 09:58:51 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 12 Jan 2021 09:59:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 12 Jan 2021 09:59:15 GMT
CMD ["pypy3"]
# Tue, 12 Jan 2021 23:07:12 GMT
ENV HY_VERSION=0.19.0
# Tue, 12 Jan 2021 23:07:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 12 Jan 2021 23:07:27 GMT
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
	-	`sha256:192dd0f6c59b618cf4a1821b8f0f6396d69b4c20159a938052224992a045e13b`  
		Last Modified: Tue, 12 Jan 2021 10:22:04 GMT  
		Size: 2.6 MB (2564581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef8eefc49bdb106c3de9dbe1faadcc76b17c05c9385d2d4751abf171490c6bd`  
		Last Modified: Tue, 12 Jan 2021 23:19:59 GMT  
		Size: 3.1 MB (3077574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
