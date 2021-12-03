## `hylang:pypy-bullseye`

```console
$ docker pull hylang@sha256:6b4cf43d764c5a1524c7bf241a4118e59898e26a461076d3b23f2d5cbbd7350d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:93e556536be0902ef2b617ec5e77a95227027dbd61845c7d3dbf88dfa2af0078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73455617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e1e73f6a5be86853817244e3fbecec5cbf891e942c7c6d24af49e8594780a9`
-	Default Command: `["hy"]`

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
# Wed, 17 Nov 2021 22:07:23 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 17 Nov 2021 22:07:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 22:07:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 22:07:57 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 22:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 22:08:08 GMT
CMD ["pypy3"]
# Thu, 18 Nov 2021 23:41:20 GMT
ENV HY_VERSION=1.0a3
# Thu, 18 Nov 2021 23:41:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 18 Nov 2021 23:41:29 GMT
CMD ["hy"]
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
	-	`sha256:1358f84c3b69100750dccdd42b24d04244ff48568b1206e3b0224cfdeddab826`  
		Last Modified: Wed, 17 Nov 2021 22:17:32 GMT  
		Size: 35.1 MB (35133919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517128f0165e0fbaabb7296a51de586374e4f6a89955bfc5312153dd298db98`  
		Last Modified: Wed, 17 Nov 2021 22:17:25 GMT  
		Size: 2.6 MB (2601868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4436b105bc19c64c52cd62937d195c3366600753440959e5f656f4baa70093c2`  
		Last Modified: Thu, 18 Nov 2021 23:45:53 GMT  
		Size: 3.3 MB (3283592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b9357d4426a82d395b81a5d726f2ecbea626f0d9d77747db324140f48822bbb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68856164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c206e9c68da8d3720f9fed89a98d8bbf59c49ad507a69ee5b6b10c7075edc664`
-	Default Command: `["hy"]`

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
# Wed, 17 Nov 2021 09:02:45 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 17 Nov 2021 09:03:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 09:03:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 09:03:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 09:03:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 09:03:35 GMT
CMD ["pypy3"]
# Wed, 17 Nov 2021 19:37:41 GMT
ENV HY_VERSION=1.0a3
# Wed, 17 Nov 2021 19:37:53 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 17 Nov 2021 19:37:54 GMT
CMD ["hy"]
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
	-	`sha256:6fa2902b838c22aeac1276513b710e43c1301654c396d2334083c563affdf3ef`  
		Last Modified: Wed, 17 Nov 2021 09:12:54 GMT  
		Size: 32.3 MB (32278399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b7e2f29d705597a6f17ec299767a93530ad4f8b0bc382c9371adb728376160`  
		Last Modified: Wed, 17 Nov 2021 09:12:49 GMT  
		Size: 2.4 MB (2386945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e613284240c607c3bdab26f7d0d3bd3b4c9b1231bf9145f01508cd78a7e7a171`  
		Last Modified: Wed, 17 Nov 2021 19:44:35 GMT  
		Size: 3.3 MB (3284488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:83ed0c8b40fea68d08ec474cd9c2dec51474f541e1626ff24b920d686e018415
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce0777ccff1bb37d34c82e0f2b7fa7695bcdeebf7ce425415ba669347f26623`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 15:07:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 15:07:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 15:07:56 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 15:07:56 GMT
ENV PYPY_VERSION=7.3.7
# Thu, 02 Dec 2021 15:08:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 02 Dec 2021 15:08:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 02 Dec 2021 15:08:32 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 02 Dec 2021 15:08:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 02 Dec 2021 15:08:47 GMT
CMD ["pypy3"]
# Fri, 03 Dec 2021 06:31:04 GMT
ENV HY_VERSION=1.0a3
# Fri, 03 Dec 2021 06:31:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 03 Dec 2021 06:31:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae0dda8434f840e922319294f80680afbb6f7668cb6731f02c3ba50822ec807`  
		Last Modified: Thu, 02 Dec 2021 15:25:25 GMT  
		Size: 1.1 MB (1078389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b00ab49b84f849962419a4a28cddbb330cfccd47e69b2bec7ce7284573c253`  
		Last Modified: Thu, 02 Dec 2021 15:25:35 GMT  
		Size: 34.5 MB (34544483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b7495b699d23ffeb883ffec27a3cdc1a2cdccd1e70cc98b0ccdafb6e526e6`  
		Last Modified: Thu, 02 Dec 2021 15:25:25 GMT  
		Size: 2.6 MB (2601542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101f2c5e35ebea6e7899fdead57ea1d81445d2bddd4bf9b80cb24337fa2d7ff`  
		Last Modified: Fri, 03 Dec 2021 06:40:19 GMT  
		Size: 3.3 MB (3283662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
