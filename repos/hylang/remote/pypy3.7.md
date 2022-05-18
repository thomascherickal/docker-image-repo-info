## `hylang:pypy3.7`

```console
$ docker pull hylang@sha256:17f503ecc740ec3925d49be3c35159362c3cfc668aee6ffd9928ceb23b9c166d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `hylang:pypy3.7` - linux; amd64

```console
$ docker pull hylang@sha256:7116017b1a5fba5796196d5470a122e1596d113019822e839d5d531d6ba33b81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74879001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead80fb315ece2756ea74d3a2ccc8726e8551cc5a7d93d23d7c00811ee3eb920`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:56:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:56:37 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:56:37 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:56:37 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 15:03:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 15:03:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 15:03:17 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 15:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 15:03:27 GMT
CMD ["pypy3"]
# Thu, 12 May 2022 02:09:10 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 02:09:10 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 02:09:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 02:09:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c63018a4470ab46343e549f63fb48115ea86ff959c6648bd44dbafbc02ddfe`  
		Last Modified: Wed, 11 May 2022 15:09:04 GMT  
		Size: 1.1 MB (1066234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb70941c7730a39394e4fa6c27141cacb079de41c9afef7329999a0c0e9efe6e`  
		Last Modified: Wed, 11 May 2022 15:13:26 GMT  
		Size: 36.3 MB (36290640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5c87a6983d4885fab72c82a9b74fbdadd30b54cb0edbbfe8b5eec65ed72ffc`  
		Last Modified: Wed, 11 May 2022 15:13:20 GMT  
		Size: 3.0 MB (2970524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf1e9b4379e646e5754b0973d859627db2162a2298c5f085a73bf61d7b2dc68`  
		Last Modified: Thu, 12 May 2022 02:13:28 GMT  
		Size: 3.2 MB (3172127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d8183f62eacbe1f3634018a6255011472af4300432ed0d3ad77742e9d27f9586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70459209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e70cca0ec75f40372aa26d04047f590fce9c04824157aeab137b053bdbceb01`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 08:22:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 08:22:38 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 08:22:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 08:22:40 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 08:30:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 08:30:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 08:30:31 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 08:30:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 08:30:45 GMT
CMD ["pypy3"]
# Thu, 12 May 2022 00:04:59 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 00:05:00 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 00:05:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 00:05:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaefd81ac55b34ce9901ddc18cf199396659fbe9aa9e9d3ab150d457b5d8238`  
		Last Modified: Wed, 11 May 2022 08:39:14 GMT  
		Size: 849.5 KB (849467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfab242cadac08a8e3230594105d0cb42e85c968e0c87bdf8fc265c8276ef5e`  
		Last Modified: Wed, 11 May 2022 08:44:06 GMT  
		Size: 33.6 MB (33622825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd904725fc4dd5df55d24712ff30c42f13f3e815034378f449a4d07cc1bbe9a7`  
		Last Modified: Wed, 11 May 2022 08:44:00 GMT  
		Size: 2.7 MB (2749488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0830d075555d9976565b7fa7601ef185b7ec890d49c3d91ca3fd172d81c281b4`  
		Last Modified: Thu, 12 May 2022 00:11:26 GMT  
		Size: 3.2 MB (3171736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - linux; 386

```console
$ docker pull hylang@sha256:914a95c486e30170583e17dce5025cac4cb209d17da6fe1d762e16439c0f6bf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74596141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f041484cd377db386ade7ad635969ed6cac81b92f003a1163cee57bfd333d4`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:42:10 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 10:42:11 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 10:42:12 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 10:50:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux64.tar.bz2'; 			sha256='c58195124d807ecc527499ee19bc511ed753f4f2e418203ca51bc7e3b124d5d1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-aarch64.tar.bz2'; 			sha256='dfc62f2c453fb851d10a1879c6e75c31ffebbf2a44d181bb06fcac4750d023fc'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-linux32.tar.bz2'; 			sha256='3398cece0167b81baa219c9cd54a549443d8c0a6b553ec8ec13236281e0d86cd'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.9-s390x.tar.bz2'; 			sha256='fcab3b9e110379948217cf592229542f53c33bfe881006f95ce30ac815a6df48'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 10:50:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 10:50:20 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 10:50:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 10:50:34 GMT
CMD ["pypy3"]
# Wed, 11 May 2022 19:58:33 GMT
ENV HY_VERSION=1.0a4
# Wed, 11 May 2022 19:58:33 GMT
ENV HYRULE_VERSION=0.1
# Wed, 11 May 2022 19:58:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 11 May 2022 19:58:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e43e2675131b3496a5f30db378ca53620a532d814a5fea2e9e5824ba6a3e1e1`  
		Last Modified: Wed, 11 May 2022 10:59:50 GMT  
		Size: 873.8 KB (873842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3493f54c13cd1aa2982cbde5e6719d58c806dac885d7e8824700de98dd15ff44`  
		Last Modified: Wed, 11 May 2022 11:04:55 GMT  
		Size: 35.4 MB (35411404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025554222f6bc6070f673409c16912dda38a63e5bb8c5e849aeacf612a794584`  
		Last Modified: Wed, 11 May 2022 11:04:50 GMT  
		Size: 2.7 MB (2749385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc5dd8b8e14bb0a3e9c35f8225af55324106c7d380b729538b7c3d8bf7a67b`  
		Last Modified: Wed, 11 May 2022 20:04:43 GMT  
		Size: 3.2 MB (3171734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - windows version 10.0.20348.707; amd64

```console
$ docker pull hylang@sha256:c41edc563d4a9f5b2754fac431f3f0c6464e94689354370986027f0945c8520a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288171083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6879f05376334c9e466ad2c96d3c0837ab7bbe4ff038abac50715b032ca06a09`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 12:04:19 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 May 2022 12:04:48 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:04:49 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 12:18:52 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '8acb184b48fb3c854de0662e4d23a66b90e73b1ab73a86695022c12c745d8b00'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:18:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 12:18:54 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 12:20:04 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:20:05 GMT
CMD ["pypy3"]
# Wed, 18 May 2022 12:33:47 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 12:33:48 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 12:34:34 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 18 May 2022 12:34:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856212015d3344ddeccfb9bc86716cbb73e023f931ec57f649eba5f92bfe3ba`  
		Last Modified: Wed, 18 May 2022 12:06:29 GMT  
		Size: 604.4 KB (604405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f806e77cf758e99e339f11b825191b78ac074c0e15df57c95ffa35234212c710`  
		Last Modified: Wed, 18 May 2022 12:06:44 GMT  
		Size: 15.7 MB (15727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b939be8ce96ba83671598e7fbe27585667afa6663b3f00274620dbe8bc53f82e`  
		Last Modified: Wed, 18 May 2022 12:06:28 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f33aab1f893763ff90cd59af31488d381aa38df2e4b70338219d057c99c5db4`  
		Last Modified: Wed, 18 May 2022 12:10:02 GMT  
		Size: 26.5 MB (26459479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893ef9fcab92e2a3e1e85f47b1575d228521f3a00a8cda1188243d815ec0a107`  
		Last Modified: Wed, 18 May 2022 12:09:33 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccd47dea152aec28bd20b41581f218294f52f399d7031103c01bc199038680d`  
		Last Modified: Wed, 18 May 2022 12:09:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143561370d59d7d48587b644e398585f3b64975367474d72b5cfa93e639cf59f`  
		Last Modified: Wed, 18 May 2022 12:09:37 GMT  
		Size: 3.6 MB (3647780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8c7fa72df558c678d6b41a1aa242fe592a6716b0d240861327ad48729fe072`  
		Last Modified: Wed, 18 May 2022 12:09:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc319c4870f843abdad481d4e492cbfef5f5b91269ed21bc2f9ebb4bf4383bfc`  
		Last Modified: Wed, 18 May 2022 12:37:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf99cb2721c9a37b66554bcf7fbc7919681e213ce3e47d0999bf96c3a3aa0f2`  
		Last Modified: Wed, 18 May 2022 12:37:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86c28ca1504173487b65bd1791af80c8dac38b6741de9b02344b28ae56b2b52`  
		Last Modified: Wed, 18 May 2022 12:37:44 GMT  
		Size: 4.2 MB (4185800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3e99fc6c322c6f1bbd1153dcfc9e91db3507eda5fa61093ffc47a40c0a22fe`  
		Last Modified: Wed, 18 May 2022 12:37:40 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7` - windows version 10.0.17763.2928; amd64

```console
$ docker pull hylang@sha256:d08b79fb703f7e17694e684dd8103e02c1a17eccc172520145ed629e7ea2ba7a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2553691524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97822c6b88a656be9bb249f79256db977194475f106240a968f7d6e2d09939c5`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 12:08:19 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 May 2022 12:09:16 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:09:17 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 12:21:32 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '8acb184b48fb3c854de0662e4d23a66b90e73b1ab73a86695022c12c745d8b00'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:21:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 12:21:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 12:23:09 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:23:11 GMT
CMD ["pypy3"]
# Wed, 18 May 2022 12:34:49 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 12:34:50 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 12:35:55 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 18 May 2022 12:35:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d2387a2c2f291aa6063bfd517e16a53cf5edf957859e74eee166038705a109`  
		Last Modified: Wed, 18 May 2022 12:07:02 GMT  
		Size: 486.1 KB (486116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d60b357cba6426f215b9ba70764743afe3d54199a19271133a07e58873f0586`  
		Last Modified: Wed, 18 May 2022 12:07:05 GMT  
		Size: 15.5 MB (15495601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d7014821b4c2a807d4879721798652cbfb821be75a3e58f40ebdd1a637aa58`  
		Last Modified: Wed, 18 May 2022 12:07:01 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db992ebe838173ea0b7d26c361d8ce9f1fbd33adb64dd8e932b3ef0f7af3cc52`  
		Last Modified: Wed, 18 May 2022 12:10:44 GMT  
		Size: 26.2 MB (26246182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168bf5229600378da68553ca05ab4e5c3cd7e322f849e360ded32dd24db2f427`  
		Last Modified: Wed, 18 May 2022 12:10:16 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd5b4703e5a1ab2155ba4ff47598107c9fd78faffee4938f1901bbc04ff3d30`  
		Last Modified: Wed, 18 May 2022 12:10:17 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b21bc096029eb8819edb25ac96abdd68c46e904bef221107109ee5ab224d0d6`  
		Last Modified: Wed, 18 May 2022 12:10:19 GMT  
		Size: 3.4 MB (3421627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e99760c43a60a78edb2878ce9b97546e5fea7b12db9b74059d31e6c691aeba`  
		Last Modified: Wed, 18 May 2022 12:10:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbbb245e0e1ccbcfa10822af2e1deb681ac711dbe6bcbb34ee75f22d8127d95`  
		Last Modified: Wed, 18 May 2022 12:37:54 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35672d3131440fa47c18676761d588069ce0fb92e062365004db2b5642c09b7b`  
		Last Modified: Wed, 18 May 2022 12:37:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e5093f90ac92efea16972da1913386c07e61ab9c4ab813667f12d4269d4807`  
		Last Modified: Wed, 18 May 2022 12:37:58 GMT  
		Size: 4.0 MB (3974922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bec64a11ed9397d4adf14ecafd11147f79b195c14b8e8941d3fa00f8bed30fe`  
		Last Modified: Wed, 18 May 2022 12:37:54 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
