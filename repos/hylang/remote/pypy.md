## `hylang:pypy`

```console
$ docker pull hylang@sha256:da7a9db4b04582148bfa9bf4a207d8599b40fcfeb71c8d019f41e1a2131b884f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy` - linux; amd64

```console
$ docker pull hylang@sha256:cbab5912276dae8247ea269e078e9e876c6931575d0056ea2cc3156e9b14161c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78641956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac27c4bf03dd22a9faf53a5687b82adb2e544d0d5ab84910d96b7bc459e0d168`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:41:00 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 20:41:00 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 20:41:00 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 20 Sep 2023 20:41:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Sep 2023 20:41:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Sep 2023 20:41:33 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Sep 2023 20:41:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Sep 2023 20:41:46 GMT
CMD ["pypy3"]
# Thu, 21 Sep 2023 05:48:00 GMT
ENV HY_VERSION=0.27.0
# Thu, 21 Sep 2023 05:48:00 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 21 Sep 2023 05:48:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 21 Sep 2023 05:48:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc028031a1b2692c9fb5b157527a596d87c3b16385dc313052277b81db0d0229`  
		Last Modified: Wed, 20 Sep 2023 20:49:29 GMT  
		Size: 3.5 MB (3485379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba2f0d2af8e51866317e23e2e3d16a1e49490518b9e38d70f7c369566da8e0`  
		Last Modified: Wed, 20 Sep 2023 20:49:35 GMT  
		Size: 36.2 MB (36207683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4905a65f3d3c7fa1ce38d06292cb2b169c07f818c08ec8359ef879a2b70da`  
		Last Modified: Wed, 20 Sep 2023 20:49:29 GMT  
		Size: 3.5 MB (3511673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d405dc8b56a3412b0d47df35f26594819451e870b7134b31040ab5a9c60b59b`  
		Last Modified: Thu, 21 Sep 2023 05:54:34 GMT  
		Size: 6.3 MB (6312516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:2ae3dc1f3f1645d1dc99bb801862a0c3615a18a41ca21bbe84db874afb3aef96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75802935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d8cbe9730611c5a52dbdddfd416cf90ff103e88f3932e704244455380242b7`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:18:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:18:40 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 16:18:40 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 16:18:40 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 20 Sep 2023 16:19:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 20 Sep 2023 16:19:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 20 Sep 2023 16:19:08 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 20 Sep 2023 16:19:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 20 Sep 2023 16:19:21 GMT
CMD ["pypy3"]
# Wed, 20 Sep 2023 22:04:36 GMT
ENV HY_VERSION=0.27.0
# Wed, 20 Sep 2023 22:04:36 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 20 Sep 2023 22:05:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Sep 2023 22:05:08 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56ceaac6b073ab5073301f4703edeffc5231bc3dd919dde3d47d1523601be7`  
		Last Modified: Wed, 20 Sep 2023 16:26:02 GMT  
		Size: 3.3 MB (3311871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04b9b17886a708cbfa54c1675b342cd7d35ef2ffdc3653f2bee82a783b1053c`  
		Last Modified: Wed, 20 Sep 2023 16:26:06 GMT  
		Size: 33.5 MB (33509928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0a37945af9dee5dcefbd95123ec390f159e4cca7a1ed259764df729ca7787`  
		Last Modified: Wed, 20 Sep 2023 16:26:03 GMT  
		Size: 3.5 MB (3511556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663587fd7b75de4e9c1bb840b01949c18fa5f1946f8fd0e6d20cf7eca085a334`  
		Last Modified: Wed, 20 Sep 2023 22:11:50 GMT  
		Size: 6.3 MB (6312359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; 386

```console
$ docker pull hylang@sha256:7a7ffe4db309af218629f61d5049ebcb400fd3b8d9e5f9428a1a39d9df397fbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75590158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6f8dbe7f8a0ee8de949ca3f444a449fd06953c42a98519376b009dd434c359`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:00 GMT
ADD file:0952a54f5474629ed000e89bfd1b8827e49b63270932e45ed8d953a2676ac79c in / 
# Thu, 07 Sep 2023 00:39:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 19:46:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:46:00 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 19:46:01 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 19:46:01 GMT
ENV PYPY_VERSION=7.3.12
# Thu, 07 Sep 2023 19:46:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux64.tar.bz2'; 			sha256='6c577993160b6f5ee8cab73cd1a807affcefafe2f7441c87bd926c10505e8731'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-aarch64.tar.bz2'; 			sha256='26208b5a134d9860a08f74cce60960005758e82dc5f0e3566a48ed863a1f16a1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-linux32.tar.bz2'; 			sha256='811667825ae58ada4b7c3d8bc1b5055b9f9d6a377e51aedfbe0727966603f60e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.12-s390x.tar.bz2'; 			sha256='043c13a585479428b463ab69575a088db74aadc16798d6e677d97f563585fee3'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 07 Sep 2023 19:46:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 07 Sep 2023 19:46:42 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 07 Sep 2023 19:46:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Sep 2023 19:46:58 GMT
CMD ["pypy3"]
# Fri, 08 Sep 2023 06:48:29 GMT
ENV HY_VERSION=0.27.0
# Fri, 08 Sep 2023 06:48:29 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 08 Sep 2023 06:49:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 08 Sep 2023 06:49:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:30ae0f429560d1effd0839849ab7780512b72d9fbc09a6cec67e03092a85a1d1`  
		Last Modified: Thu, 07 Sep 2023 00:43:48 GMT  
		Size: 30.1 MB (30141753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0620241d024e7b1c780e92e4b6c77bbedcca1790c6e218f814025f232750eda9`  
		Last Modified: Thu, 07 Sep 2023 19:56:40 GMT  
		Size: 3.5 MB (3492719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21573e8ba747881947a7c03f08be0946f4f917d83e778cccb79d9a3ab92f5657`  
		Last Modified: Thu, 07 Sep 2023 19:56:46 GMT  
		Size: 32.1 MB (32131993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3884a4ef282dd2b74b410f23576e05f2240c1ccca7f153b6ec147e5e541388d8`  
		Last Modified: Thu, 07 Sep 2023 19:56:40 GMT  
		Size: 3.5 MB (3511330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2176cfe39035fcdec8fe8e46973f855be02579c8b1eb753da70c9e9549d101e4`  
		Last Modified: Fri, 08 Sep 2023 06:56:22 GMT  
		Size: 6.3 MB (6312363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
