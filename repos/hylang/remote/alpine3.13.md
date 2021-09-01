## `hylang:alpine3.13`

```console
$ docker pull hylang@sha256:5e2379ee3e9f5014398b024babb06332fd15c9ab746c46a1711d93009b37991e
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

### `hylang:alpine3.13` - linux; amd64

```console
$ docker pull hylang@sha256:02c459f8c1efecafe5080296f8222bfcf6d2bf89007343a7b5260616c2b3a898
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.4 MB (22408286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66abd736b1f2871417be9a14e19f3273ed1760b7ea97744b5a7d0976ee0c5b85`
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
# Thu, 15 Apr 2021 04:23:56 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 15 Apr 2021 04:42:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 19:03:06 GMT
ENV PYTHON_VERSION=3.9.7
# Tue, 31 Aug 2021 19:12:38 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 19:12:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 19:12:39 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 19:12:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 19:12:39 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 19:12:46 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 19:12:47 GMT
CMD ["python3"]
# Tue, 31 Aug 2021 22:35:28 GMT
ENV HY_VERSION=1.0a3
# Tue, 31 Aug 2021 22:35:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 31 Aug 2021 22:35:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037ddac5dded861806878db50a3f6b6ba8f8efe5c50f9329bf78028c7cc8bdc`  
		Last Modified: Thu, 15 Apr 2021 08:46:20 GMT  
		Size: 656.2 KB (656228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02fe15417d449cb3121bdfc7ab4db39d3590c59783c90bb047538917a3c2a1e`  
		Last Modified: Tue, 31 Aug 2021 20:12:00 GMT  
		Size: 13.5 MB (13494055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba3e9628f00a730689953b55ceb9cb3c4faac687f0da2476b1f85f42f574159`  
		Last Modified: Tue, 31 Aug 2021 20:11:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda121c1b4df75ffd717716df4ee70222156390fe3ca2d7f10b22d2431ea70e`  
		Last Modified: Tue, 31 Aug 2021 20:11:59 GMT  
		Size: 2.3 MB (2348884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6bad49bb03ac36c59130c71bf1714ca6ee1a46a1cb17a0962dda2ac195c094`  
		Last Modified: Tue, 31 Aug 2021 22:40:43 GMT  
		Size: 3.1 MB (3096920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm variant v6

```console
$ docker pull hylang@sha256:77c7a9e1cd0f7454ac4ed9bce6c85c4a927f59460d8f9a193cdae019c8357aff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19796526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ebcd6d6861e375f2f414bd0a7b468ceb3b79a24ad5e286edfaca29c32c2eb24`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:06:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 23:06:08 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 23:06:14 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 31 Aug 2021 23:21:58 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 23:21:59 GMT
ENV PYTHON_VERSION=3.9.7
# Tue, 31 Aug 2021 23:36:04 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 23:36:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 23:36:09 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 23:36:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 23:36:11 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 23:36:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 23:36:34 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 00:42:37 GMT
ENV HY_VERSION=1.0a3
# Wed, 01 Sep 2021 00:42:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Sep 2021 00:42:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238dba267981e6af977f39d19a985777c9fe772b1d002414d4a16d5a0c7a5fbf`  
		Last Modified: Wed, 01 Sep 2021 00:26:15 GMT  
		Size: 661.8 KB (661761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5887bf53164c13891e6e1eaf5e670784231d7e600e5e3996e275621325dbc2e4`  
		Last Modified: Wed, 01 Sep 2021 00:26:55 GMT  
		Size: 11.1 MB (11064692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36cd660c5b9b9646dd607ae983f3c59c72a268a1c4b8f105455653cf952a51d`  
		Last Modified: Wed, 01 Sep 2021 00:26:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4d7e1904390637028e3faf1e5e7179fca0d9292950901ea745acc3c2a1bbf2`  
		Last Modified: Wed, 01 Sep 2021 00:26:52 GMT  
		Size: 2.3 MB (2348892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86994da7fe2fba4ed17c77a97a8185cbad7632f03f51dc28ca8c1e970fcfc64b`  
		Last Modified: Wed, 01 Sep 2021 00:48:54 GMT  
		Size: 3.1 MB (3097189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm variant v7

```console
$ docker pull hylang@sha256:ea7c6a341f3a9be06f9ee21a80d565ea23a336e83a1806adaf709deeb49998c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19098784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a2de913e2ea27e242e2fc2ec64a22c1d1f1502e43b499e81da93774d2a24407`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Sep 2021 01:26:54 GMT
ADD file:4a3cd5b6e6a9e76edf236ec86eb493ae8b09bf3220a8c0fdcaa474b9d6135ad3 in / 
# Wed, 01 Sep 2021 01:26:55 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:31:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 01:31:19 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 01:31:23 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 01:44:21 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Sep 2021 01:44:22 GMT
ENV PYTHON_VERSION=3.9.7
# Wed, 01 Sep 2021 01:55:09 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 01:55:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 01:55:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 01 Sep 2021 01:55:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 01 Sep 2021 01:55:13 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 01 Sep 2021 01:55:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Sep 2021 01:55:30 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 02:53:34 GMT
ENV HY_VERSION=1.0a3
# Wed, 01 Sep 2021 02:53:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Sep 2021 02:53:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:48fad15491f9799a77d01e4a4a3b0e201ca2aba6f0849c39afa1160d6f3d905a`  
		Last Modified: Wed, 01 Sep 2021 01:28:39 GMT  
		Size: 2.4 MB (2425373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033df4fb521a8f542dd1c3aa7b2cdcf544601a15bb5c54f4c98b0b271abb9235`  
		Last Modified: Wed, 01 Sep 2021 02:47:12 GMT  
		Size: 655.1 KB (655071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4471ed27cdbb8c56b645ee3e2e886c6b4c7666a44c82b5bd541b9c3d1a8c5b9f`  
		Last Modified: Wed, 01 Sep 2021 02:48:27 GMT  
		Size: 10.6 MB (10572006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17f2a90fe471f68237e0daf6d0c637ac2d506203d8ab7a45133bd6e2efb90f`  
		Last Modified: Wed, 01 Sep 2021 02:48:23 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b062d81d020efe78dfa25d3ace1eb00fcfcd438e26a52e78cf77b8f39421e354`  
		Last Modified: Wed, 01 Sep 2021 02:48:24 GMT  
		Size: 2.3 MB (2348908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0f143b576800129e16cf34778422072b789c06ad17cd38c82b9103e1403c7c`  
		Last Modified: Wed, 01 Sep 2021 03:05:42 GMT  
		Size: 3.1 MB (3097194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:36d4034d8cafa9285e6bc6e3915ff873ecaffad98eb023a360448fb243859249
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20736175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878f03a3d7828535b9bc67c4bcf6100af5c24f15f611950edcf8248b54146c04`
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
# Wed, 16 Jun 2021 09:49:28 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 16 Jun 2021 10:02:57 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Jun 2021 19:42:22 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 29 Jun 2021 19:49:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 29 Jun 2021 19:49:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 13 Aug 2021 04:15:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 13 Aug 2021 04:15:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 13 Aug 2021 04:15:34 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 13 Aug 2021 04:15:41 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 13 Aug 2021 04:15:41 GMT
CMD ["python3"]
# Fri, 13 Aug 2021 06:45:49 GMT
ENV HY_VERSION=1.0a3
# Fri, 13 Aug 2021 06:45:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 13 Aug 2021 06:45:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe8a6b629fdcbc043a474ab2528de47d67857394cb4b2d20b835d966e9903e0`  
		Last Modified: Wed, 16 Jun 2021 11:01:39 GMT  
		Size: 658.6 KB (658565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c9ad1cfaa99d2fa1bc654d5277876d42b67a4a174fffeec4a9052e64897bc7`  
		Last Modified: Tue, 29 Jun 2021 21:44:23 GMT  
		Size: 11.9 MB (11920602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b77728fa50ffd19184326e34f8631d7f8db16ef9d102249702c6ab07492ccd`  
		Last Modified: Tue, 29 Jun 2021 21:44:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec39cd8c191b7c7387fc183791c6b2e05fec1c4c826138d9483a685e6606233`  
		Last Modified: Fri, 13 Aug 2021 04:25:55 GMT  
		Size: 2.3 MB (2348776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff548972fbe3476c61b78c0bfed20f4a63f4c338fe7ef912c6a2aed41e230e21`  
		Last Modified: Fri, 13 Aug 2021 06:51:54 GMT  
		Size: 3.1 MB (3095976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; 386

```console
$ docker pull hylang@sha256:096aad9656078ab8346d9db8ced59dec9f522035e55bdbb6a3db0c542a637d0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20624811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe33aae7211259b051ccfa8039b6c80ce9e50697ede4bbec028b7394e0ff885`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 02:08:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 02:08:14 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 02:08:17 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 02:20:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Sep 2021 02:20:40 GMT
ENV PYTHON_VERSION=3.9.7
# Wed, 01 Sep 2021 02:30:56 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 02:30:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 02:30:58 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 01 Sep 2021 02:30:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 01 Sep 2021 02:30:59 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 01 Sep 2021 02:31:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Sep 2021 02:31:08 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 04:26:34 GMT
ENV HY_VERSION=1.0a3
# Wed, 01 Sep 2021 04:26:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Sep 2021 04:26:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf560901ebe47442ad4de0e77444a2c3bf75a5954ddb70738a3fbf4d886539d2`  
		Last Modified: Wed, 01 Sep 2021 03:03:28 GMT  
		Size: 664.0 KB (663976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10026abcbaaf40bcb9db8566633a712ff8d3324707f2ed0c0bd7be67810ceca0`  
		Last Modified: Wed, 01 Sep 2021 03:04:11 GMT  
		Size: 11.7 MB (11693585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619d9f7207f3b8107cf3dba077cd6aa71756fbc0dd7ef4e10e95635d013364d`  
		Last Modified: Wed, 01 Sep 2021 03:04:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990833f19faf27c49cc5b5c72e04b647e1c974e9cb31b7aba1a7d4ebd0a227b`  
		Last Modified: Wed, 01 Sep 2021 03:04:09 GMT  
		Size: 2.3 MB (2348849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa07434bca9cd1aed7bd0da765bdf3c4e4ac70698f10e62e7da54b374cfb0a4`  
		Last Modified: Wed, 01 Sep 2021 04:33:44 GMT  
		Size: 3.1 MB (3097077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; ppc64le

```console
$ docker pull hylang@sha256:fd930441dd2b00f3d2b3a8e63814d02d182bb4c3becc2bab936f089bb83904cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20724488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc49461c6f9c96637107f559f06d2c6ef410bd621d0173633a3bc35730f2e799`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 02:45:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 02:45:58 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 02:46:07 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 02:56:25 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Sep 2021 02:56:30 GMT
ENV PYTHON_VERSION=3.9.7
# Wed, 01 Sep 2021 03:05:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 03:05:24 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 03:05:32 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 01 Sep 2021 03:05:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 01 Sep 2021 03:05:45 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 01 Sep 2021 03:06:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Sep 2021 03:06:16 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 03:49:45 GMT
ENV HY_VERSION=1.0a3
# Wed, 01 Sep 2021 03:50:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 01 Sep 2021 03:50:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730cfc82e3f69a3006664e1e068061a68c4d3ede158be43aaf0e0bb45295df2d`  
		Last Modified: Wed, 01 Sep 2021 03:44:02 GMT  
		Size: 664.8 KB (664786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf1cd7ad33fe9a8fe5c4d2f0c7446dd37caf56747f564301d7160e5ee3a28d`  
		Last Modified: Wed, 01 Sep 2021 03:44:37 GMT  
		Size: 11.8 MB (11798680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d22449b53203c2beae75679341e1b34c98cfe8523ee708a66eea4465e373ed`  
		Last Modified: Wed, 01 Sep 2021 03:44:34 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9d5c116e3c3cb831cbd5a8c0a83a529e94757345f1079c4380d895aaeb62bc`  
		Last Modified: Wed, 01 Sep 2021 03:44:35 GMT  
		Size: 2.3 MB (2348922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084a3d5d4d1b8762a946fd9f4c4ed3d4d71a47bd25f15154500ca27ffad21f12`  
		Last Modified: Wed, 01 Sep 2021 03:58:47 GMT  
		Size: 3.1 MB (3097055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; s390x

```console
$ docker pull hylang@sha256:23a2119b3665c23bf4f6313708e72785aadccf99d4dedee2ed9b2dc57f8e628f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.5 MB (20538653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f575121f7527d688f9030647f6bd718b270f61b6e6fcf791156e0d9f49b99154`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 01:24:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 31 Jul 2021 01:24:05 GMT
ENV LANG=C.UTF-8
# Sat, 31 Jul 2021 01:24:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 31 Jul 2021 01:31:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 31 Jul 2021 01:31:28 GMT
ENV PYTHON_VERSION=3.9.6
# Sat, 31 Jul 2021 01:36:37 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sat, 31 Jul 2021 01:36:38 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 13 Aug 2021 02:12:51 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 13 Aug 2021 02:12:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 13 Aug 2021 02:12:52 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 13 Aug 2021 02:13:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 13 Aug 2021 02:13:02 GMT
CMD ["python3"]
# Fri, 13 Aug 2021 04:59:49 GMT
ENV HY_VERSION=1.0a3
# Fri, 13 Aug 2021 04:59:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 13 Aug 2021 05:00:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906ca2358c7a1d438536fd5c348c434ae7c765f866d341c72b466f97197f8445`  
		Last Modified: Sat, 31 Jul 2021 04:56:34 GMT  
		Size: 661.5 KB (661543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390a75ae2dc7cf667ed5e1b0a83b44117c57a1bfa223d69b07185135f975c54f`  
		Last Modified: Sat, 31 Jul 2021 04:56:56 GMT  
		Size: 11.8 MB (11829443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b832300399bdcb59fa2229999b4c022fb97832d0688023cc27e766dd25bd22b`  
		Last Modified: Sat, 31 Jul 2021 04:56:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f2af7e9fed7a7d6c21a5d326b4591f032ebf3ded6917e2a97479068179edb`  
		Last Modified: Fri, 13 Aug 2021 02:27:25 GMT  
		Size: 2.3 MB (2348868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebce795a720979e05c18196dafbde677369e7d90e361c887f477122687c1267`  
		Last Modified: Fri, 13 Aug 2021 05:04:59 GMT  
		Size: 3.1 MB (3095920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
