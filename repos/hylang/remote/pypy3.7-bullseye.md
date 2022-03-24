## `hylang:pypy3.7-bullseye`

```console
$ docker pull hylang@sha256:945c9150440291f9a8d817248a6d611ea7ae8d299762def0856455a421d8dbf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.7-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:4352d78de57dacc419a523fa39dbaacee887fa4f0b930e9126bbb2b582ad1624
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72764411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04429a220b2826122c6f33c96ec42172a969212911e9ea7471eca1d0fbbfe0`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:19:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:19:55 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:19:55 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 08:19:55 GMT
ENV PYPY_VERSION=7.3.8
# Fri, 18 Mar 2022 08:26:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='639c76f128a856747aee23a34276fa101a7a157ea81e76394fbaf80b97dcf2f2'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 18 Mar 2022 08:26:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 18 Mar 2022 08:26:06 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 18 Mar 2022 08:26:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 18 Mar 2022 08:26:16 GMT
CMD ["pypy3"]
# Fri, 18 Mar 2022 22:22:15 GMT
ENV HY_VERSION=1.0a4
# Fri, 18 Mar 2022 22:22:16 GMT
ENV HYRULE_VERSION=0.1
# Fri, 18 Mar 2022 22:22:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 18 Mar 2022 22:22:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c472301ac0bbdd309c9790c3ec8d1ce83321c26c38be2cc43301b5f811c6ce`  
		Last Modified: Fri, 18 Mar 2022 08:31:56 GMT  
		Size: 1.1 MB (1065922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e6f088ffda22f7e74297b29b12a39121fc29a57197fedd8fc19a63dd0bc02`  
		Last Modified: Fri, 18 Mar 2022 08:36:08 GMT  
		Size: 35.4 MB (35401356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc70efbd37b7cd3862224072f5a36df547192f605001cd3485946a1d8a873547`  
		Last Modified: Fri, 18 Mar 2022 08:36:01 GMT  
		Size: 2.4 MB (2371744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230e82a603dc1536b6c36033448f522ddebd77e9cb078a2b91efb026fdb0d653`  
		Last Modified: Fri, 18 Mar 2022 22:26:04 GMT  
		Size: 2.5 MB (2548817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:5b948d50996d45f0eb644dfa04d1f3f4bbf8f658b3d5d772de1921529203cb5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68357122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03b3eb537a899a029fa83d22dbd37715221a393f96c56ee28fd401d374de65`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:06:11 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:06:12 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 00:06:13 GMT
ENV PYPY_VERSION=7.3.8
# Fri, 18 Mar 2022 00:14:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='639c76f128a856747aee23a34276fa101a7a157ea81e76394fbaf80b97dcf2f2'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 18 Mar 2022 00:14:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 18 Mar 2022 00:14:09 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 18 Mar 2022 00:14:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 18 Mar 2022 00:14:22 GMT
CMD ["pypy3"]
# Fri, 18 Mar 2022 06:50:15 GMT
ENV HY_VERSION=1.0a4
# Fri, 18 Mar 2022 06:50:16 GMT
ENV HYRULE_VERSION=0.1
# Fri, 18 Mar 2022 06:50:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 18 Mar 2022 06:50:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b29e28f3b6592a1077fba71808cf5f544fd04feb4cd65db2beb492a2af87596`  
		Last Modified: Fri, 18 Mar 2022 00:23:06 GMT  
		Size: 849.9 KB (849880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27360ce8ab9c923ca4a808276f6055c738618ecf9eb89d5e17c3570b6723284`  
		Last Modified: Fri, 18 Mar 2022 00:27:52 GMT  
		Size: 32.7 MB (32738791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072c4bdb088d97486013fe25191fc3b62429e83733b0b2969d024dd46c21dba5`  
		Last Modified: Fri, 18 Mar 2022 00:27:46 GMT  
		Size: 2.2 MB (2156134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90111ec4e0cda4906ca6e802b5f34847a226512f5fb9b1b2231a7b574e55b4a`  
		Last Modified: Fri, 18 Mar 2022 06:55:51 GMT  
		Size: 2.5 MB (2549304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:54cc611010d67e8f5655eece762a4f59b7e8739fecad59bb889b2a663aa5705a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73106335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e1cb34611fd81752628f7b0f8aac2bc36f087af55728b69d82e454254761fc`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 13:57:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 13:57:28 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 13:57:28 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 13:57:28 GMT
ENV PYPY_VERSION=7.3.8
# Fri, 18 Mar 2022 14:04:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux64.tar.bz2'; 			sha256='409085db79a6d90bfcf4f576dca1538498e65937acfbe03bd4909bdc262ff378'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='639c76f128a856747aee23a34276fa101a7a157ea81e76394fbaf80b97dcf2f2'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-linux32.tar.bz2'; 			sha256='38429ec6ea1aca391821ee4fbda7358ae86de4600146643f2af2fe2c085af839'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.8-s390x.tar.bz2'; 			sha256='5c2cd3f7cf04cb96f6bcc6b02e271f5d7275867763978e66651b8d1605ef3141'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 18 Mar 2022 14:04:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 18 Mar 2022 14:04:10 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 18 Mar 2022 14:04:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 18 Mar 2022 14:04:26 GMT
CMD ["pypy3"]
# Thu, 24 Mar 2022 14:45:49 GMT
ENV HY_VERSION=1.0a4
# Thu, 24 Mar 2022 14:45:50 GMT
ENV HYRULE_VERSION=0.1
# Thu, 24 Mar 2022 14:45:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 24 Mar 2022 14:45:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e0fad5a47a84890257050246996562d31ae0022f07c8231909a61c353b26cf`  
		Last Modified: Fri, 18 Mar 2022 14:12:34 GMT  
		Size: 1.1 MB (1078418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2259db5d1d00df3fc392a45fe6993ff519d65d53c27aa67f1427e0bf36975b82`  
		Last Modified: Fri, 18 Mar 2022 14:16:07 GMT  
		Size: 34.7 MB (34720110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db58dae457a7ecdf93637f1d4f6c65a9bcca81881e6574295cc4efb0466c3291`  
		Last Modified: Fri, 18 Mar 2022 14:15:57 GMT  
		Size: 2.4 MB (2371556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ceb8b6aae59967a276c39e81b68533b0b86ee35ec0d37506e9efd2d36e06`  
		Last Modified: Thu, 24 Mar 2022 14:54:36 GMT  
		Size: 2.5 MB (2549776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
