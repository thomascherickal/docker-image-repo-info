## `hylang:0-pypy-buster`

```console
$ docker pull hylang@sha256:1b874e43ae8d5959d4a4db4107794e9b1b4f461ca0dbbf4ee405d1c0d6c26448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-pypy-buster` - linux; amd64

```console
$ docker pull hylang@sha256:3a6514ba6982d0fc28e985b721f8194a448fc4c0bd0f9dd9d4e5f517db660007
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74969332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c496dc6fa18973e165a19607a4bd4e15697f64d85c934929d84b88c72acb864`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:49:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:49:53 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 13:49:53 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 13:49:53 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 13:53:14 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 13:53:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 13:53:14 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 13:53:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 13:53:27 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 23:10:51 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 23:10:51 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 23:11:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 23:11:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf539a507ae1f36f9ada1f280153caf00388f19270985ba5667ac025af37ff5b`  
		Last Modified: Tue, 15 Nov 2022 14:01:08 GMT  
		Size: 2.8 MB (2768026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb488cebb090b7abf9f3b2fb8262839638814f5b98807096cbef32d8b931ce65`  
		Last Modified: Tue, 15 Nov 2022 14:03:16 GMT  
		Size: 37.9 MB (37860917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbe1c636be844abe883f6d62cd80b3e9a3518bd361f57b91044bfbac3578a56`  
		Last Modified: Tue, 15 Nov 2022 14:03:10 GMT  
		Size: 3.2 MB (3168310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f7ada93abbbf494c4bd2e9b67667352770b2dccc51ff89b84e9c3509148ddd`  
		Last Modified: Tue, 15 Nov 2022 23:19:21 GMT  
		Size: 4.0 MB (4031747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:0540c102dd84305ae6efd97f7050dc33175588b1131b5a67d14bf6191696f4dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70751556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc50766864a4a81368859aec17c53ae22c04eaad748c01e70d4c19b4b31072d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:11:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:11:34 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 07:11:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 07:11:34 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 07:14:20 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 07:14:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 07:14:20 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 07:14:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 07:14:37 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 21:58:05 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 21:58:06 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 21:58:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 21:58:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5059a2d6ab02eb1e0ed6415dfe6a05fc6d678698e3339a15487717fb34144390`  
		Last Modified: Tue, 15 Nov 2022 07:22:01 GMT  
		Size: 2.6 MB (2636566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe44357eeed4cd7acfb91f939d0e7f3641c1ff4ce95319284d8db1ef82cc2e`  
		Last Modified: Tue, 15 Nov 2022 07:24:12 GMT  
		Size: 35.0 MB (35000334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aded69aeac9bc559de0dba58b21464e8ebb69b741472e635849dee1c3adb609`  
		Last Modified: Tue, 15 Nov 2022 07:24:08 GMT  
		Size: 3.2 MB (3167941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e537d92011b01770034db709ab43bbcce1b206fa51a95c952776150e24507d27`  
		Last Modified: Tue, 15 Nov 2022 22:07:06 GMT  
		Size: 4.0 MB (4031791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; 386

```console
$ docker pull hylang@sha256:52457dc8ca0c49bf8fa3bcf1f87c3c46fb0d74ce8dd796b231ecfd77cf791f69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77234317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a53bff4a5303180bbdff568972053328b8cec3151f9a102abed4b0c2c79cfef6`
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
# Tue, 15 Nov 2022 09:30:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 09:30:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 09:30:07 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 09:30:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 09:30:22 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 19:47:53 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 19:47:54 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 19:48:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 19:48:35 GMT
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
	-	`sha256:c342c15f24a57cedadda147712d3c9caee3fc7d9b7d6db38da80a3c03df63797`  
		Last Modified: Tue, 15 Nov 2022 09:44:44 GMT  
		Size: 39.7 MB (39671632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830bfe01bb72cdde8c007775b02b3a008c93c8daad6a2412df1ac1ec8749525d`  
		Last Modified: Tue, 15 Nov 2022 09:44:38 GMT  
		Size: 3.0 MB (2951497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a154854327c0b1ac2e78e77760cdfa2b31c99894247a36ac01bb5635d0bd936`  
		Last Modified: Tue, 15 Nov 2022 20:01:31 GMT  
		Size: 4.0 MB (4031733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
