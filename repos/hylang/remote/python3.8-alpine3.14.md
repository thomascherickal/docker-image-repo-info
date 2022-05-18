## `hylang:python3.8-alpine3.14`

```console
$ docker pull hylang@sha256:b603eb7e45f276c28b85e47c0d1c2f2e79a247ede79e61d147cf2e386387f1d6
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

### `hylang:python3.8-alpine3.14` - linux; amd64

```console
$ docker pull hylang@sha256:11ac5d524f5cffd81d9f9ec14c1a88f68e4519771c5e576a53409221bb682298
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21126353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5add4666cd8d5f27a2777bbc7d83063b4a3cb9200a425f1643a5a8383ecdee3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:01:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 08:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 08:10:26 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 09:04:02 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 09:15:56 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 02:36:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 02:36:37 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 02:36:37 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 02:36:37 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 02:44:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:44:25 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:44:32 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:44:32 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:31:18 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:31:18 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:31:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:31:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6202aa870befe19a5b6da7484e3ac1b39b0762008cbc7ed14e11815e9ac4668`  
		Last Modified: Tue, 05 Apr 2022 09:38:32 GMT  
		Size: 666.7 KB (666689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3435575490db5206db80166b4720ae1cc7ce73c4bc477c230ebdb95c58d94a35`  
		Last Modified: Wed, 20 Apr 2022 03:42:17 GMT  
		Size: 11.8 MB (11830343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507de137dab2065186c6c44e6ea15fbfeda587cb2fb9e34ea438c9a37a71bba8`  
		Last Modified: Wed, 20 Apr 2022 03:42:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eb23c1648aa75d32b6020f1ada2cb003e911bf834421fa7d8a24d4bc3f6e90`  
		Last Modified: Wed, 18 May 2022 02:52:31 GMT  
		Size: 2.9 MB (2874020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde56ddc1a2d7c95850f3d6804cc4cd0cbf689048ae4075f1fe125028f04f8d`  
		Last Modified: Wed, 18 May 2022 04:35:56 GMT  
		Size: 2.9 MB (2936701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm variant v6

```console
$ docker pull hylang@sha256:b7db8e4cc6a51144c6626fc5cd4ee1413651a9a79d12e35c43cd523024957cd0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.5 MB (20523430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a83c70a272c6175be3756b9b9ea0758c8c988729fb1a2ad4c3d18ab054e1f1`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:03:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 08:03:43 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 08:03:46 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 10:06:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 10:30:45 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 02:05:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 02:05:09 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 02:05:09 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 02:05:10 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 01:38:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 01:38:40 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 01:38:56 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 01:38:57 GMT
CMD ["python3"]
# Wed, 18 May 2022 02:42:36 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 02:42:36 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 02:42:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 02:42:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c092face47a2112c72860166b813286834ab14f8f92854ffc9f489eca2acbe8`  
		Last Modified: Tue, 05 Apr 2022 11:23:43 GMT  
		Size: 672.5 KB (672521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dc5523435cf95a29fd6ccc735b017832554405f518122918dc0b58945acad`  
		Last Modified: Wed, 20 Apr 2022 02:51:21 GMT  
		Size: 11.4 MB (11413608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2e87ba00e60918ff29536f9e5b4f0619898b485bc1e4343e61627687763555`  
		Last Modified: Wed, 20 Apr 2022 02:51:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc076b86034b284e17491fdb4ec83639787d7f7cf33b2ddd860ded0ba331b274`  
		Last Modified: Wed, 18 May 2022 01:45:20 GMT  
		Size: 2.9 MB (2874108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98611f1a20167bffbae079867613a5357d362c926c6f8f820bd7ea8f25bfc7a4`  
		Last Modified: Wed, 18 May 2022 02:47:45 GMT  
		Size: 2.9 MB (2936904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm variant v7

```console
$ docker pull hylang@sha256:4722ad9ffa837edbe47e79d4be5cc6e4e102152a10af762a80905ba31ba9e02a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19836077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edcd4aef198377858dfca85fe90fbbfd1a30efff27c788a8827cf5e9e1158278`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 12:02:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 12:02:01 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 12:02:04 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 14:01:33 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 14:24:02 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 10:33:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 10:33:04 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 10:33:04 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 10:33:04 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 20 Apr 2022 10:33:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 10:33:05 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 10:33:20 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 10:33:21 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 19:26:51 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 19:26:52 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 19:26:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 19:27:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3106007b2bf37305f1ef428030e7ce4df21b1481c0b001c8ff496c2177affc`  
		Last Modified: Tue, 05 Apr 2022 15:18:56 GMT  
		Size: 664.5 KB (664465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd7141012c9a8df90c7c6c8df57d12848d0ac03a6c32ef53d36c638cf826dca`  
		Last Modified: Wed, 20 Apr 2022 12:55:08 GMT  
		Size: 10.9 MB (10933073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f9e61a598997c0ff27ff4098a418322d6fa95b1636b2bd16a55632c1dd880`  
		Last Modified: Wed, 20 Apr 2022 12:55:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ddb9b82e485bfd90f83a6477e3ba32ac7aaf4d621d08d480d528feeaf035a4`  
		Last Modified: Wed, 20 Apr 2022 12:55:04 GMT  
		Size: 2.9 MB (2874109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320f5db1be3dad89bbbc8f716b93099aee081204e324675a5e91767611ba3644`  
		Last Modified: Wed, 20 Apr 2022 19:36:16 GMT  
		Size: 2.9 MB (2936231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a43803912d3b6d6c8c4cb73941744461137fcbe9ea181996f3516948731930f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21087860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:942bc683a8e5bbb1f46a9d4fb0a27854178ecb83ce12867dd29c1e89bc7eb285`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:07:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 05:07:01 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 05:07:03 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 06:07:04 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 06:17:04 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 03:16:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:16:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:16:56 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:16:57 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 04:41:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 04:41:27 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 04:41:34 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 04:41:34 GMT
CMD ["python3"]
# Wed, 18 May 2022 05:45:10 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 05:45:11 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 05:45:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 05:45:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d5c20c24764c1957d965bf2629678511b31309d3e5bd85ee06a19e1df4b9eb`  
		Last Modified: Tue, 05 Apr 2022 06:42:15 GMT  
		Size: 668.3 KB (668287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364167e532ad0cefec6c096374d298fa369b6190d2445c3320598c1322dc88a7`  
		Last Modified: Wed, 20 Apr 2022 04:11:54 GMT  
		Size: 11.9 MB (11891867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0569fd34744932a01d0dda4f072af26a43d3f61bf5d4b5046133a97605f75b1e`  
		Last Modified: Wed, 20 Apr 2022 04:11:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da36455234d07c87830bb6f762b76764a614493480915877260df731dac9c90`  
		Last Modified: Wed, 18 May 2022 04:52:29 GMT  
		Size: 2.9 MB (2873545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876c344733f3ae2429cb9ff78c6021644f4c1b743ea0c7f35cf291a6c39c8ea1`  
		Last Modified: Wed, 18 May 2022 05:51:50 GMT  
		Size: 2.9 MB (2936541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; 386

```console
$ docker pull hylang@sha256:591c56a98104b9f5f670e6571ec39627eb97778e47a26262b9d84d0200f7d7cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21329511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0865043dcbe7ada888cd945ce30850cfdb803ca0651355e468a7f30a0958e2c5`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:59:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:59:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:59:53 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 05:49:09 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 06:00:09 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 03:01:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 03:01:36 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 03:01:37 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 03:01:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:17:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:17:26 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:17:34 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:17:34 GMT
CMD ["python3"]
# Wed, 18 May 2022 03:48:40 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 03:48:40 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 03:48:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 03:48:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215ecdd17ee697ca711b6420aaeee57970412708c0d0c25f8a6c10cf57f07002`  
		Last Modified: Tue, 05 Apr 2022 06:24:35 GMT  
		Size: 674.6 KB (674589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79831f52b67076bdf41fc9df8ed5b88ad3abb85877598e7e2b5fa7c63e6fdfa0`  
		Last Modified: Wed, 20 Apr 2022 05:38:22 GMT  
		Size: 12.0 MB (12023452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d6338c8f8c9f35f51c2c924558086e512fefe1ae98ed6b721847ae5c32d651`  
		Last Modified: Wed, 20 Apr 2022 05:38:20 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0521c070f49febb2e2019a7332076769dab1ea1c7eae6211b8f16f12d05f8f4`  
		Last Modified: Wed, 18 May 2022 03:28:58 GMT  
		Size: 2.9 MB (2873545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f685dfff0e1a364fc857e8c5594791a42889e0691d300ccd9297c9fa82c87d`  
		Last Modified: Wed, 18 May 2022 03:55:38 GMT  
		Size: 2.9 MB (2936481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; ppc64le

```console
$ docker pull hylang@sha256:dc8786d8663c6ca3934c6f8972e9b48ed87d5e78e6d39ddb6010e90d85c45752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21434868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515144a6d08b959a90348c9bba126363b13a2c88c041346a25682a4c75bf2796`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:34:29 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 16:34:31 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:34:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 18:04:36 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 18:24:37 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 07:27:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 07:27:25 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 07:27:33 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 07:27:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 20 Apr 2022 07:27:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 07:27:50 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 07:28:10 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 07:28:13 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 16:04:14 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 16:04:19 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 16:05:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 16:05:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60ada6e38c11c96e48223b00e85ed8734a57312657ff8d2a373f5ec559b3aec`  
		Last Modified: Tue, 05 Apr 2022 19:05:40 GMT  
		Size: 676.4 KB (676427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe6f1e052b8844f9c8c223ddb8ddb1a2914eae18b332254ac083893c1b54088`  
		Last Modified: Wed, 20 Apr 2022 09:11:16 GMT  
		Size: 12.1 MB (12133061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b1e88fb250aff1b4aae69596692b6f30739fba5b13661c765f1a605e14e83`  
		Last Modified: Wed, 20 Apr 2022 09:11:14 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420c8cc1e203b74b0b7745aca78e6da03bd6f692b967b1dd0fb387b18ff5f72`  
		Last Modified: Wed, 20 Apr 2022 09:11:15 GMT  
		Size: 2.9 MB (2874036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887b5b978e29da0bbb313adf9b36439f201aa15ab14998ef5e274e9ac5e48ac2`  
		Last Modified: Wed, 20 Apr 2022 16:15:55 GMT  
		Size: 2.9 MB (2936947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; s390x

```console
$ docker pull hylang@sha256:aaf8ed6853259613390069a1614db55c6b041ac01e38fb8c9f8bd3c27c5b3ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.9 MB (20901616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49068e433a8345fdb63cccf74d406729b9b23e38fe1715737c6b43101f49277`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:41:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:41:16 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:41:18 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 05:27:00 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 05:37:11 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 02:27:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 02:27:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 02:27:45 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 02:27:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:04:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:04:01 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:04:08 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:04:09 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:52:37 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:52:38 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:52:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:52:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d253464dc85c5cf8aa9aac3b36322787444bb45a3610d2ffc14ecfeaf8cff11`  
		Last Modified: Tue, 05 Apr 2022 05:59:14 GMT  
		Size: 672.5 KB (672460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad279a1b75508822c7b82fc2c54a1d34a1f9433731444c66f4ce29c90c2388e`  
		Last Modified: Wed, 20 Apr 2022 05:00:32 GMT  
		Size: 11.8 MB (11814223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee28b7a833bc3423dcca104e6448fac2ce9f2f114046a0cdc3b57ce4e2f3b614`  
		Last Modified: Wed, 20 Apr 2022 05:00:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a70b79caf4a836a3823b6d68fbcd7ea0f5806278ee6da4c75df107b3ca95a98`  
		Last Modified: Wed, 18 May 2022 03:13:35 GMT  
		Size: 2.9 MB (2874010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53938f7ceeca59b508671db5809a1c5d3513236b21c0fe08ebad8f3d44115513`  
		Last Modified: Wed, 18 May 2022 04:57:50 GMT  
		Size: 2.9 MB (2936617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
