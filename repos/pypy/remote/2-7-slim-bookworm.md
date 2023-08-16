## `pypy:2-7-slim-bookworm`

```console
$ docker pull pypy@sha256:267d92d98704fa60196e07505b49f0a3e018e329a5afc0a4725e8fc8f0fd1ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-7-slim-bookworm` - linux; amd64

```console
$ docker pull pypy@sha256:5700498237cfdc97a60e7d06c2412e38fdf93d2d26d3f3177144b566f38733fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.8 MB (65794229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276181815be185b9f853bed580161274a7b3cc661a6c1b81baea69845cdc73ce`
-	Default Command: `["pypy"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 14:02:06 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 14:02:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:02:06 GMT
ENV PYPY_VERSION=7.3.12
# Fri, 28 Jul 2023 14:08:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 28 Jul 2023 14:08:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 28 Jul 2023 14:08:03 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 28 Jul 2023 14:08:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 28 Jul 2023 14:08:11 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd75e07d7aa79c2aa60b0ecf2fb5ad50381780db291be1709b8ca0f0ad294b2`  
		Last Modified: Fri, 28 Jul 2023 14:10:34 GMT  
		Size: 3.5 MB (3485416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c96343350ffe5dc58aee4b301042f0b426a9eccb31cd49296f8bc0f19daf82e`  
		Last Modified: Fri, 28 Jul 2023 14:14:06 GMT  
		Size: 31.0 MB (31026821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdf42fffefb785aac9909b6b92808496d7aca1f4d4afdf0c0cba5d1004f7fb7`  
		Last Modified: Fri, 28 Jul 2023 14:14:01 GMT  
		Size: 2.2 MB (2157460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:489a9a4acd664ae55927f2e95e16fb2df4e4284c968d7e132a1483ec546dd8b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63628495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a324791d2ddec740965176a921471f921bb20615e367fd094dfe3438153b97`
-	Default Command: `["pypy"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:15:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:15:19 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 06:15:19 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 06:15:19 GMT
ENV PYPY_VERSION=7.3.12
# Fri, 28 Jul 2023 06:20:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 28 Jul 2023 06:20:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 28 Jul 2023 06:20:21 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 28 Jul 2023 06:20:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 28 Jul 2023 06:20:29 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95f2ea93c5dbab06e76ad2618a7011dfd95380229a8b1f9a182e5cd064c0765`  
		Last Modified: Fri, 28 Jul 2023 06:22:47 GMT  
		Size: 3.3 MB (3311881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ab0d007790e91206f52ede648d551ce69ccb8f0a5ba4d4a0528e2a77d23f45`  
		Last Modified: Fri, 28 Jul 2023 06:25:59 GMT  
		Size: 29.0 MB (29001841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0879ab0e5f3772fbd0a67b4b3168c12ee4c637adfa99358b48d8f63259c91617`  
		Last Modified: Fri, 28 Jul 2023 06:25:55 GMT  
		Size: 2.2 MB (2157547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-7-slim-bookworm` - linux; 386

```console
$ docker pull pypy@sha256:49457db3481da77c347fe9461c929fbc9ee94d99f113ddcc97b70ee1ddc3d33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62876095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17393e2c8f10be9eb06cb7b420f93d310115e5c77c59a311e54cf725fdb50e9`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:47:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 07:47:15 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 07:47:15 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 07:47:15 GMT
ENV PYPY_VERSION=7.3.12
# Wed, 16 Aug 2023 07:53:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 16 Aug 2023 07:53:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 16 Aug 2023 07:53:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 16 Aug 2023 07:54:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 16 Aug 2023 07:54:03 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2219e3eeb706ebd934e6fe4fcd4428f6931908beb1fc6be6aa12fcb077d46b`  
		Last Modified: Wed, 16 Aug 2023 07:56:34 GMT  
		Size: 3.5 MB (3492671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422247129acac9f536f70b807b76d55ce8b63ff59c3142722bc6c3902db3b5c`  
		Last Modified: Wed, 16 Aug 2023 08:00:22 GMT  
		Size: 27.1 MB (27084231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd19d609e6b45519114983301df04e766cfaffd1fdfbb865fe5d1c4c8e9905c`  
		Last Modified: Wed, 16 Aug 2023 08:00:16 GMT  
		Size: 2.2 MB (2157370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
