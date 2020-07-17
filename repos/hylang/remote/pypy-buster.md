## `hylang:pypy-buster`

```console
$ docker pull hylang@sha256:b4266d7aa0c033f446ebb041f3f082ef9c8a87312d5b81f0c630d4e2b665d516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:pypy-buster` - linux; amd64

```console
$ docker pull hylang@sha256:29e8ad0801863f1a9240e8b87d657fc29dddf3cb287407fad1854e2bea818e60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70667012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccfd09daff59adae40f3a27e1e299a0507ec2f304ab3f8f303ef3695fb0f62f9`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 00:31:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 00:31:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 00:31:22 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 00:31:22 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 17 Jun 2020 00:33:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Jun 2020 00:33:38 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 17 Jun 2020 00:33:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 17 Jun 2020 00:33:38 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 17 Jun 2020 00:33:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Jun 2020 00:33:54 GMT
CMD ["pypy3"]
# Thu, 16 Jul 2020 22:23:03 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 22:23:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Jul 2020 22:23:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97a53bc5d52d838fb7c85f5298f4b2bd07cc536b5c39080dde9ac69ff244e2b`  
		Last Modified: Wed, 17 Jun 2020 00:34:57 GMT  
		Size: 2.7 MB (2742451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bac09d21c73c1e3ccb858eb8bfa97707a689a07c2be5d1ec40fcd83eb7a310`  
		Last Modified: Wed, 17 Jun 2020 00:35:51 GMT  
		Size: 35.7 MB (35686846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef39bbb1883a233b063ea21c19c8d116fae8ad18ad1454f10f4f7975d9f0c314`  
		Last Modified: Wed, 17 Jun 2020 00:35:43 GMT  
		Size: 2.2 MB (2207053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481efee3058e6a3ed4fedb07d5f2b921602b198e7aceb904774987c9d918e4c2`  
		Last Modified: Thu, 16 Jul 2020 22:25:49 GMT  
		Size: 2.9 MB (2932397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:e75a932308de11e3ee76c6f2f74051fa30cb421629de5bdfa2790804410f383b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63090211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea0083a3f6932c62856d7c8eff0e0458609d8ba6d63a90e04e068c457623540a`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 01:17:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 01:17:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:17:35 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 01:17:36 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 17 Jun 2020 01:22:19 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Jun 2020 01:22:21 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 17 Jun 2020 01:22:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 17 Jun 2020 01:22:22 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 17 Jun 2020 01:22:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Jun 2020 01:22:59 GMT
CMD ["pypy3"]
# Thu, 16 Jul 2020 21:48:37 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 21:49:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Jul 2020 21:49:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed1db355fc46a30b243f69530bc0a46aef5231306c1563277cad68518f5d039`  
		Last Modified: Wed, 17 Jun 2020 01:24:55 GMT  
		Size: 2.6 MB (2606556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaaf3ac27a4c8fb9006c58fbffbd19c6802bec726ad56d1e8a51219a98e4028`  
		Last Modified: Wed, 17 Jun 2020 01:26:16 GMT  
		Size: 29.5 MB (29484423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e7e3da3369f0fe48c344182aa1dc862d459308d60cc3267f7c5518682e0b29`  
		Last Modified: Wed, 17 Jun 2020 01:26:04 GMT  
		Size: 2.2 MB (2208072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e6f5c998bb4f9b49a603d02ba480bee033a6c537ba71414cb2ab75a6534f3`  
		Last Modified: Thu, 16 Jul 2020 21:53:40 GMT  
		Size: 2.9 MB (2933456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-buster` - linux; 386

```console
$ docker pull hylang@sha256:48c551c628a64aa19dc1d37c98c36cc5b35b308374db35feaa0f6d57728b79a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73643763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec50a1d9e1c28cf39e9ff89fb39dc781bfda1b1ec2103dc7f78216cbdd02a747`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 00:46:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 00:46:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 00:46:26 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 00:46:27 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 17 Jun 2020 00:49:10 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Jun 2020 00:49:11 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 17 Jun 2020 00:49:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 17 Jun 2020 00:49:11 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 17 Jun 2020 00:49:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Jun 2020 00:49:30 GMT
CMD ["pypy3"]
# Thu, 16 Jul 2020 21:41:59 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 21:42:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Jul 2020 21:42:09 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc51cd1bef5ddf9965fc1598fd928ea2f88e82332da05dc45feab0532923fc9`  
		Last Modified: Wed, 17 Jun 2020 00:51:08 GMT  
		Size: 2.8 MB (2752696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d45322b2090da8b59b648f7e16f6e978523ffb34a46a4ee4abeecc3f32e89b`  
		Last Modified: Wed, 17 Jun 2020 00:52:15 GMT  
		Size: 38.0 MB (37997124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5637135f12254d5f3706c84e208c333bc3c3016fb6dfbe3649104a99be1fda68`  
		Last Modified: Wed, 17 Jun 2020 00:52:02 GMT  
		Size: 2.2 MB (2206803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a551b388eba70cde68ba6d2c3162a2b57a92e4406d67286479b12fef62e28dd`  
		Last Modified: Thu, 16 Jul 2020 21:44:48 GMT  
		Size: 2.9 MB (2932231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:a73d918ff059e580942f9dc35a3d307f1271fa747da966d9e2a68aac994f6f76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69021271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0970b92b180d76e08bf3e92f99e56c99c71e0670f198326ec030d10a8f3c539c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 00:49:07 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 00:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 00:50:00 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 00:50:31 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 17 Jun 2020 00:53:14 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Jun 2020 00:53:21 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 17 Jun 2020 00:53:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 17 Jun 2020 00:53:32 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 17 Jun 2020 00:54:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Jun 2020 00:54:14 GMT
CMD ["pypy3"]
# Thu, 16 Jul 2020 22:38:56 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 22:39:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Jul 2020 22:39:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa4f664f89e214924c309ffa3f796bfc6e86e6353b8eb24e675f0dbddb3efe8`  
		Last Modified: Wed, 17 Jun 2020 00:55:59 GMT  
		Size: 2.9 MB (2855706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1a2d49fedd7333d0d6ff0c179bbdab3d7560628c787c3d96207504d22af7`  
		Last Modified: Wed, 17 Jun 2020 00:56:08 GMT  
		Size: 30.5 MB (30498968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3725b3b9f7b742f451f6cba484e95c36c27467c53655fb0399bfa38cf225f6e2`  
		Last Modified: Wed, 17 Jun 2020 00:55:59 GMT  
		Size: 2.2 MB (2208403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1762881f254ee0498a0b88f2f8431658279bb9be1ba8cf9f34f9d8bbcaa07c`  
		Last Modified: Thu, 16 Jul 2020 22:47:15 GMT  
		Size: 2.9 MB (2933789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-buster` - linux; s390x

```console
$ docker pull hylang@sha256:80bd10529f280b016899950eb8cfde6828ef703945a03f11c7648d1ba54e5029
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65919640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e20b7dc7e24700ea6962b09f661d2c78f1e0662fab0d6bac617131366f4038`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 00:51:19 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 00:51:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 00:51:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 00:51:24 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 17 Jun 2020 00:51:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Jun 2020 00:51:48 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 17 Jun 2020 00:51:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 17 Jun 2020 00:51:48 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 17 Jun 2020 00:51:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Jun 2020 00:52:00 GMT
CMD ["pypy3"]
# Thu, 16 Jul 2020 21:46:55 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 21:47:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Jul 2020 21:47:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5674d6bc17674dc4130dae778e9560d372a136ab2736d660b4e9bab8dd6fcfe`  
		Last Modified: Wed, 17 Jun 2020 00:53:01 GMT  
		Size: 2.4 MB (2432841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e96ad48e2f75116f325184c1bfb39bee1e22db698192b13a37e75a563e16336`  
		Last Modified: Wed, 17 Jun 2020 00:53:13 GMT  
		Size: 32.6 MB (32634047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b26463a0cd4b3d863da2deeb2c1dae79087269e5e11b8a0128b088002f6c7d5`  
		Last Modified: Wed, 17 Jun 2020 00:53:17 GMT  
		Size: 2.2 MB (2207183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d756c53dec26fe05a2f4c33490bf6f5d5d57406f5f9e2e6d1353e8e15dbb51`  
		Last Modified: Thu, 16 Jul 2020 21:50:34 GMT  
		Size: 2.9 MB (2932901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
