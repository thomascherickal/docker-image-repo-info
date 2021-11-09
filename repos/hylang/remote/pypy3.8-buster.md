## `hylang:pypy3.8-buster`

```console
$ docker pull hylang@sha256:ff3208f95e9cef8cae34896dfaa749ab63feb0e5baa404f293b7e009cdf4cbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.8-buster` - linux; amd64

```console
$ docker pull hylang@sha256:37ecdae2bbeb3ebac50cb018259e4187d83fd8a7b346569612a9485eb12df547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71758519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1dbaa887c95c02eba239599b8397cb379bffc6f026227db7091c3e9a573dda`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:10:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:10:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:10:11 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:06:01 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 27 Oct 2021 00:06:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 27 Oct 2021 00:06:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 27 Oct 2021 00:06:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 27 Oct 2021 00:06:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 00:06:47 GMT
CMD ["pypy3"]
# Thu, 28 Oct 2021 00:25:10 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 00:25:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 00:25:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9691daf778691e301182cf757435ee1bd54288ea1f709d9f89568cb18cb64ad9`  
		Last Modified: Tue, 12 Oct 2021 16:18:00 GMT  
		Size: 2.8 MB (2757989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00deb571522aa6250236df0db674eb48857d41fef9117f26adab3a4647ea3c`  
		Last Modified: Wed, 27 Oct 2021 00:14:44 GMT  
		Size: 36.0 MB (35980106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d9a4d2013b550943ec54685b48ab8d09813f01411dcc486444f051228e82d`  
		Last Modified: Wed, 27 Oct 2021 00:14:38 GMT  
		Size: 2.6 MB (2597286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cfde64e4eb0a89f96a0f67ae92491461eb6c227006aa7a2c08f6b94a34517a`  
		Last Modified: Thu, 28 Oct 2021 00:27:29 GMT  
		Size: 3.3 MB (3283628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:ae73f2df8c9963fe5075ba9f02d73c047241c35a2bd692d8969d8c0e6ad42a24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66893762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8893b3c9bd3b5d21cd13a18d60909fd399730f8f4b3443a490c7314d5614661e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 16:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 16:41:49 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 16:41:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 23:27:13 GMT
ENV PYPY_VERSION=7.3.7
# Tue, 26 Oct 2021 23:27:41 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 26 Oct 2021 23:27:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 26 Oct 2021 23:27:42 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 26 Oct 2021 23:27:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 23:27:58 GMT
CMD ["pypy3"]
# Thu, 28 Oct 2021 00:51:28 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 00:51:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 00:51:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f33f924dedcf5fbbc21c8d0606479984ab4304a4ae0b5f0351fe9ed1980959`  
		Last Modified: Wed, 13 Oct 2021 16:50:22 GMT  
		Size: 2.6 MB (2626756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08901c0f5c40dbd930a645244bc6318befe796c4155988f7932b02d400a942c`  
		Last Modified: Tue, 26 Oct 2021 23:38:27 GMT  
		Size: 32.7 MB (32688561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03fd0224a962831b789cd7c33cb785eb68e9858f50cb6984bde7fd2d0752940`  
		Last Modified: Tue, 26 Oct 2021 23:38:22 GMT  
		Size: 2.4 MB (2385682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa23363301a45150404798546321f3eea2373966745922bdec235d80d8a2040`  
		Last Modified: Thu, 28 Oct 2021 00:55:22 GMT  
		Size: 3.3 MB (3284284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8-buster` - linux; 386

```console
$ docker pull hylang@sha256:d222775a948d36b69f9ebda09dd1e8ade62c062dc2299e3de44cc99e3e31a570
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74476869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f384b5d18cafa8279e1d802dd3b0ccb174794d8e9e516ad5d7c4f185b232f52`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:54:02 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 09:54:03 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 01:51:46 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 27 Oct 2021 01:52:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 27 Oct 2021 01:52:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 27 Oct 2021 01:52:20 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 27 Oct 2021 01:52:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 01:52:36 GMT
CMD ["pypy3"]
# Mon, 08 Nov 2021 22:32:48 GMT
ENV HY_VERSION=1.0a3
# Mon, 08 Nov 2021 22:32:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 08 Nov 2021 22:32:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524c209c075137bc466a890c426fede913f5ca5e85b3773a09154d1c05a5fbc6`  
		Last Modified: Tue, 12 Oct 2021 10:04:42 GMT  
		Size: 2.8 MB (2769479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9f9006067a40985e533ac8520e2a9371a891ca045ed5ad3d271c0300173c6f`  
		Last Modified: Wed, 27 Oct 2021 02:04:34 GMT  
		Size: 38.0 MB (38035195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8dbfea87c7674ebcfa1ac99236c304d21d1ab82773e009aa974085e0a7e424`  
		Last Modified: Wed, 27 Oct 2021 02:04:25 GMT  
		Size: 2.6 MB (2597022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f55928143e12ed331574bc1e0fd6fb12b0af99daeb54b2c3accb130ac2ac9f`  
		Last Modified: Mon, 08 Nov 2021 22:37:10 GMT  
		Size: 3.3 MB (3283728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8-buster` - linux; s390x

```console
$ docker pull hylang@sha256:972a79a4073b8ad3ba5dd4f279e35bf5ea4e981d622d24c347077cabc60bf481
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69091338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c7b66358b863750ff17be7dd0a154f9e9a3fab59b9d7ca6f2fa324f0f2ef11`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:37:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:37:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:16:10 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 27 Oct 2021 00:17:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux64.tar.bz2'; 			sha256='5dee37c7c3cb8b160028fbde3a5901c68043dfa545a16794502b897d4bc40d7e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-aarch64.tar.bz2'; 			sha256='cbd44e0a9146b3c03a9d14b265774a848f387ed846316c3e984847e278d0efd3'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-linux32.tar.bz2'; 			sha256='dfb9d005f0fc917edc60fd618143e4934c412f9168b55166f5519ba0a3b1a835'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.7-s390x.tar.bz2'; 			sha256='ae7d6a76490b317a74b87788d596610c7ffd0ae2d3ffa2433d5bb5300f6b4b77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 27 Oct 2021 00:17:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 27 Oct 2021 00:17:12 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 27 Oct 2021 00:17:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 00:17:29 GMT
CMD ["pypy3"]
# Thu, 28 Oct 2021 00:44:06 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 00:44:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 00:44:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc903ecfe37be2bc114c57a6a772f19f0f9fd9c9c99cd3513fb964b0bb9146ea`  
		Last Modified: Tue, 12 Oct 2021 07:39:05 GMT  
		Size: 2.5 MB (2452801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997d20063dcb48f0fc59795fbf0d9366e241b583b3da1fcd62c341cc66d23fc6`  
		Last Modified: Wed, 27 Oct 2021 00:21:31 GMT  
		Size: 35.0 MB (35003390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f777e117ed8131e08e932169e129c948eae4cf1d50dd44f1719de5799eda829`  
		Last Modified: Wed, 27 Oct 2021 00:21:24 GMT  
		Size: 2.6 MB (2597251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c127459a0965fb3c913a22c1524bd180814edfcf36fe3acca8c3651e17cf71cc`  
		Last Modified: Thu, 28 Oct 2021 00:47:33 GMT  
		Size: 3.3 MB (3283644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
