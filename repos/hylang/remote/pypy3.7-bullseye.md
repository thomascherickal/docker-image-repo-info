## `hylang:pypy3.7-bullseye`

```console
$ docker pull hylang@sha256:c441a40cdf06bf4ff32cdf8fcc72e86cdfb3a205aac34453b2261c4cb9c968fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.7-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:5496fc342595740df4ebf61ad577063374e8c3759d859c7702fd638d9fd44d25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72017081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b31453fb5d0cddebd9ccb5d3d2ae14fc190ce2a0bd42fdc9ffb5d98ff6bdb9b`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:03:49 GMT
ENV LANG=C.UTF-8
# Thu, 27 Jan 2022 02:03:49 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Feb 2022 01:24:11 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 23 Feb 2022 01:30:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64.tar.bz2'; 			sha256='4fb2f8281f3aaca72e6fe62ecc5fc054fcc79cd061ca3e0eea730f7d82d610d4'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 23 Feb 2022 01:30:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 23 Feb 2022 01:30:01 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 23 Feb 2022 01:30:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 23 Feb 2022 01:30:11 GMT
CMD ["pypy3"]
# Wed, 23 Feb 2022 02:00:34 GMT
ENV HY_VERSION=1.0a4
# Wed, 23 Feb 2022 02:00:34 GMT
ENV HYRULE_VERSION=0.1
# Wed, 23 Feb 2022 02:00:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 23 Feb 2022 02:00:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a83cdbef0c4ef2c4d58637a5627be3ec26cbc814f2d2ef6b869ed259874a58`  
		Last Modified: Thu, 27 Jan 2022 02:14:53 GMT  
		Size: 1.1 MB (1065969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6316aea514a58b272a92dc49d5e9c999094a727c9575349d439c778eb19e77`  
		Last Modified: Wed, 23 Feb 2022 01:40:07 GMT  
		Size: 34.7 MB (34664961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ea475ef14af7dd43f466d3d8a0fa9793851f50432ad66031806604e5c6c868`  
		Last Modified: Wed, 23 Feb 2022 01:40:01 GMT  
		Size: 2.4 MB (2371214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a737468e099c7f87800766bda8404d70d668a134f487ad3101260d3c5c3362fd`  
		Last Modified: Wed, 23 Feb 2022 02:02:53 GMT  
		Size: 2.5 MB (2548680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:07fdd9c6b8ec034c6200ae6f5feb8d04096bcaf376792ddad0c9d7a8341480ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68257883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab18175f2c679862afa3ad828ffa8b24530b610fbff5edaa76920761df96a02`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:16:32 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:16:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 07:16:34 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 26 Jan 2022 07:20:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 26 Jan 2022 07:20:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 26 Jan 2022 07:20:37 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 26 Jan 2022 07:20:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 07:20:50 GMT
CMD ["pypy3"]
# Thu, 27 Jan 2022 01:40:42 GMT
ENV HY_VERSION=1.0a4
# Thu, 27 Jan 2022 01:40:42 GMT
ENV HYRULE_VERSION=0.1
# Thu, 27 Jan 2022 01:40:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 27 Jan 2022 01:40:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d332b8dc1bea2b1e4430228d6b8623218bd585e47857521ff520e5a97cc0892`  
		Last Modified: Wed, 26 Jan 2022 07:29:13 GMT  
		Size: 1.1 MB (1053980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce70a01b9a42b17e8b8adb7517def8ae1e49e2f08f54abab9546772abeb98a12`  
		Last Modified: Wed, 26 Jan 2022 07:31:17 GMT  
		Size: 32.5 MB (32457862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c76ea4d09262a018e51a40b9ca1ed97c9c6afa123fc4de50bb8cbd29b5cc527`  
		Last Modified: Wed, 26 Jan 2022 07:31:11 GMT  
		Size: 2.2 MB (2155731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffd422a1249c00b49d13d54c09797a86b0d185c0c20b5cb3b5033993348587d`  
		Last Modified: Thu, 27 Jan 2022 01:46:11 GMT  
		Size: 2.5 MB (2533536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:a59f23220f82ff204cc2d6cf57ddd6936910acea3226b5c1ff503a88f6d2d3ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72305948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c3cb0e30903015e323fdab467d6722a64f1e57dab0f142964ea08fd1fc9cfc`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 21:15:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:15:39 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 21:15:40 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Feb 2022 01:45:01 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 23 Feb 2022 01:51:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64.tar.bz2'; 			sha256='4fb2f8281f3aaca72e6fe62ecc5fc054fcc79cd061ca3e0eea730f7d82d610d4'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 23 Feb 2022 01:51:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 23 Feb 2022 01:51:41 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 23 Feb 2022 01:51:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 23 Feb 2022 01:51:52 GMT
CMD ["pypy3"]
# Wed, 23 Feb 2022 02:28:38 GMT
ENV HY_VERSION=1.0a4
# Wed, 23 Feb 2022 02:28:38 GMT
ENV HYRULE_VERSION=0.1
# Wed, 23 Feb 2022 02:28:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 23 Feb 2022 02:28:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4290f5bd0570d5b05b3e56fe28aae36e64a91d62b9536c9738b84821f106c`  
		Last Modified: Wed, 26 Jan 2022 21:31:25 GMT  
		Size: 1.1 MB (1078383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8656b6eb5d8fa6d9a8ad552d517e1d1bb563fc1fcc24395435a19610ae5d500`  
		Last Modified: Wed, 23 Feb 2022 02:06:21 GMT  
		Size: 33.9 MB (33930399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6a13726101a7f0f707db3b385347948bc4fc548f170c635748833846efda25`  
		Last Modified: Wed, 23 Feb 2022 02:06:13 GMT  
		Size: 2.4 MB (2370962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7902ddfce38823da5ba3e46a0b08eefe4833c4ae294dab964d75a8ad837ac064`  
		Last Modified: Wed, 23 Feb 2022 02:32:43 GMT  
		Size: 2.5 MB (2548798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
