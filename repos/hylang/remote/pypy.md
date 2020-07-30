## `hylang:pypy`

```console
$ docker pull hylang@sha256:ce72072d72d856c78079ff559e82efec7dbde5591777183c0be6697629b6fdd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:pypy` - linux; amd64

```console
$ docker pull hylang@sha256:6c05b55cbcceca07c41ac1dd1f35ea50a6a72cc90982eb46d82ae85d4cf3a684
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70841846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d6bef34c9d5a7f0deedf3559006a64f1e9c8b2b77a4f4fe408ad965a5426b2`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 12:04:06 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 12:04:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 12:04:14 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 12:04:14 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 22 Jul 2020 12:06:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 22 Jul 2020 12:06:38 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 22 Jul 2020 12:06:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 22 Jul 2020 12:06:38 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 22 Jul 2020 12:06:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 22 Jul 2020 12:06:55 GMT
CMD ["pypy3"]
# Thu, 23 Jul 2020 06:44:23 GMT
ENV HY_VERSION=0.19.0
# Thu, 23 Jul 2020 06:44:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 23 Jul 2020 06:44:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b8692a0fa0527389efb37c557750b23c6e4fb7d19800e050ec9b00182affe6`  
		Last Modified: Wed, 22 Jul 2020 12:07:55 GMT  
		Size: 2.7 MB (2742457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da38d528ab2390abf43df9f1867d920c84fd91e4267c5ea6c99f4dbea852ddd0`  
		Last Modified: Wed, 22 Jul 2020 12:08:48 GMT  
		Size: 35.7 MB (35686804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc30854cc304c8a2f54106a540f705019e9c1e0e984cf16dac1816d0cf1bc5c`  
		Last Modified: Wed, 22 Jul 2020 12:08:39 GMT  
		Size: 2.4 MB (2381064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb1bc0a2119c0ba1bfc94abe6719769d252fd14031289201ad037405a2b95bd`  
		Last Modified: Thu, 23 Jul 2020 06:46:23 GMT  
		Size: 2.9 MB (2932977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:13d99d5476ed73df853ec53f3aaadf3205bd61da390085f55ec93c1a531735c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63264554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4807f2ad3b6a5330dd58e56d4c27017009fec4557a320e97b24e4f517c8529d9`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 15:29:16 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 15:29:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 15:29:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 15:29:34 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 22 Jul 2020 15:33:20 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 22 Jul 2020 15:33:23 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 22 Jul 2020 15:33:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 22 Jul 2020 15:33:25 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 22 Jul 2020 15:33:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 22 Jul 2020 15:34:01 GMT
CMD ["pypy3"]
# Thu, 23 Jul 2020 04:31:56 GMT
ENV HY_VERSION=0.19.0
# Thu, 23 Jul 2020 04:32:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 23 Jul 2020 04:32:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346f4494a8b3b1bfa66927c94fd9f1c236d438a8044d0e2689e5926c21ccc62`  
		Last Modified: Wed, 22 Jul 2020 15:35:30 GMT  
		Size: 2.6 MB (2606549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a5edd6eaf612cc48458faffeffdcb07e6a0df9eb91417421fcadd32c05a545`  
		Last Modified: Wed, 22 Jul 2020 15:36:50 GMT  
		Size: 29.5 MB (29484538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bf24f572c1a3b565a9d67c5d04724410ca78f8aa08d578c34cd294c023cb34`  
		Last Modified: Wed, 22 Jul 2020 15:36:40 GMT  
		Size: 2.4 MB (2381889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a79bf0bd42b94341ac8aa2de20f68d8b43cda1f22f5396a1d3234684812e6b5`  
		Last Modified: Thu, 23 Jul 2020 04:34:59 GMT  
		Size: 2.9 MB (2933752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; 386

```console
$ docker pull hylang@sha256:b8f95d3bfbf7116819738e2b17ee5754cee46b1d0e819657cd3a97284742bdee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73818440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58be13ec2463497fdcad82bafdd298a01de408dcf91adf7a48557c1bd497ac10`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 12:14:42 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 12:14:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 12:14:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 12:14:50 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 22 Jul 2020 12:17:16 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 22 Jul 2020 12:17:17 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 22 Jul 2020 12:17:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 22 Jul 2020 12:17:17 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 22 Jul 2020 12:17:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 22 Jul 2020 12:17:45 GMT
CMD ["pypy3"]
# Wed, 22 Jul 2020 23:49:26 GMT
ENV HY_VERSION=0.19.0
# Wed, 22 Jul 2020 23:49:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 22 Jul 2020 23:49:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68151976a15217c11f10871e573301c49eaeca9eaeb4a9904d8eddb12a4152`  
		Last Modified: Wed, 22 Jul 2020 12:19:14 GMT  
		Size: 2.8 MB (2752691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75935bd56645b00c4ca298fcfc8b7db6c8047d9fb2e17e7c6aabc5a5c086f184`  
		Last Modified: Wed, 22 Jul 2020 12:20:36 GMT  
		Size: 38.0 MB (37997095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd634c6f8284dbc8bd79c77aca243e063cbc66deb23287049435106d0bb0dfca`  
		Last Modified: Wed, 22 Jul 2020 12:20:15 GMT  
		Size: 2.4 MB (2380751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ed0dd251d47ab35aa0f3f8004b38e96b187cb22255637364a277e9836b0653`  
		Last Modified: Wed, 22 Jul 2020 23:51:59 GMT  
		Size: 2.9 MB (2933004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; ppc64le

```console
$ docker pull hylang@sha256:ce798f408e55ab89e88bf19466a451923aed8dd61958471c1ba7101ccfa4c1f7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69224055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf32dcbe9dae5db1c4b0cc8102b15c4c9fda22465a9c1fec661086a45fe140f1`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 14:07:01 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 14:07:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 14:07:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 14:08:02 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 22 Jul 2020 14:11:42 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 30 Jul 2020 22:25:37 GMT
ENV PYTHON_PIP_VERSION=20.2
# Thu, 30 Jul 2020 22:25:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/cb5b85a8e0c3d13ced611b97816d7490d2f1497e/get-pip.py
# Thu, 30 Jul 2020 22:25:47 GMT
ENV PYTHON_GET_PIP_SHA256=a30ff8a3446c592c6d70403a82483716e7b759e8eecba2c8d3f6ecfb34a8d6d7
# Thu, 30 Jul 2020 22:28:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 30 Jul 2020 22:28:30 GMT
CMD ["pypy3"]
# Thu, 30 Jul 2020 22:51:39 GMT
ENV HY_VERSION=0.19.0
# Thu, 30 Jul 2020 22:52:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 30 Jul 2020 22:52:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a327eb67cc833bea3ccf49ca84426b30b87d2496ae3647c1ce629bebd56fb`  
		Last Modified: Wed, 22 Jul 2020 14:15:09 GMT  
		Size: 2.9 MB (2855673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958c252ccaf3d42458563642b85fb9a9150731f876bd2616aa72800710ff8f99`  
		Last Modified: Wed, 22 Jul 2020 14:15:17 GMT  
		Size: 30.5 MB (30499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20a975908368c01bbc65754514f90aab9e5d5bd1a962be396c665323259968a`  
		Last Modified: Thu, 30 Jul 2020 22:30:12 GMT  
		Size: 2.4 MB (2394979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af347d953eed01b5ea24b4a0855d45fe1d01d6a999e13c3555dba3fa12cd0e1`  
		Last Modified: Thu, 30 Jul 2020 22:55:02 GMT  
		Size: 2.9 MB (2949799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; s390x

```console
$ docker pull hylang@sha256:c22fb49669fae34ca0468c78101bfa6faf6e4f9197e76c54198b03c8587fb74b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66122501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254babd29aac012f8370739d37b6d8125d1d2570fbee346376a35800364ee5c5`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 04:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 04:49:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 04:49:20 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 04:49:20 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 22 Jul 2020 04:49:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 30 Jul 2020 22:44:04 GMT
ENV PYTHON_PIP_VERSION=20.2
# Thu, 30 Jul 2020 22:44:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/cb5b85a8e0c3d13ced611b97816d7490d2f1497e/get-pip.py
# Thu, 30 Jul 2020 22:44:04 GMT
ENV PYTHON_GET_PIP_SHA256=a30ff8a3446c592c6d70403a82483716e7b759e8eecba2c8d3f6ecfb34a8d6d7
# Thu, 30 Jul 2020 22:44:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 30 Jul 2020 22:44:16 GMT
CMD ["pypy3"]
# Thu, 30 Jul 2020 23:02:48 GMT
ENV HY_VERSION=0.19.0
# Thu, 30 Jul 2020 23:02:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 30 Jul 2020 23:02:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc40667d28e89059eabf8219519331e5ac2b4f40729f2a469c0fb61915b47f8`  
		Last Modified: Wed, 22 Jul 2020 04:50:50 GMT  
		Size: 2.4 MB (2432835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca8cc5491e3cf6c74ea7cdc217d8cb14073fbe4b8063e07584295a555d01cb`  
		Last Modified: Wed, 22 Jul 2020 04:50:56 GMT  
		Size: 32.6 MB (32633988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3968c7263be2ce04432ec9ba5c170dea727a90725b45ad026ca2190504294bc`  
		Last Modified: Thu, 30 Jul 2020 22:44:51 GMT  
		Size: 2.4 MB (2393710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3703b92dbbe50fabd0f042f6ddd9da70019befe858afb182c7de806478750`  
		Last Modified: Thu, 30 Jul 2020 23:05:27 GMT  
		Size: 2.9 MB (2949148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
