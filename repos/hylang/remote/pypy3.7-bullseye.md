## `hylang:pypy3.7-bullseye`

```console
$ docker pull hylang@sha256:2cb9aa00af6762c9d83bf13e64a5b5d9cb74e16230630c049209192dfd6fe37a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.7-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:c444ab564fbce974f8cb33fb355ce05e842643f8d4a7c1180fa116a4faaf499e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75377862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608cd43c767d6e401ce87bbcb9dbb07f4e71c2d67a48b581bb501e820f6f8a1d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:09:39 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:09:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:09:39 GMT
ENV PYPY_VERSION=7.3.5
# Fri, 03 Sep 2021 13:10:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux64.tar.bz2'; 			sha256='9000db3e87b54638e55177e68cbeb30a30fe5d17b6be48a9eb43d65b3ebcfc26'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-aarch64.tar.bz2'; 			sha256='85d83093b3ef5b863f641bc4073d057cc98bb821e16aa9361a5ff4898e70e8ee'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux32.tar.bz2'; 			sha256='3dd8b565203d372829e53945c599296fa961895130342ea13791b17c84ed06c4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-s390x.tar.bz2'; 			sha256='dffdf5d73613be2c6809dc1a3cf3ee6ac2f3af015180910247ff24270b532ed5'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 20 Sep 2021 23:24:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 20 Sep 2021 23:24:34 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 20 Sep 2021 23:24:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 20 Sep 2021 23:24:48 GMT
CMD ["pypy3"]
# Mon, 20 Sep 2021 23:48:40 GMT
ENV HY_VERSION=1.0a3
# Mon, 20 Sep 2021 23:48:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 20 Sep 2021 23:48:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d4ef918ac5de33b592e5a155071c462c2fcab9cf6015458ede77fc167bfcc5`  
		Last Modified: Fri, 03 Sep 2021 13:19:09 GMT  
		Size: 1.1 MB (1065963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe976b83b90b06f56b042ff312b45f6fb547fdb3bce47f9bf5a0e1d4fbe28bf`  
		Last Modified: Fri, 03 Sep 2021 13:19:15 GMT  
		Size: 37.5 MB (37507880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d33491c77edb6017fc45db08caf7ecb57b39df4c61a05728d08f7e5274fbecf`  
		Last Modified: Mon, 20 Sep 2021 23:28:26 GMT  
		Size: 2.4 MB (2370159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80ed7f773fe376ba9b18f079f29a37606dd876acf99ac1e3eb6a37ea68b1108`  
		Last Modified: Mon, 20 Sep 2021 23:50:50 GMT  
		Size: 3.1 MB (3065158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:cf2a3fa20c2ac52e3224ccbd63f1f97426da4b6e57602f934fbe86c2ace36072
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71328927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65da30a8def46c1b010f4106fb6b2038c98af099a820e068cc6b8d05515c855d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:33 GMT
ADD file:9600a4686ae105acffa54787a7c81f5252e90023cbcfbe37519150b954110c5c in / 
# Fri, 03 Sep 2021 00:40:34 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:20:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:20:25 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 04:20:25 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 04:20:25 GMT
ENV PYPY_VERSION=7.3.5
# Fri, 03 Sep 2021 04:20:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux64.tar.bz2'; 			sha256='9000db3e87b54638e55177e68cbeb30a30fe5d17b6be48a9eb43d65b3ebcfc26'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-aarch64.tar.bz2'; 			sha256='85d83093b3ef5b863f641bc4073d057cc98bb821e16aa9361a5ff4898e70e8ee'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux32.tar.bz2'; 			sha256='3dd8b565203d372829e53945c599296fa961895130342ea13791b17c84ed06c4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-s390x.tar.bz2'; 			sha256='dffdf5d73613be2c6809dc1a3cf3ee6ac2f3af015180910247ff24270b532ed5'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Fri, 03 Sep 2021 04:20:56 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 11 Sep 2021 01:41:54 GMT
ENV PYTHON_SETUPTOOLS_VERSION=44.1.1
# Sat, 11 Sep 2021 01:41:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 11 Sep 2021 01:41:54 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 11 Sep 2021 01:42:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 		"setuptools == $PYTHON_SETUPTOOLS_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 11 Sep 2021 01:42:09 GMT
CMD ["pypy3"]
# Sat, 11 Sep 2021 02:11:17 GMT
ENV HY_VERSION=1.0a3
# Sat, 11 Sep 2021 02:11:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 11 Sep 2021 02:11:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1901ca797b5ea06f6a4facc81ad772177fdd833ed4329dc86ef126078633b949`  
		Last Modified: Fri, 03 Sep 2021 00:48:51 GMT  
		Size: 30.1 MB (30055483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5580faf0995f8729d3a51c241a55ca75d8a87b0971080c80cbd69eb3a1f4b2f4`  
		Last Modified: Fri, 03 Sep 2021 04:27:53 GMT  
		Size: 1.1 MB (1054096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2332e8ef18ee8e81cf9f4bd022b7c1f910da17ecf926249880d3d24ad260b576`  
		Last Modified: Fri, 03 Sep 2021 04:28:01 GMT  
		Size: 34.7 MB (34697170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95af6336d764c907cdb1a197086455d045c6b0553017ac1bbd754caca31be92d`  
		Last Modified: Sat, 11 Sep 2021 01:48:26 GMT  
		Size: 2.4 MB (2401050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2550e60522ef12f6dfd6d2a0c582d3b219288e3e8bbe85196f32e4c0cabdca`  
		Last Modified: Sat, 11 Sep 2021 02:15:26 GMT  
		Size: 3.1 MB (3121128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:429a20586144ecdd6f1c36930a1718eaf9c0856edde4313031fa3052f93d27bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75725439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fdc58ee9a14ca36402c63b31ae6dfe439773d4a5c3ce248176f81bf6d9bb12`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:52 GMT
ADD file:dcef0e50863a79295fdbbdad2086d337d6935a220550cb8adaedd7929bd7de63 in / 
# Fri, 03 Sep 2021 00:39:52 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 16:19:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 16:19:31 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 16:19:31 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 16:19:31 GMT
ENV PYPY_VERSION=7.3.5
# Fri, 03 Sep 2021 16:20:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux64.tar.bz2'; 			sha256='9000db3e87b54638e55177e68cbeb30a30fe5d17b6be48a9eb43d65b3ebcfc26'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-aarch64.tar.bz2'; 			sha256='85d83093b3ef5b863f641bc4073d057cc98bb821e16aa9361a5ff4898e70e8ee'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-linux32.tar.bz2'; 			sha256='3dd8b565203d372829e53945c599296fa961895130342ea13791b17c84ed06c4'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.5-s390x.tar.bz2'; 			sha256='dffdf5d73613be2c6809dc1a3cf3ee6ac2f3af015180910247ff24270b532ed5'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 20 Sep 2021 23:39:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 20 Sep 2021 23:39:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 20 Sep 2021 23:39:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 20 Sep 2021 23:39:40 GMT
CMD ["pypy3"]
# Tue, 21 Sep 2021 00:08:28 GMT
ENV HY_VERSION=1.0a3
# Tue, 21 Sep 2021 00:08:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 21 Sep 2021 00:08:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e16e03ac165c3106d1f4265c32840999585f4c4f0e56bd13286caeef08c5be9a`  
		Last Modified: Fri, 03 Sep 2021 00:48:04 GMT  
		Size: 32.4 MB (32379875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca19d4309787a26a20521ed8ed329ba985a2be062bccef9b0700b837523185`  
		Last Modified: Fri, 03 Sep 2021 16:32:28 GMT  
		Size: 1.1 MB (1078326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4839150517afaf0642ead01000cb01c96ad5c8876e0dd8ed53a68b72a6a9e78`  
		Last Modified: Fri, 03 Sep 2021 16:32:38 GMT  
		Size: 36.8 MB (36832205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740fd13252423ce8c0df34af33011d675169125a216b5e87fe51103d5ce7ea7d`  
		Last Modified: Mon, 20 Sep 2021 23:45:55 GMT  
		Size: 2.4 MB (2369761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3abec2d9e6412c6222302af3d7265207942f020f7dc301b57e85d08ef42f2`  
		Last Modified: Tue, 21 Sep 2021 00:12:33 GMT  
		Size: 3.1 MB (3065272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
