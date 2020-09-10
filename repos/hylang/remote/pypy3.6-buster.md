## `hylang:pypy3.6-buster`

```console
$ docker pull hylang@sha256:4799761c578f0ce2a3b9583dfd9de88a66922523f0a4398a32e6a2fedb052195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:pypy3.6-buster` - linux; amd64

```console
$ docker pull hylang@sha256:cdaa2cc48dd485e1c443714ba73afd7e674afb88c6bcbfe13a17a134da27a3ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70859868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3632abc602da48be789616df02ea181c7aeffe37a83bdf902c2dcc63711b40`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:28:23 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 06:28:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:28:30 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 06:28:30 GMT
ENV PYPY_VERSION=7.3.1
# Wed, 05 Aug 2020 06:30:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Sep 2020 20:28:15 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:28:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:28:15 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:28:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:28:32 GMT
CMD ["pypy3"]
# Wed, 09 Sep 2020 01:04:51 GMT
ENV HY_VERSION=0.19.0
# Wed, 09 Sep 2020 01:05:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 09 Sep 2020 01:05:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba752debb3c3e0ed5c7d24db21b2548297fed7d74e1da6804f764e5c63d18fff`  
		Last Modified: Wed, 05 Aug 2020 06:31:52 GMT  
		Size: 2.7 MB (2742465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c80b4771d05e39d1df6c82b14ae4836dcf740374ea3ef38e2abcff35a59a5e9`  
		Last Modified: Wed, 05 Aug 2020 06:32:38 GMT  
		Size: 35.7 MB (35686864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538dce9d1e523c4ad7aa64e141b7ceb0778a7e0bdabde6b969ea13a24744a4c9`  
		Last Modified: Tue, 08 Sep 2020 20:30:14 GMT  
		Size: 2.4 MB (2395292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a67fd8e5d28b7d8fc168dd9ab618881fa2693d6070b91257ce0170bd2ad0907`  
		Last Modified: Wed, 09 Sep 2020 01:07:28 GMT  
		Size: 2.9 MB (2943126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:f4a8a20097d7fe9bf9ba006766d6c84459d56534bc380c16486e19557674a26f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63280842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb2f357fa3f7286fbaac8271cb02e99e86429bcfb8a92a31b67f6c9ef3447340`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:53:00 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 09:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 09:53:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Aug 2020 09:53:27 GMT
ENV PYPY_VERSION=7.3.1
# Tue, 04 Aug 2020 09:56:47 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Sep 2020 23:01:50 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 23:01:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 23:01:55 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 23:02:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 23:02:49 GMT
CMD ["pypy3"]
# Tue, 08 Sep 2020 23:53:07 GMT
ENV HY_VERSION=0.19.0
# Tue, 08 Sep 2020 23:53:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 08 Sep 2020 23:53:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ead8238ab6c3577178d87cecdfba4724b27518c235f3c352ca7b7232df97e0`  
		Last Modified: Tue, 04 Aug 2020 09:59:20 GMT  
		Size: 2.6 MB (2606653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdc4960e1ec3f88b442e3ab664683c5a1157f7aa673950b128523fe78df07e8`  
		Last Modified: Tue, 04 Aug 2020 10:00:11 GMT  
		Size: 29.5 MB (29484563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73acfdfe1c1bd436ec366063baad889de1f2ccdd0f72ebc04bc60bf5b9f64bb2`  
		Last Modified: Tue, 08 Sep 2020 23:05:25 GMT  
		Size: 2.4 MB (2396225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ff9bcf05b50c9c6184b123c5c1263a166c1e6fae9a7dca2eba1c7975916634`  
		Last Modified: Tue, 08 Sep 2020 23:57:50 GMT  
		Size: 2.9 MB (2944100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6-buster` - linux; 386

```console
$ docker pull hylang@sha256:50436688fb5e61c4da29b5e2899d0197f8ee04e7dc3eb1dfb7c30bbf9978651e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73838166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2464ff4d4b56921ec5b89c81e0c3964c3e8cb9633d2ae3d2dec131e6540c3822`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:22:22 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:22:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 15:22:34 GMT
ENV PYPY_VERSION=7.3.1
# Thu, 10 Sep 2020 15:25:43 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 10 Sep 2020 15:25:43 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 15:25:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 15:25:43 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 15:26:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 15:26:01 GMT
CMD ["pypy3"]
# Thu, 10 Sep 2020 21:19:40 GMT
ENV HY_VERSION=0.19.0
# Thu, 10 Sep 2020 21:19:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 10 Sep 2020 21:19:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4188f53dca4cf8543c8c5c4056a7c31bd176fd2b356c3a55f9189834ab833c2c`  
		Last Modified: Thu, 10 Sep 2020 15:27:40 GMT  
		Size: 2.8 MB (2752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f8b34f8fd5b76799cba80ebb157bf7f833fd8f54e4f9e18a0e5a34efb33aa2`  
		Last Modified: Thu, 10 Sep 2020 15:29:23 GMT  
		Size: 38.0 MB (37997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03386505e2210f47c9820b1a48e68cec9e36b9c5a9ec88126567ce45b04c8cd7`  
		Last Modified: Thu, 10 Sep 2020 15:29:12 GMT  
		Size: 2.4 MB (2394976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb8d9be377ef5f20f9d0428e0d084c60e9fe65981bad637da04a0a34c9439b6`  
		Last Modified: Thu, 10 Sep 2020 21:21:43 GMT  
		Size: 2.9 MB (2943012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:37c3d489653969aecea81bed01b8a9407959daf9af3685d42052512fe18b8768
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69214056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b2998655928bd2a1d29402418e9b14f013ce41f5db8d97835f41e94b4537ab`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:57:37 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 15:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:59:23 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Aug 2020 15:59:32 GMT
ENV PYPY_VERSION=7.3.1
# Tue, 04 Aug 2020 16:04:21 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Sep 2020 21:20:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:20:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:20:50 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:22:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:22:15 GMT
CMD ["pypy3"]
# Wed, 09 Sep 2020 00:01:40 GMT
ENV HY_VERSION=0.19.0
# Wed, 09 Sep 2020 00:03:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 09 Sep 2020 00:03:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e574ade0fff998b900879bc23d853090e208ab3a97185e5228d1329f59fa7f`  
		Last Modified: Tue, 04 Aug 2020 16:08:10 GMT  
		Size: 2.9 MB (2855740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75de69cc0b5846e05b161c1bd7f3150ec531de87eff9d6cb998e9aea42e5df30`  
		Last Modified: Tue, 04 Aug 2020 16:08:17 GMT  
		Size: 30.5 MB (30499205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa3794fcdc5c5d6cd3a58c65d9bc417ac1bc1d63459a3e7ecf2e56782be03b`  
		Last Modified: Tue, 08 Sep 2020 21:24:23 GMT  
		Size: 2.4 MB (2396655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6030615373b464978a0f77783e0509035e040a3088c9775e56bb5385a0f373ef`  
		Last Modified: Wed, 09 Sep 2020 00:11:06 GMT  
		Size: 2.9 MB (2944612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.6-buster` - linux; s390x

```console
$ docker pull hylang@sha256:56254318a034a279ec94019c8ec259426ea4f2cbfdf9c339811ff396acae6f5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66113536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad6b93d5e52698795d7b851cbdb2c1424e413b70d0a82ba0d9fefb744f0fe7b`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:34:35 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 04:34:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:34:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 04:34:40 GMT
ENV PYPY_VERSION=7.3.1
# Thu, 10 Sep 2020 04:34:59 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f67cf1664a336a3e939b58b3cabfe47d893356bdc01f2e17bc912aaa6605db12' ;; 		arm64) pypyArch='aarch64'; sha256='0069bc3c1570b935f1687f5e128cf050cd7229309e48fad2a2bf2140d43ffcee' ;; 		i386) pypyArch='linux32'; sha256='2e7a818c67f3ac0708e4d8cdf1961f30cf9586b3f3ca2f215d93437c5ea4567b' ;; 		ppc64el) pypyArch='ppc64le'; sha256='089fd806629ebf79cb0cb4b0c303d8665f360903b79f0df9214b58dbc42e8231' ;; 		s390x) pypyArch='s390x'; sha256='147592888e25678c1ae1c2929dc7420b3a0990117fdb25f235cb22476b4e4b5a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		patch 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://downloads.python.org/pypy/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		wget -O pypy-sqlite.patch 'https://foss.heptapod.net/pypy/pypy/commit/fbbe06715eb48df1a03640672d99335695d3e47c.patch'; 	awk '$1 == "diff" { yes = ($3 == "a/lib_pypy/_sqlite3.py") } yes { print }' pypy-sqlite.patch | patch --strip=1 --directory=/opt/pypy; 	rm pypy-sqlite.patch; 		ln -svT '/opt/pypy/bin/pypy3' '/usr/local/bin/pypy3'; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 10 Sep 2020 04:35:01 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 04:35:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 04:35:01 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 04:35:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 04:35:12 GMT
CMD ["pypy3"]
# Thu, 10 Sep 2020 08:16:09 GMT
ENV HY_VERSION=0.19.0
# Thu, 10 Sep 2020 08:16:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 10 Sep 2020 08:16:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25730a1e3b8989c53b55fae2816f43912b41a14a52a44f5c864cc37548d898b3`  
		Last Modified: Thu, 10 Sep 2020 04:36:21 GMT  
		Size: 2.4 MB (2432841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ff63ebb223a2afb0cae1118bb14ece781c37eaf97d4d847eba882bd38dbfba`  
		Last Modified: Thu, 10 Sep 2020 04:36:27 GMT  
		Size: 32.6 MB (32634057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159e285808c846ac5e3b9691ed5f29e38500addaea689355ad169e17d94ddc0`  
		Last Modified: Thu, 10 Sep 2020 04:36:21 GMT  
		Size: 2.4 MB (2395389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9861fd7645d474f94cf5a9828994fee386c4342033b3394f01d7708eb6f443c9`  
		Last Modified: Thu, 10 Sep 2020 08:17:57 GMT  
		Size: 2.9 MB (2943652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
