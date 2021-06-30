## `hylang:python3.8-alpine3.13`

```console
$ docker pull hylang@sha256:0d878017ec4e0cb022128296b9b5f41c61109c407b5b8f4a74a8bdbd0df37e46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:python3.8-alpine3.13` - linux; amd64

```console
$ docker pull hylang@sha256:b431ea8b046c057687d058e42f202ca29f43f1221ff282d7d6ddec3ac7c9f568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19775965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad683d919f37787b13e3aff795650a3d426651d383cd3202bbc3acb0a12d749d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:45:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 04:23:52 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 05:00:34 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 15 Apr 2021 05:00:34 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 04 May 2021 19:01:12 GMT
ENV PYTHON_VERSION=3.8.10
# Tue, 04 May 2021 19:08:32 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 May 2021 19:08:35 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 01:46:42 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 01:46:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 01:46:42 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 01:46:49 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 01:46:49 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 06:00:16 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 06:00:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 06:00:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ad1a75a9998a18ceb4b3e77ebc933525c48a5e9b1dd6abf258e86f537a7fbf`  
		Last Modified: Thu, 15 Apr 2021 08:47:56 GMT  
		Size: 281.3 KB (281266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5472576d6ead46f9c7adf670e276a4af22a014b07f79ceade70b60a9b8d9a03c`  
		Last Modified: Tue, 04 May 2021 19:23:31 GMT  
		Size: 11.2 MB (11233765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107b9b7cb26b3361f6979cb06c8f6c7022a6bf748040ec787fe04d16efaa5995`  
		Last Modified: Tue, 04 May 2021 19:23:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c810b10e5b4d8c963667477f58feb23139465dcfd866acd1e010d8afe8780ed`  
		Last Modified: Tue, 29 Jun 2021 02:12:04 GMT  
		Size: 2.3 MB (2348453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d186d266c3ea94a9c723d3bfef505d6834770ae5f01116f82db2d7e514d98c`  
		Last Modified: Tue, 29 Jun 2021 06:04:01 GMT  
		Size: 3.1 MB (3100282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; arm variant v6

```console
$ docker pull hylang@sha256:9691eb45cf9f02ee7d2a01a6b66fa108cd43e05a0dbe287ef302f835d150fa8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19559023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95158e79b29b8508e8383eb6b5f1c7b9563c0733b47a1f642eb0955b2b384047`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 21:28:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 28 Jun 2021 21:28:23 GMT
ENV LANG=C.UTF-8
# Mon, 28 Jun 2021 22:19:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Mon, 28 Jun 2021 22:19:07 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Jun 2021 20:24:21 GMT
ENV PYTHON_VERSION=3.8.11
# Tue, 29 Jun 2021 20:35:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 29 Jun 2021 20:35:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 20:35:23 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 20:35:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 20:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 20:35:40 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 20:35:40 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 22:19:40 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 22:19:51 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 22:19:51 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b17504c2712f62b78626fbce799ae1591e8c79a273cd3f68bdab3c51361988`  
		Last Modified: Mon, 28 Jun 2021 23:38:35 GMT  
		Size: 281.4 KB (281384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afa69520d16d8f7c96b47424120b67c822987a3a04cbbf6d0abe089a017c7ce`  
		Last Modified: Tue, 29 Jun 2021 21:41:59 GMT  
		Size: 11.2 MB (11206051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff22779cc62d78373285d49054d63d37645bf12d560e726187b1db648b475b2`  
		Last Modified: Tue, 29 Jun 2021 21:41:51 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d03d9a37e7dc0844bcaa589a3b8596ce8828e02a042661403d02d343c754245`  
		Last Modified: Tue, 29 Jun 2021 21:41:54 GMT  
		Size: 2.3 MB (2348629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde8fe1581f7ebac20a091ffd50a4e547c43b7f7f72fd2e7dd6f26b5ffb2edc`  
		Last Modified: Tue, 29 Jun 2021 22:24:58 GMT  
		Size: 3.1 MB (3100600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; arm variant v7

```console
$ docker pull hylang@sha256:f32d51d9054834c45ee2109a29973860e0342ee8ac0b8cbef2236f433646b109
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf49d073e528a6b1bb258b58ec60db7f786555784db8efa92140b500ffc19d9`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 01:40:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 01:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 24 Jun 2021 03:37:04 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 24 Jun 2021 03:37:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Jun 2021 03:37:05 GMT
ENV PYTHON_VERSION=3.8.10
# Thu, 24 Jun 2021 03:47:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Jun 2021 03:47:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 01:24:46 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 01:24:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 01:24:47 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 01:25:02 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 01:25:02 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 10:29:57 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 10:30:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 10:30:08 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c96cfb28e40eb5ef86a77eff7ddd1fc7c31fdb45a563f3636e81b96833ab4c0`  
		Last Modified: Thu, 24 Jun 2021 07:01:49 GMT  
		Size: 280.5 KB (280542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbd8e1c6abeab3bfb30b0ca494489c1a71a66f8f65c730bd2251533dd44291`  
		Last Modified: Thu, 24 Jun 2021 07:01:56 GMT  
		Size: 10.7 MB (10701800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5c75f085471b8925ec44ebe59f8d0fcd4906a3cd58a5a38650d071b48b59fa`  
		Last Modified: Thu, 24 Jun 2021 07:01:49 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588382bd27e7952dbd413dcf78ead82a2846cdfb8433be82de379cd8298eda3`  
		Last Modified: Tue, 29 Jun 2021 02:11:20 GMT  
		Size: 2.3 MB (2348547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137dbce9a577ec6085e7e6463a4e8f01baafc4ab1b9c760d467ba37193824c27`  
		Last Modified: Tue, 29 Jun 2021 10:39:41 GMT  
		Size: 3.1 MB (3100384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:ab623463f527cbf4401acc1bb1bfbfc0eaa557006627049c8c868b19c7aa0552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.1 MB (20139746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe9d43cf91cab59e08118e8aa6d26c71b8ecc2c3fdee5e7ffd8b1c2dc4547eb`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:38:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Jun 2021 09:49:27 GMT
ENV LANG=C.UTF-8
# Wed, 16 Jun 2021 10:15:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Wed, 16 Jun 2021 10:15:52 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Jun 2021 20:08:31 GMT
ENV PYTHON_VERSION=3.8.11
# Tue, 29 Jun 2021 20:14:28 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 29 Jun 2021 20:14:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 20:14:29 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 20:14:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 20:14:30 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 20:14:37 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 20:14:37 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 23:05:08 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 23:05:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 23:05:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db77ac15191d233fe7f71898dbd2c9b8d850259ab0cc3c9b110497026db798`  
		Last Modified: Wed, 16 Jun 2021 11:03:28 GMT  
		Size: 281.5 KB (281492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2fe18fea7cfb7cebce05f326a2dd1c91654695c0d2616f06f4bb834bea941b`  
		Last Modified: Tue, 29 Jun 2021 21:45:37 GMT  
		Size: 11.7 MB (11697454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752a077ae74fdfc2c58439561f4edf7b67b6bf9ef0068510d781fc9a01b9e250`  
		Last Modified: Tue, 29 Jun 2021 21:45:35 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa03497b24346dfbe4ebb1b073cd676b2c975a92bffda64805ea9baa14511b8c`  
		Last Modified: Tue, 29 Jun 2021 21:45:36 GMT  
		Size: 2.3 MB (2348460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c979c505138fa20cf29743befcb389b6e7d9739f46c5ad63ea04541744bb16`  
		Last Modified: Tue, 29 Jun 2021 23:10:28 GMT  
		Size: 3.1 MB (3100083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; 386

```console
$ docker pull hylang@sha256:ca426867d16dd2eb39212e7735f8f89abb3ff82999d195f29e6199a5b7f60cdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19964315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240bce14ff0eabde7c4eed411f6e93c202e8377dd57c07867568703afc88b38e`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:17:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 19:17:48 GMT
ENV LANG=C.UTF-8
# Wed, 14 Apr 2021 19:49:30 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Wed, 14 Apr 2021 19:49:30 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 04 May 2021 19:45:26 GMT
ENV PYTHON_VERSION=3.8.10
# Tue, 04 May 2021 19:52:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 May 2021 19:52:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 02:45:56 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 02:45:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 02:45:57 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 02:46:05 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 02:46:05 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 07:10:28 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 07:10:33 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 07:10:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e260bc1179379ba879b804dfb2c61deb922bd0606ef56eebe66c93e873a8b003`  
		Last Modified: Wed, 14 Apr 2021 23:36:30 GMT  
		Size: 281.8 KB (281818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a03d87cceea9a9a7516accf6e9c6cc8c016a2cd68b46f406349360d6fc225e`  
		Last Modified: Tue, 04 May 2021 20:07:40 GMT  
		Size: 11.4 MB (11414603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053a67e561a33f56105758443110fa5ec12712501ef1154dfdc8a39bcabe9c28`  
		Last Modified: Tue, 04 May 2021 20:07:37 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc37b6daa8b25ae6c97b1df7b763d5eb51069152a621aa13a6ae0b35e2f2a14a`  
		Last Modified: Tue, 29 Jun 2021 03:14:53 GMT  
		Size: 2.3 MB (2348582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b52bbd22f6601b8ea6ed7397c0f4033831690d7fb5be2b8a1db19a041a1f2`  
		Last Modified: Tue, 29 Jun 2021 07:16:06 GMT  
		Size: 3.1 MB (3100180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; ppc64le

```console
$ docker pull hylang@sha256:07f5d09132ef8f8dc53aa6ae2d59a6acd651ce682097ff0b30188f00292d6c16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.5 MB (20467553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef861eeb84e88cf55b475ed30aa025a5da85875bff72fc7d48c2561038a1f291`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 05:07:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 27 Jun 2021 05:07:43 GMT
ENV LANG=C.UTF-8
# Sun, 27 Jun 2021 06:48:16 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sun, 27 Jun 2021 06:48:21 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sun, 27 Jun 2021 06:48:25 GMT
ENV PYTHON_VERSION=3.8.10
# Sun, 27 Jun 2021 06:56:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sun, 27 Jun 2021 06:56:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sun, 27 Jun 2021 06:56:55 GMT
ENV PYTHON_PIP_VERSION=21.1.2
# Sun, 27 Jun 2021 06:56:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/936e08ce004d0b2fae8952c50f7ccce1bc578ce5/public/get-pip.py
# Sun, 27 Jun 2021 06:57:03 GMT
ENV PYTHON_GET_PIP_SHA256=8890955d56a8262348470a76dc432825f61a84a54e2985a86cd520f656a6e220
# Sun, 27 Jun 2021 06:57:23 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sun, 27 Jun 2021 06:57:31 GMT
CMD ["python3"]
# Sun, 27 Jun 2021 21:14:01 GMT
ENV HY_VERSION=1.0a1
# Sun, 27 Jun 2021 21:14:41 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sun, 27 Jun 2021 21:14:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e627f67523943275607c87a6ac1632e6be292fb61ac0bb23c64b5ee191de9f`  
		Last Modified: Sun, 27 Jun 2021 09:04:55 GMT  
		Size: 283.4 KB (283411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4691bfc08a02582c20a6edeeaa233af1c3dea38dddca6a734095fb168367df5c`  
		Last Modified: Sun, 27 Jun 2021 09:04:58 GMT  
		Size: 11.9 MB (11920950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d9344ba2d2d8a6f39be1547782b950830c86a6ea6eb0694688c0aa84235a6`  
		Last Modified: Sun, 27 Jun 2021 09:04:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14117807461388e80844dcba58da8370d87e9e2e431b02dac614cf53367ec6bc`  
		Last Modified: Sun, 27 Jun 2021 09:04:56 GMT  
		Size: 2.3 MB (2348498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa515a25efe8384bca561310ce8172ef3864edf7ad7397ac25e45488d4bf4d`  
		Last Modified: Sun, 27 Jun 2021 21:29:43 GMT  
		Size: 3.1 MB (3101322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.13` - linux; s390x

```console
$ docker pull hylang@sha256:1b6146ea27472db95a03a843094f39f25da0645a2402d803a4e050667ceea883
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19944633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70083813e256f83ba0fa986b9aedf3329f590d40e9347575ff0c778aab2bd418`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 21:55:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 26 Jun 2021 21:55:22 GMT
ENV LANG=C.UTF-8
# Sun, 27 Jun 2021 04:34:32 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sun, 27 Jun 2021 04:34:32 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sun, 27 Jun 2021 04:34:33 GMT
ENV PYTHON_VERSION=3.8.10
# Sun, 27 Jun 2021 04:40:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sun, 27 Jun 2021 04:40:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 29 Jun 2021 06:34:58 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 06:34:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 06:34:59 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 06:35:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Jun 2021 06:35:10 GMT
CMD ["python3"]
# Tue, 29 Jun 2021 11:53:10 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 11:53:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 29 Jun 2021 11:53:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3458e7c8450afd4ac23016a210cff9430775463b81b2c791ca25a7e1fef4b0a`  
		Last Modified: Sun, 27 Jun 2021 11:33:44 GMT  
		Size: 281.7 KB (281714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df39682fa6c9282e8e73e918d8e4476e099947c62ecdc67921e2fe08d826541`  
		Last Modified: Sun, 27 Jun 2021 11:33:50 GMT  
		Size: 11.6 MB (11611528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6bbd28aa3f6bfd6f857e9a1744d7867fdf415582f7873b272c02c0837cee40`  
		Last Modified: Sun, 27 Jun 2021 11:33:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41cea811a9f8629de6069d0c84cd958340135f485519dd83e6d0662729f0374`  
		Last Modified: Tue, 29 Jun 2021 06:51:42 GMT  
		Size: 2.3 MB (2348452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7dfa6dd78ee0efb57e4245aa32378910f91f73930692e88548beb2b52e5cc`  
		Last Modified: Tue, 29 Jun 2021 11:58:46 GMT  
		Size: 3.1 MB (3100059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
