## `hylang:0-python3.11-alpine3.17`

```console
$ docker pull hylang@sha256:ebcd8d8af194547cb3f6ab79089b20c9b99e37555d18731812d2bb073939c26a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:0-python3.11-alpine3.17` - linux; amd64

```console
$ docker pull hylang@sha256:529cdd16ff9b5a95a33d8df82bda55673af6638c47a89a7ecf2b0163afc77930
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25704549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145b35f21e9fa1845f2d21bbf9d64f75697b70639dbccbf792325885bdd68325`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:56:34 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:56:34 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:56:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:56:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c7bc1de87416dec0f281eccd0b87cdc6eaf1b885647bab3db0d695d6a783f3`  
		Last Modified: Fri, 01 Dec 2023 02:41:47 GMT  
		Size: 622.6 KB (622587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f21e7eee5bdacb0d4a90f07bc27234a8966da6cbd54694873f25d248ecbaa9`  
		Last Modified: Fri, 01 Dec 2023 02:42:20 GMT  
		Size: 12.5 MB (12507105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7273d2245b5c7bbfdfaacde0b0ae49d7a761d866d464107dbd5efd58fc03a313`  
		Last Modified: Fri, 01 Dec 2023 02:42:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d673a1d3d5e296f41a279640695508e06c208e4daa06905afb33b6118562c66`  
		Last Modified: Fri, 01 Dec 2023 02:42:20 GMT  
		Size: 3.1 MB (3109457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3fa625f0bbd990b05f23555e1b9d043eeec939fa4eabbb8fe765afa70706c9`  
		Last Modified: Fri, 01 Dec 2023 20:04:29 GMT  
		Size: 6.1 MB (6085848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; arm variant v6

```console
$ docker pull hylang@sha256:46c21eb9a422bf66baf2e4084f8eb0756bf4ac341007b2d96323e479e1a3e6e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25068036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b78f333a1ab4bf76c17bc1184b378cb035db558df084c412d07ee521bad8bc5`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:90d3bdc6a557ead63796de0110e2fda87e65aa091070cbae612dfb2126568253 in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:15:07 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:15:07 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:15:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:15:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f0440ff44d712e5fc701b84856116589b428157893ac461b633b1ab30b627eed`  
		Last Modified: Thu, 30 Nov 2023 22:49:52 GMT  
		Size: 3.1 MB (3113003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea249d01dc1eeea024b6a10991000458242ecf5ca7d2c418fbcbb6c9349902f2`  
		Last Modified: Fri, 01 Dec 2023 11:12:19 GMT  
		Size: 624.8 KB (624787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b7f169d292bd2b1c3773a8e2072cf0a607a374c3a545f60bc85c3e5f137c60`  
		Last Modified: Fri, 01 Dec 2023 11:12:45 GMT  
		Size: 12.1 MB (12134314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafe56488525d05fca084ced781089d2da1ea1e9e54a5130cdb1b6c25a6232af`  
		Last Modified: Fri, 01 Dec 2023 11:12:44 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2414bbb2c447e4a83abaed1efb5cc95d7c55e36b72bd620a60795a82793e15b0`  
		Last Modified: Fri, 01 Dec 2023 11:12:44 GMT  
		Size: 3.1 MB (3109457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863f763d3eda17d9f31ae9745b76947f7436fd0ee6d9af7b1b09ae24150c2b75`  
		Last Modified: Fri, 01 Dec 2023 20:19:11 GMT  
		Size: 6.1 MB (6086245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; arm variant v7

```console
$ docker pull hylang@sha256:1ccfeacd8a047975b201d46bd915033190ce3f48e3fc5e709a4222e56f028040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24424593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70c5fffcb009bb0941822c7b37dfbe843ceeea56c91dbb9bac531080e24f80c`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:02a6ccbee2a71a547141a8480f3a3912c7bb0934df31124f4a4720204d326698 in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:50:40 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:50:41 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:50:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:50:54 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d4ee79c42f17f258e1c67dc32e0776c934799d208cd0a9b6264f65d60f1a26fc`  
		Last Modified: Thu, 30 Nov 2023 22:50:08 GMT  
		Size: 2.9 MB (2869713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f1360fd2e691e916d990e509541719fb6fccbb47b4a49d758853c2ef805ba`  
		Last Modified: Fri, 01 Dec 2023 02:30:18 GMT  
		Size: 623.8 KB (623783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58eaa8a32cc6b6389131a41f746ff210d83561a3d773f5364954387b348110a9`  
		Last Modified: Fri, 01 Dec 2023 02:30:51 GMT  
		Size: 11.7 MB (11735546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4fb422c3086ff50d1d71cad2cacd99137519ee16aa69aea3b56b490acd105`  
		Last Modified: Fri, 01 Dec 2023 02:30:50 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9634efaa4a566072a800d51e11641acee6a68334b9d50e79269e7bff3650aa`  
		Last Modified: Fri, 01 Dec 2023 02:30:51 GMT  
		Size: 3.1 MB (3109466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e215c73fdd5099f634a0496d4fdfb05f73436eb268eee10f146f123a748dca29`  
		Last Modified: Fri, 01 Dec 2023 19:58:09 GMT  
		Size: 6.1 MB (6085854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:fa5447fea103e93a13e16acd5a20fe54ed888c4a960e247e4ef2cc78a1342f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27606368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce550706249e6c7c89abfea1ddcbfb8fbf1997d0857546b45ceec3ce6431cf4`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:18:03 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:18:04 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:18:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:18:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908ffe9cdedf78821f28c2912c9cb38bad6606802eecf25875c1c2cc261791e1`  
		Last Modified: Wed, 29 Nov 2023 05:41:34 GMT  
		Size: 624.6 KB (624648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a2e8417877eced2b50f38217362a592dec3f97270c792fe3aed9002349c9f`  
		Last Modified: Wed, 29 Nov 2023 05:42:45 GMT  
		Size: 14.5 MB (14527742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18891d39df0b1f627f36d9a75c10dc5bd6f2d2f9fb68ec1370e8c471604d9c5f`  
		Last Modified: Wed, 29 Nov 2023 05:42:44 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c249243161f124754e3aa9b301a39bd47af6721591262b5bcf1b82edb28faad6`  
		Last Modified: Wed, 29 Nov 2023 05:42:45 GMT  
		Size: 3.1 MB (3109469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5635833eb0315125c4171f79a906f13416606082e45d0907fc6f5374d0572976`  
		Last Modified: Fri, 01 Dec 2023 20:25:06 GMT  
		Size: 6.1 MB (6085990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; 386

```console
$ docker pull hylang@sha256:c84bcacc65d3675c63cccef679e4f64e3e103c68453227fffca3319b62e7addd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25959109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db301e30c75c3f4e4b44aa22a38ed5f516dee0867875b1ce801fe002fd747f4`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:4ad1e09b0030ebbf09adcc7c616502a079dc61aff7c6edce2f2ea248cd85b2df in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:08:32 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:08:33 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:08:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:08:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7583c43471b6e056e4cc98119de7f0921ba6ad8cd2645554165c3d9869b344dc`  
		Last Modified: Fri, 01 Dec 2023 02:04:31 GMT  
		Size: 3.4 MB (3414867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530344b953536ade25733b1703e51118274a7f5f02a08769ba8023a87595521c`  
		Last Modified: Fri, 01 Dec 2023 07:08:37 GMT  
		Size: 623.0 KB (622954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993e1ec0c1f0968ea6bbb21da49517e455835b6f9f12dbdfd1e339ff3e7b72e0`  
		Last Modified: Fri, 01 Dec 2023 07:09:11 GMT  
		Size: 12.7 MB (12725461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648456011949770bfac76b294d41d345265457581de3e7d36d98aa62192f64c0`  
		Last Modified: Fri, 01 Dec 2023 07:09:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622a765b3aa8371d8cab0a61c411012cebb15bced4989399d440518fec1b94ea`  
		Last Modified: Fri, 01 Dec 2023 07:09:11 GMT  
		Size: 3.1 MB (3109453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e616e442dda02fd95c7fe011303e6a5850ba4cd72dcdf63ce8ea8dc738e065`  
		Last Modified: Fri, 01 Dec 2023 20:17:45 GMT  
		Size: 6.1 MB (6086145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; ppc64le

```console
$ docker pull hylang@sha256:db1640903aca082a929dc71e8c16cce5b137be826b4a0b6f44d3b6c9e17a0cc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26106048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493a5ecbce39d409a44a9164eb3199d998481ee2f599d3ff69f79ae52eb3ced9`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:e3eb0ea4f652282ad08228d0d146f33998b9e93641756d780ac0205aa828c070 in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:55:09 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:55:09 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:55:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:55:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c7d387f1f267ea360529df8d70b246f949e1afdb2317cdf84b028cda80a093d1`  
		Last Modified: Thu, 30 Nov 2023 23:20:17 GMT  
		Size: 3.4 MB (3391875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a004ba37d88223a300024b1e8b487623463145eac66bd4bdcd32a38c0197c58`  
		Last Modified: Fri, 01 Dec 2023 03:44:49 GMT  
		Size: 625.0 KB (625038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73da667b1b9ee36d01f9b348af570de9cab9fe0fbf8af2e15743dd3644a6836`  
		Last Modified: Fri, 01 Dec 2023 03:45:22 GMT  
		Size: 12.9 MB (12893544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9954ae041ee5f243e6640c6b4cfee9f55dc7d6f9407bb352225b9688fae99a`  
		Last Modified: Fri, 01 Dec 2023 03:45:20 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447fdea9c8867445875f57b15a3b5e0b6e9dba1e4e02f19c0f816747c992c85f`  
		Last Modified: Fri, 01 Dec 2023 03:45:21 GMT  
		Size: 3.1 MB (3109458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10fc2b1c5e06f8e3c648118172b5c5b57100ff05c4ee53242ab37b3e35269ce`  
		Last Modified: Fri, 01 Dec 2023 20:04:49 GMT  
		Size: 6.1 MB (6085903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.11-alpine3.17` - linux; s390x

```console
$ docker pull hylang@sha256:ebc119fcd09e9346f10f30959789f32bb4bcdd04805b9f0e1918f04705c3ee60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25556422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ccbd3d618a85fe67df3dd180ce2667cbc99c21f8522b3d01bcf0b4afc866bb`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 17:01:38 GMT
ADD file:bf416048d22b9a0deecb508385355d79b8d5d12b655c600dbdc0948f7dcbb2c2 in / 
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 17:01:38 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_VERSION=3.11.6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 17:01:38 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 17:01:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 17:01:38 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:12:42 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:12:42 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:12:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:12:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7e9e7e53b618240d2e82e8cab6b677eab6786c4210dcc2b1a35bfd4cb492757e`  
		Last Modified: Thu, 30 Nov 2023 22:43:01 GMT  
		Size: 3.2 MB (3176332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a5260fc11fc98d3d3f073ba28ca56dad71831f7308cdeac837087945276340`  
		Last Modified: Fri, 01 Dec 2023 02:09:41 GMT  
		Size: 622.9 KB (622885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de02a0534e9f203c0bed6c39c218961a4e167082c2e72d682e9cf839374b81e`  
		Last Modified: Fri, 01 Dec 2023 02:10:05 GMT  
		Size: 12.6 MB (12561831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2e6a57fef3ebe85bb33421201a3ee94e16d2f857548c5a3192e2fc4945245`  
		Last Modified: Fri, 01 Dec 2023 02:10:05 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0bd1231d44ce6f5d960b0d60b080e9ffc3a3658fd2d2b582d0997080e6d6f9`  
		Last Modified: Fri, 01 Dec 2023 02:10:05 GMT  
		Size: 3.1 MB (3109436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0076b54b041b86ae88445b1af951835b37f65f4ce79e433f975362ac92583d7`  
		Last Modified: Fri, 01 Dec 2023 20:19:45 GMT  
		Size: 6.1 MB (6085709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
