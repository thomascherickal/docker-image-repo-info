## `hylang:0-pypy-bullseye`

```console
$ docker pull hylang@sha256:2715a4802160423646a39fd45d79801dd385ae507186b27102eff8c14a0e8c41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-pypy-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:0c971a2314fea4f654591babf5b5f11661ccef847deaf55112eacba41bb89214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75551483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c69d172aa90e7df18379b918a4973a6b691b2d86ae976192a4bfd9241e03742`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 11:48:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 11:48:29 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 11:48:29 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:35:02 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 07 Dec 2022 02:38:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux64.tar.bz2'; 			sha256='ceef6496fd4ab1c99e3ec22ce657b8f10f8bb77a32427fadfb5e1dd943806011'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-aarch64.tar.bz2'; 			sha256='e4caa1a545f22cfee87d5b9aa6f8852347f223643ad7d2562e0b2a2f4663ad98'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux32.tar.bz2'; 			sha256='b70ed7fdc73a74ebdc04f07439f7bad1a849aaca95e26b4a74049d0e483f071c'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-s390x.tar.bz2'; 			sha256='c294f8e815158388628fe77ac5b8ad6cd93c8db1359091fa02d41cf6da4d61a1'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 07 Dec 2022 02:38:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 07 Dec 2022 02:38:16 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 07 Dec 2022 02:38:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 07 Dec 2022 02:38:27 GMT
CMD ["pypy3"]
# Wed, 07 Dec 2022 03:06:43 GMT
ENV HY_VERSION=0.25.0
# Wed, 07 Dec 2022 03:06:43 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 07 Dec 2022 03:07:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 07 Dec 2022 03:07:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51466f3f8a8b55ab274f39a90e1dee7c042198a1e3c8c487a2dcb277d863ddf3`  
		Last Modified: Tue, 06 Dec 2022 12:00:36 GMT  
		Size: 1.1 MB (1067963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7913444e0b1faa00e3d6d84d09e2f31e14086c9f121006841e544329d50d82`  
		Last Modified: Wed, 07 Dec 2022 02:45:58 GMT  
		Size: 35.9 MB (35865830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fda9d628d9b95b72518d716a5b3cf274b2889e04bf320197186910c371c715`  
		Last Modified: Wed, 07 Dec 2022 02:45:51 GMT  
		Size: 3.2 MB (3171152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da9e952a0414836636ae9c63d8164fe277081a5b0cf9aa2738bf3e896ff9f4`  
		Last Modified: Wed, 07 Dec 2022 03:11:38 GMT  
		Size: 4.0 MB (4033686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:4be4b91555a29e2b76959ba068b2224a5d04f0aedb5e6b4753197d3da9c2e148
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71716744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162a94993ada6300d9603747f59fdc0ef8b07e379572a4492fe0db1b8aa2cb61`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:41:39 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 06:41:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:13:26 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 07 Dec 2022 02:16:14 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux64.tar.bz2'; 			sha256='ceef6496fd4ab1c99e3ec22ce657b8f10f8bb77a32427fadfb5e1dd943806011'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-aarch64.tar.bz2'; 			sha256='e4caa1a545f22cfee87d5b9aa6f8852347f223643ad7d2562e0b2a2f4663ad98'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux32.tar.bz2'; 			sha256='b70ed7fdc73a74ebdc04f07439f7bad1a849aaca95e26b4a74049d0e483f071c'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-s390x.tar.bz2'; 			sha256='c294f8e815158388628fe77ac5b8ad6cd93c8db1359091fa02d41cf6da4d61a1'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 07 Dec 2022 02:16:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 07 Dec 2022 02:16:15 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 07 Dec 2022 02:16:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 07 Dec 2022 02:16:26 GMT
CMD ["pypy3"]
# Wed, 07 Dec 2022 03:12:22 GMT
ENV HY_VERSION=0.25.0
# Wed, 07 Dec 2022 03:12:22 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 07 Dec 2022 03:12:53 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 07 Dec 2022 03:12:53 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10899d04f0abe7df84b5d209e23478deeda253b78e63b28797c2c513ee13c8b0`  
		Last Modified: Tue, 06 Dec 2022 06:52:42 GMT  
		Size: 1.1 MB (1055302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1aa7227b43e257606db521b4601a28a335d1a07d362b65dbddc1e2f851036b0`  
		Last Modified: Wed, 07 Dec 2022 02:23:31 GMT  
		Size: 33.4 MB (33396416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dc92281c03253f5b61fe944d677f93f1f6458ebfef0b70df2ab815f21d0536`  
		Last Modified: Wed, 07 Dec 2022 02:23:27 GMT  
		Size: 3.2 MB (3171012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b87187ffc63e1d040928de4446e5a8c43b06339488799db2537d8841791f73`  
		Last Modified: Wed, 07 Dec 2022 03:17:46 GMT  
		Size: 4.0 MB (4033694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:156a8b22ef0dbeac264663c57029032459c4b847c52254efd82e6a8848a4aa84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74230905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303b0c8f8d6a2f929809b079064dfea35a1f2f27c37abcdcf9853221a2de506d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 15:33:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 15:33:59 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 15:34:00 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:08:53 GMT
ENV PYPY_VERSION=7.3.10
# Wed, 07 Dec 2022 02:13:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux64.tar.bz2'; 			sha256='ceef6496fd4ab1c99e3ec22ce657b8f10f8bb77a32427fadfb5e1dd943806011'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-aarch64.tar.bz2'; 			sha256='e4caa1a545f22cfee87d5b9aa6f8852347f223643ad7d2562e0b2a2f4663ad98'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-linux32.tar.bz2'; 			sha256='b70ed7fdc73a74ebdc04f07439f7bad1a849aaca95e26b4a74049d0e483f071c'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.10-s390x.tar.bz2'; 			sha256='c294f8e815158388628fe77ac5b8ad6cd93c8db1359091fa02d41cf6da4d61a1'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 07 Dec 2022 02:13:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 07 Dec 2022 02:13:01 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 07 Dec 2022 02:13:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 07 Dec 2022 02:13:17 GMT
CMD ["pypy3"]
# Wed, 07 Dec 2022 03:01:47 GMT
ENV HY_VERSION=0.25.0
# Wed, 07 Dec 2022 03:01:48 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 07 Dec 2022 03:02:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 07 Dec 2022 03:02:31 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d94d6ca55160fc7f8b2b78a357a51fd01e31eb115f1e8a952ae510a2238603a`  
		Last Modified: Tue, 06 Dec 2022 15:52:11 GMT  
		Size: 875.0 KB (874951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c031376af8238a255734f6d01480673f9334f05c3e14041aa6d379792787a8bb`  
		Last Modified: Wed, 07 Dec 2022 02:24:32 GMT  
		Size: 34.0 MB (33978007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbfa84eae6ee60c23788d3673bfe093f7f8d95ee1ebeec13ad591dc109ad9e9`  
		Last Modified: Wed, 07 Dec 2022 02:24:27 GMT  
		Size: 3.0 MB (2951446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c1fa960f7dc7909f6ad9c414b92efe1099680868b4ffe7ef9c969b85d1d22c`  
		Last Modified: Wed, 07 Dec 2022 03:11:07 GMT  
		Size: 4.0 MB (4033455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
