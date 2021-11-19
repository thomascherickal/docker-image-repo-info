## `hylang:pypy`

```console
$ docker pull hylang@sha256:a5e59e9d61e3e42bee67de5251799259e861966e3950cf018146455754ab4968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.2300; amd64

### `hylang:pypy` - linux; amd64

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

### `hylang:pypy` - linux; arm64 variant v8

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

### `hylang:pypy` - linux; 386

```console
$ docker pull hylang@sha256:ca46bc6e7d02f70ccee39b9023cac5f412d5126524379417cb3de2ba97132103
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0b14c3967c4eddb81f483125a279ad466666126e22c119c133b2756454bc7c`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:55:24 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 19:55:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 19:55:24 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 17 Nov 2021 19:56:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 17 Nov 2021 19:56:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 17 Nov 2021 19:56:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 17 Nov 2021 19:56:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 19:56:30 GMT
CMD ["pypy3"]
# Thu, 18 Nov 2021 00:26:55 GMT
ENV HY_VERSION=1.0a3
# Thu, 18 Nov 2021 00:27:04 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 18 Nov 2021 00:27:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3612a2d42ac8871dbb97f355e86cdfdc929b333c15e0ff44e596a30b9242d80`  
		Last Modified: Wed, 17 Nov 2021 20:13:07 GMT  
		Size: 1.1 MB (1078398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaca3cbbc8d09df4e4bf4af4b47d72268c10619281894786be69d740da43096`  
		Last Modified: Wed, 17 Nov 2021 20:13:16 GMT  
		Size: 34.5 MB (34544485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a4da072406febb1d6bffee12c259887aa0d561cc8944b7b92fb467e6fa2b55`  
		Last Modified: Wed, 17 Nov 2021 20:13:08 GMT  
		Size: 2.6 MB (2601564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53352370b18b15e8014bea4c6d94cb52f8718dc7fb306200da8ebbd54948ae57`  
		Last Modified: Thu, 18 Nov 2021 00:34:19 GMT  
		Size: 3.3 MB (3283574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - windows version 10.0.17763.2300; amd64

```console
$ docker pull hylang@sha256:8533c64e1faa735ae5d39dc1fdaf4af73d541f7b44942c66bd17f04d664ada08
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2756220333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05bc45c7df364aa7156859cb0481ad588cb38883d6fbd686e89119a729959cf`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:03:26 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 10 Nov 2021 13:04:27 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 13:04:28 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 10 Nov 2021 13:06:02 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.7-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '8ceb03d2f7b73c6ce0758290bc42ba366a45c46e033eda36f1779d957a905735'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.7-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 13:06:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 10 Nov 2021 13:06:06 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 10 Nov 2021 13:07:42 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 13:07:43 GMT
CMD ["pypy3"]
# Wed, 10 Nov 2021 21:38:14 GMT
ENV HY_VERSION=1.0a3
# Wed, 10 Nov 2021 21:39:47 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 10 Nov 2021 21:39:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c449cbead98a7c91d47e5f7b5cd106427ea3ef6fafe2b405733eca89645cbb`  
		Last Modified: Wed, 10 Nov 2021 13:17:18 GMT  
		Size: 356.8 KB (356782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a01c89b85b9c6c4f92644ce8e39c8d6f3fb64d20736f5e3f9cba4ef48885275`  
		Last Modified: Wed, 10 Nov 2021 13:17:20 GMT  
		Size: 15.5 MB (15499347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14d32dd311ec5dfc6cb282e63560bc1e76f1b3c35ddb964e583ba05382888ae`  
		Last Modified: Wed, 10 Nov 2021 13:17:17 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d0f73ae9cb8ea54c89307790df2e9ed7983f413020af2ad02bff2cd05781d6`  
		Last Modified: Wed, 10 Nov 2021 13:17:23 GMT  
		Size: 27.0 MB (26998251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2de784ba7ee8c61d85c4e4644cfd5063cd06c1c7f1fab16e8028d3fcd29b85`  
		Last Modified: Wed, 10 Nov 2021 13:17:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8911a5542589b2d14bb77483b45a02150aa57f0dac5f7ddfa60b73944f88c1`  
		Last Modified: Wed, 10 Nov 2021 13:17:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d5f56fd3bf8507084cfbcb6a8a6824d73b5e7f457e2ca68042aa3598237ac`  
		Last Modified: Wed, 10 Nov 2021 13:17:16 GMT  
		Size: 2.9 MB (2943969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109014683a198bba5f2cddd3ee260eea1310048a15b302552cac85c114fa410a`  
		Last Modified: Wed, 10 Nov 2021 13:17:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20658ee8c9d2b8016ac2096f4affeb17a842cbffb7c62910f65c67fcef1094e`  
		Last Modified: Wed, 10 Nov 2021 21:42:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52244f589732d5362f42b72dd531ca7f48ba37d4b92ab7a6ca7fd1ba281430c`  
		Last Modified: Wed, 10 Nov 2021 21:42:05 GMT  
		Size: 4.3 MB (4290884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa91090f052bcc6acbf71ea99210819708d1248f535dbfa4846651aca918efa`  
		Last Modified: Wed, 10 Nov 2021 21:42:01 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
