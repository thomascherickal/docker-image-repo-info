## `hylang:pypy3.8`

```console
$ docker pull hylang@sha256:8425efd521eeac779d21e485b11977bfe47a0136dbec6db59561bbb9481fb323
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `hylang:pypy3.8` - linux; amd64

```console
$ docker pull hylang@sha256:48d4209f91b5dd6800abbf3af02d2adc276a6279e1bf17a4abdd6ad9208af5e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75654343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a63b92881d9115e7371d3d9d455ff659f07975ca23881e33938b0a6ad466d534`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:14:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:14:03 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 10:14:04 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 10:14:04 GMT
ENV PYPY_VERSION=7.3.11
# Sat, 04 Feb 2023 10:17:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 04 Feb 2023 10:17:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 04 Feb 2023 10:17:40 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 04 Feb 2023 10:17:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 04 Feb 2023 10:17:51 GMT
CMD ["pypy3"]
# Thu, 09 Feb 2023 02:59:10 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:59:10 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:59:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:59:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b11e0b6bc0df3479428b6d6c71c16a9a05e94050fad9a222b4ca4746af187e`  
		Last Modified: Sat, 04 Feb 2023 10:23:14 GMT  
		Size: 1.1 MB (1066527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8479cf02d249ddd8f5739fc4da473d1b4b3d55f3f1adbaae7fdda5e38687d149`  
		Last Modified: Sat, 04 Feb 2023 10:25:21 GMT  
		Size: 35.9 MB (35891399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cefdd1200e1d5369bddf7ba144e81dcf05cab7bb8f77d2e8dd5801af724731`  
		Last Modified: Sat, 04 Feb 2023 10:25:15 GMT  
		Size: 3.2 MB (3170527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c42353b41b20b116396b1ee4f989ccfab104fe4f761d38ef990664c31a3e4`  
		Last Modified: Thu, 09 Feb 2023 03:10:21 GMT  
		Size: 4.1 MB (4128971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:f3fbebca5ca2fb2daad7721c5decd47e7033dc08a7945cccc2d771fab56c6e9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71827237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b1c4db7ffe58253cbaf8d3a95a01abedbe5312ef6761796c1809f2aa8d486a0`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:31:09 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 13:31:09 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 13:31:09 GMT
ENV PYPY_VERSION=7.3.11
# Sat, 04 Feb 2023 13:34:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 04 Feb 2023 13:34:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 04 Feb 2023 13:34:14 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 04 Feb 2023 13:34:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 04 Feb 2023 13:34:25 GMT
CMD ["pypy3"]
# Thu, 09 Feb 2023 03:30:04 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 03:30:04 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 03:30:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 03:30:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94d355ce69d649276dc220c3dfad9c0be5263fbc905a47c71e5cb93b76e493f`  
		Last Modified: Sat, 04 Feb 2023 13:39:27 GMT  
		Size: 1.1 MB (1054066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb09525e82b4d6164b6f4ca044676d926e46aba67ea6a681e519a133ab726fa`  
		Last Modified: Sat, 04 Feb 2023 13:41:27 GMT  
		Size: 33.4 MB (33428983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d3a012cf34d92ddc1a37a4e28d2075586ea5af2dc3ee7067ecb7ae4b2d377b`  
		Last Modified: Sat, 04 Feb 2023 13:41:23 GMT  
		Size: 3.2 MB (3170453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865313d46e417520b6a1e36da25da05a0b6b26144da257f345e2c3ef7d8bf44`  
		Last Modified: Thu, 09 Feb 2023 03:41:24 GMT  
		Size: 4.1 MB (4128943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; 386

```console
$ docker pull hylang@sha256:74593bfdbceeb1a789a9dd26c31b12c083918a15e18aa3fa3fc4eadf4964e289
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74523018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b368245979de4d505d6cc3a2df772096a0a39f6c1363a7f142b90c21ca6948e`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:51:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:51:39 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 21:51:40 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 21:51:41 GMT
ENV PYPY_VERSION=7.3.11
# Sat, 04 Feb 2023 21:56:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 04 Feb 2023 21:56:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 04 Feb 2023 21:56:09 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 04 Feb 2023 21:56:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 04 Feb 2023 21:56:25 GMT
CMD ["pypy3"]
# Thu, 09 Feb 2023 04:51:29 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 04:51:29 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 04:52:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 04:52:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f691486b509c1df658bbbc95b2f405b7e13a551c3578fc7d3f1058a35470b74d`  
		Last Modified: Sat, 04 Feb 2023 22:04:48 GMT  
		Size: 1.1 MB (1078741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932d5357370ea66b0ccc58c857fd60c8364edded03f1a8081a417347ff89dd7`  
		Last Modified: Sat, 04 Feb 2023 22:07:22 GMT  
		Size: 34.0 MB (33987410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e506456a94d3f9b36aafa9f463f14995fc9cbc82d20821895909351dca95f`  
		Last Modified: Sat, 04 Feb 2023 22:07:17 GMT  
		Size: 3.0 MB (2951569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c326f7d078c6ecaa1aae556197f84a29f0fdb3a2e2953f69b5f5d9b6a510e3`  
		Last Modified: Thu, 09 Feb 2023 05:07:25 GMT  
		Size: 4.1 MB (4129526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.20348.1487; amd64

```console
$ docker pull hylang@sha256:a7afa779a1c067ad50b2b4b61c09116fc418e37bda4a01bb53fc6087642d0c41
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1437899250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bc25fa99e917d2acd3362b4abc906dcc271a8fe54a0095a88fd66e9e1b39cc`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 07:31:28 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:31:59 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:32:00 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 12 Jan 2023 07:39:18 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0f46fb6df32941ea016f77cfd7e9b426d5ac25a2af2453414df66103941c8435'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:39:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 12 Jan 2023 07:39:20 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 12 Jan 2023 07:40:29 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:40:30 GMT
CMD ["pypy3"]
# Thu, 09 Feb 2023 01:25:01 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 01:25:02 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 01:27:38 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 09 Feb 2023 01:27:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a931dc7d1f2a06b2a90b68bc4412c2ba2908af1c2cf5bc63e11fa55eb3241f64`  
		Last Modified: Thu, 12 Jan 2023 08:32:02 GMT  
		Size: 612.4 KB (612387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cfe9a2a5f1b4a3cae3eedc722e73f41dbe2b1e6655baaff675a2cf70491fc`  
		Last Modified: Thu, 12 Jan 2023 08:32:05 GMT  
		Size: 15.7 MB (15742123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bb7c6df4ddcc7da657292c237b8d201a1fd19c7a668eb411f5c212890ee966`  
		Last Modified: Thu, 12 Jan 2023 08:32:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb137c4aebaa94731d02f72b62573e0f4711e03a0aa8c174183180ed00e2dd`  
		Last Modified: Thu, 12 Jan 2023 08:33:16 GMT  
		Size: 26.6 MB (26603205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a526f51a7ce4f0b8fb1c4cc485031cab5abf8b55ba4b3ca43f4b53c7d9d63`  
		Last Modified: Thu, 12 Jan 2023 08:33:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e5ee0d5eb254d3b830937c0b0ba53ad0a533c830ddc47b961c0445ee722210`  
		Last Modified: Thu, 12 Jan 2023 08:33:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3bbad9d7e6d5698e3365591ab1762c658d8e92caa140db326b6f84826fac5a`  
		Last Modified: Thu, 12 Jan 2023 08:33:10 GMT  
		Size: 3.8 MB (3758191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d57d060d4bf02481e42bb1fa0067948de90134f6558c736defad459afb6f0fa`  
		Last Modified: Thu, 12 Jan 2023 08:33:07 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abe133230149793b530b977138d9b0d25fea073bb709bb3e626ffe591c7b25b`  
		Last Modified: Thu, 09 Feb 2023 01:32:36 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b44c24c60dce1ad441b10f6e97d08654a0b9b6f29532b2e0e2d376ce847f9`  
		Last Modified: Thu, 09 Feb 2023 01:32:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae71c142d28cfde9b688dfb09e4b7d9977e674e0289faeea9926861af787131`  
		Last Modified: Thu, 09 Feb 2023 01:32:38 GMT  
		Size: 5.1 MB (5143334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd5dd935e94ffa5a56c168c1f4b7e5765334249506a4b5ce967675f23d53cd0`  
		Last Modified: Thu, 09 Feb 2023 01:32:36 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.17763.3887; amd64

```console
$ docker pull hylang@sha256:2b18f47cde31474604452601da85b56e55c4ce7149089417259a0b9500649f3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1758538760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb37b8439f66a3537fb942251c3c1867d684acfaa079b504e6dadaa5c3f99eb`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 07:35:05 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:35:43 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:35:44 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 12 Jan 2023 07:41:42 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0f46fb6df32941ea016f77cfd7e9b426d5ac25a2af2453414df66103941c8435'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:41:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 12 Jan 2023 07:41:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 12 Jan 2023 07:43:11 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 12 Jan 2023 07:43:12 GMT
CMD ["pypy3"]
# Thu, 09 Feb 2023 01:28:02 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 01:28:03 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 01:30:46 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 09 Feb 2023 01:30:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31da2f54a33a71f225ee6d9c2903100380650bfb87243e753ab189b16a3b1a1`  
		Last Modified: Thu, 12 Jan 2023 08:32:36 GMT  
		Size: 364.6 KB (364564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a762462b9c02d170bd93f742eb949d2af6da43c3f64529a7ebef274a2ce0ed7f`  
		Last Modified: Thu, 12 Jan 2023 08:32:38 GMT  
		Size: 15.5 MB (15497383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab2e1ab0fde4783e04474d94c1b21218b3c2526171f7f3f9bf8475b57b6fcbb`  
		Last Modified: Thu, 12 Jan 2023 08:32:34 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005997e6e1100c4e1e1547193b22a2f5982e92e9b46b9478bce7987119bbdca8`  
		Last Modified: Thu, 12 Jan 2023 08:33:37 GMT  
		Size: 26.4 MB (26363128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f14effb9889e7d7a4b3a40a4ea298dbb05b661edbecb83cb33771a32ed1b8a0`  
		Last Modified: Thu, 12 Jan 2023 08:33:29 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78da6785f0ada8cdd9d7de315eac357c8a0109886ad9acc706784f0530b8bf6c`  
		Last Modified: Thu, 12 Jan 2023 08:33:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b53e58a23ae2ce7424f8c0fe75c6e6d96fedf607ed953aa31cb7ed4300bf9e`  
		Last Modified: Thu, 12 Jan 2023 08:33:31 GMT  
		Size: 3.5 MB (3521561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d8302e8598e8e4b33d99ad43d3fb1fa9b60bae8675ee4e7f75b00848b2a78`  
		Last Modified: Thu, 12 Jan 2023 08:33:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae170d618cadbf837e96e933ad00fca7c4be2351fb7a1755063e4511e3ffb8d8`  
		Last Modified: Thu, 09 Feb 2023 01:32:54 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98755875ecae0fd8929db22d3412da9f5e487cd9bb4daaf29994663897bb73c`  
		Last Modified: Thu, 09 Feb 2023 01:32:54 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee8757624f52ea0c4e88f2b965bcad77099e5217b8b91c8fa2539d814ea16f3`  
		Last Modified: Thu, 09 Feb 2023 01:32:56 GMT  
		Size: 4.8 MB (4837519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f7d96f6e9869b9b2e853d321f65d08133c885d0fba9979d0753dd4b9aa7a6`  
		Last Modified: Thu, 09 Feb 2023 01:32:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
