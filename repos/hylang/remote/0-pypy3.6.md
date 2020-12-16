## `hylang:0-pypy3.6`

```console
$ docker pull hylang@sha256:4d04468d01c75d93af83991a4cebeaaae694837ae069db64408122e44547a977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:0-pypy3.6` - linux; amd64

```console
$ docker pull hylang@sha256:1480dbc3e77047ebead61b773878fdbe1672818188ceae9c65ccbf48fa629a7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70962383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:086f6a255b1f15f169e734eb38c2fe225a73aa97b6a336e8857070fc49c6be47`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:21:03 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 19:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:21:10 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 19:21:10 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 19:22:31 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a' ;; 		arm64) pypyArch='aarch64'; sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b' ;; 		i386) pypyArch='linux32'; sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69' ;; 		s390x) pypyArch='s390x'; sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 22:26:18 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:26:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:26:18 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:26:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:26:35 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 22:48:37 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 22:48:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 22:48:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862ff65907287da7787a1512d3d8837f7bea201508670fdaa8a0edbd815e629c`  
		Last Modified: Fri, 11 Dec 2020 19:25:08 GMT  
		Size: 2.7 MB (2742693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6509f8f75bdfe6a2bfa071a33dcca1b6429f19a2be6ef768a59d65d761fa61d`  
		Last Modified: Fri, 11 Dec 2020 19:25:49 GMT  
		Size: 35.7 MB (35694261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bc1f79370fbff75ae12f43873707e940e8b5a8ed01a2842ca00c489c5f8f6b`  
		Last Modified: Tue, 15 Dec 2020 22:30:04 GMT  
		Size: 2.4 MB (2413556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7c3ba4ff78ba3d7c0d615ec70cdd9fdce8fa7523b7c1ab0ebc4d5f678d662f`  
		Last Modified: Tue, 15 Dec 2020 22:52:26 GMT  
		Size: 3.0 MB (3012578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.6` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:325fdb17053b9bd26f65acce58629193e58a066f1cde5caacf8462e43bc16639
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63361691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fedc1342aca2137aed369ad6abd7785f3403d01841ab2e02db2ced1a4cb7196`
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
# Fri, 11 Dec 2020 16:55:54 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a' ;; 		arm64) pypyArch='aarch64'; sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b' ;; 		i386) pypyArch='linux32'; sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69' ;; 		s390x) pypyArch='s390x'; sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 22:47:20 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:47:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:47:23 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:48:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:48:02 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 23:17:34 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:17:53 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:17:55 GMT
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
	-	`sha256:97da6e3285517e9b5b978da6105f91e27eb3d911871e2b73487004fa654f5399`  
		Last Modified: Fri, 11 Dec 2020 17:01:11 GMT  
		Size: 29.5 MB (29471058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959d297b0df85c93e9a05700420153910687e7cff2f181685f365a376c7219b8`  
		Last Modified: Tue, 15 Dec 2020 22:52:38 GMT  
		Size: 2.4 MB (2414633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad431c23970807973a7513ca5373e8ea450c304fdaf1cf8a11044c31695213f8`  
		Last Modified: Tue, 15 Dec 2020 23:22:41 GMT  
		Size: 3.0 MB (3013313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.6` - linux; 386

```console
$ docker pull hylang@sha256:dc87bae486d0c61c8b66386b30ae1149e8ef907f243d3138b3d7e444543708c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73931035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb70014297516357d6a0b6b44ca311006ef8ee60b91e5cd743a5c6e26df0f1e`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 22:18:45 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 22:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 22:18:55 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 22:18:55 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 22:21:36 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a' ;; 		arm64) pypyArch='aarch64'; sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b' ;; 		i386) pypyArch='linux32'; sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69' ;; 		s390x) pypyArch='s390x'; sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 23:03:03 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 23:03:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 23:03:04 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 23:03:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 23:03:23 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 23:46:36 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:46:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:46:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afc78f63aaea6458a1464eb07ba0cdb68d083175bebee11d5d502b846e12b1a`  
		Last Modified: Fri, 11 Dec 2020 22:25:40 GMT  
		Size: 2.8 MB (2752978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335377511c8ea3b6078dce069427f74b41c903fd2fab3afba4ed19e1f5fd6f45`  
		Last Modified: Fri, 11 Dec 2020 22:26:58 GMT  
		Size: 38.0 MB (37994743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8434cc90fa2b3065c1ef700a8a1f2c1679ca6dc04e76f2866ef288074e17044`  
		Last Modified: Tue, 15 Dec 2020 23:06:23 GMT  
		Size: 2.4 MB (2413267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ed9978e8045cae2f51bde6e5666a6a4398227a3294c884b3c85e94ba55b78`  
		Last Modified: Tue, 15 Dec 2020 23:50:23 GMT  
		Size: 3.0 MB (3012463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.6` - linux; s390x

```console
$ docker pull hylang@sha256:9c8e8bf4b66863ae72816e00bb8ff8bf7e76422035f591808576f30191f561a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66217638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a92ceaa654744600e467f109b9d86823cc8c8d2bbc88f7e6f2e6acbf9595450`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:19:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:20:01 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:20:02 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 11 Dec 2020 16:20:48 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='4fb85fdd516482cab727bb9473b066ff8fb672940dedf7ccc32bf92957d29e0a' ;; 		arm64) pypyArch='aarch64'; sha256='bc82cf7f0182b942a2cfad4a0d167f364bfbf18f434e100a2fe62bc88547ac9b' ;; 		i386) pypyArch='linux32'; sha256='f183c61e66fd2c536a65695bd7ff770748c2884c235a589b9c6ac63690770c69' ;; 		s390x) pypyArch='s390x'; sha256='0de9c33ff3500c6e7fd273d0a6d341bc839b0298f697c4d6fe141f2b54c5c3e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Dec 2020 21:43:51 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 21:43:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 21:43:52 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 21:44:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 21:44:08 GMT
CMD ["pypy3"]
# Tue, 15 Dec 2020 22:03:56 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 22:04:04 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 22:04:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1873488019a5a723e31f96e4bfefafcfd2bf9df4c7cbd724308f1aaaa9205d3`  
		Last Modified: Fri, 11 Dec 2020 16:25:26 GMT  
		Size: 2.4 MB (2432982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2792abcfee60efeb3ae7dc16b0480f596e1400364109fc4a24fb4bc7d93ddc74`  
		Last Modified: Fri, 11 Dec 2020 16:25:33 GMT  
		Size: 32.6 MB (32643947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86645a55a7bb7cb3f297daa8807ee900cef015f0e0bfe87f3f33029d2540bd2b`  
		Last Modified: Tue, 15 Dec 2020 21:46:20 GMT  
		Size: 2.4 MB (2413755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc490111084863e6bd70c8788ec90819f64d3cc4ebea4a1ed7410b99cb4308fe`  
		Last Modified: Tue, 15 Dec 2020 22:06:23 GMT  
		Size: 3.0 MB (3012997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
