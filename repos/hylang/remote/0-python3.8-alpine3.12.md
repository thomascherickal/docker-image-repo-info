## `hylang:0-python3.8-alpine3.12`

```console
$ docker pull hylang@sha256:bab552011170cc320dd9ea3d59fd92748d773c5d64abd2c3eaf11c6f4600eb12
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

### `hylang:0-python3.8-alpine3.12` - linux; amd64

```console
$ docker pull hylang@sha256:89a2b63dfaf6c1fb94f01952daf43ba436114a8beb48abbb7a18d748252bdea6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19375277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f405e8d98a87ddfaa41b27c307631e8b8dc422d13fb5683671d7cd75c9882`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:33:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:03:58 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:56 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 11 Dec 2020 14:39:56 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 14:39:57 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 11 Dec 2020 14:46:02 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 14:46:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Dec 2020 22:33:15 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:33:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:33:15 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:33:21 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:33:22 GMT
CMD ["python3"]
# Tue, 15 Dec 2020 22:46:42 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 22:46:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 22:46:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a294b7a50964d927f56c36d222326194c96b17568893f059084c1fd482dc27`  
		Last Modified: Fri, 11 Dec 2020 15:34:21 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f0602835631a561ecc8f87fe7ed94eaf444da2bcb33b4d525e8f7c2d62cb8e`  
		Last Modified: Fri, 11 Dec 2020 15:34:19 GMT  
		Size: 11.3 MB (11285239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43527bdab7f3dd363c5165b842042ba104a1aa83b1810f0c1e71e3bd453c0ac8`  
		Last Modified: Fri, 11 Dec 2020 15:34:20 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fa9d7a2d9fe0122aca9ae94330db35ba5d1e6d727bda05773301d1fa25f17`  
		Last Modified: Tue, 15 Dec 2020 22:39:01 GMT  
		Size: 2.1 MB (2138050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19361e099a613b4dfefd351e6bfaaec7df0df38a2055e55fa24d63244cb19a6e`  
		Last Modified: Tue, 15 Dec 2020 22:50:23 GMT  
		Size: 2.9 MB (2874003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; arm variant v6

```console
$ docker pull hylang@sha256:20071f93bb5d70e8234a064c6bb3168d1fb475ef97d85f619992ac0988252fa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18812770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5254ca55d1e84cb85f1d2733daff0af001bc5ef32384e57e22849920b3099f5`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:10:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:10:12 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:31:37 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 06:31:38 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Dec 2020 06:31:40 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 17 Dec 2020 06:40:48 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 06:40:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 17 Dec 2020 06:40:52 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Thu, 17 Dec 2020 06:40:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Thu, 17 Dec 2020 06:40:55 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Thu, 17 Dec 2020 06:41:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 17 Dec 2020 06:41:12 GMT
CMD ["python3"]
# Thu, 17 Dec 2020 10:34:38 GMT
ENV HY_VERSION=0.19.0
# Thu, 17 Dec 2020 10:34:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 17 Dec 2020 10:34:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58afa002a7f38e3dc8df0d977ab013b084a3589bdc2ca0065d0cea13c04dfc07`  
		Last Modified: Thu, 17 Dec 2020 07:45:09 GMT  
		Size: 281.0 KB (280984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95a5610672b268aa222bee406fbbf2bd21e0e68f5864bd0001cb20718337180`  
		Last Modified: Thu, 17 Dec 2020 07:45:13 GMT  
		Size: 10.9 MB (10914554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1db14576d256964a7cba529462db1d791db04e150dfac137d281c84e1c9abe`  
		Last Modified: Thu, 17 Dec 2020 07:45:08 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bc9691b3dd867bac07b0a007bb0466066715e0230ae349ef3827229adc18f9`  
		Last Modified: Thu, 17 Dec 2020 07:45:10 GMT  
		Size: 2.1 MB (2138372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c894a796fd18602c6fd975753894cf3b649e983cf4cde658f6132c215a2be`  
		Last Modified: Thu, 17 Dec 2020 10:37:33 GMT  
		Size: 2.9 MB (2874464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; arm variant v7

```console
$ docker pull hylang@sha256:7105974c7f2f941cedb8817008926d9fe76a0deb6504f492688aa2841ce363f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17755199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da85b6e4440bce81a750ca677f1b36c0fca2aca1f0acb0296cf782bbeb87ed6c`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:50:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:50:14 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 07:02:55 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 07:02:56 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Dec 2020 07:02:56 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 17 Dec 2020 07:07:55 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 07:07:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 17 Dec 2020 07:07:59 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Thu, 17 Dec 2020 07:08:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Thu, 17 Dec 2020 07:08:02 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Thu, 17 Dec 2020 07:08:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 17 Dec 2020 07:08:15 GMT
CMD ["python3"]
# Thu, 17 Dec 2020 10:55:14 GMT
ENV HY_VERSION=0.19.0
# Thu, 17 Dec 2020 10:55:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 17 Dec 2020 10:55:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bde4e2c4e405b74851c8a2fdc7a64519a624c11ddbddae83643e5bf29e5b51`  
		Last Modified: Thu, 17 Dec 2020 07:49:17 GMT  
		Size: 280.1 KB (280062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea6a79e2da40b8c1e58de442918d66f63e7e26c332de0bb8199930becde4f4`  
		Last Modified: Thu, 17 Dec 2020 07:49:21 GMT  
		Size: 10.1 MB (10054421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89497a0576dc8a6f8928b65f0e11a0dfab7318f73d0566cf6589be8e4194037`  
		Last Modified: Thu, 17 Dec 2020 07:49:18 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa605f8f3042fa78e3d00d9cc073deb78ba43d587040d58f59fabd678e4e073`  
		Last Modified: Thu, 17 Dec 2020 07:49:18 GMT  
		Size: 2.1 MB (2138380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad265f89fc26ab64c4744bc9135c4b32e56b8f253d5899de5c67739e6643992`  
		Last Modified: Thu, 17 Dec 2020 10:58:41 GMT  
		Size: 2.9 MB (2874548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:0cf8fc6d123db55848a02a0d3bb29ba8f4c6a1749080234023b3b5ece10865e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19374538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb73daffb35cbcadff87e0b97df0504ce52e1620824a389bc59b3ec587c792bf`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:50:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:23:16 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 13:04:58 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 11 Dec 2020 13:05:00 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 13:05:08 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 11 Dec 2020 13:12:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 13:12:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Dec 2020 22:59:10 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:59:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:59:13 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:59:32 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:59:41 GMT
CMD ["python3"]
# Tue, 15 Dec 2020 23:14:09 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:14:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:14:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013782172d7687fb9bab7c7236554bfc548042ac8776a51cc3cde1d7d20292cb`  
		Last Modified: Fri, 11 Dec 2020 14:32:00 GMT  
		Size: 281.2 KB (281216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a0881b983c6767039614f638250cb638600976455f086db8e1c86924180a03`  
		Last Modified: Fri, 11 Dec 2020 14:32:02 GMT  
		Size: 11.4 MB (11373513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eff1f7f3f9daa84fe189f2e0f01a34fdb3a9b61b746910e9d015cc385a479f9`  
		Last Modified: Fri, 11 Dec 2020 14:31:59 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10115fa6f61d60dac47906f80df4dcdcb4633fcb188f45c0df156d66771a245a`  
		Last Modified: Tue, 15 Dec 2020 23:10:49 GMT  
		Size: 2.1 MB (2138430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be878c67b1ab206508c803b21f028323cc51bef3fab8a886c8b110d637b4f59`  
		Last Modified: Tue, 15 Dec 2020 23:19:51 GMT  
		Size: 2.9 MB (2874528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; 386

```console
$ docker pull hylang@sha256:4776838852ea3a90a5d531cfd8b5d4571a8db27dba49dfccc90d8d4090366871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19571315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4dfd05a62172fa892dc6c9e51c04c01370014db1c940632e9b3eb7df54bd59`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:08:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:08:38 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:25:23 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 06:25:24 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Dec 2020 06:25:24 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 17 Dec 2020 06:32:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 17 Dec 2020 06:32:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 17 Dec 2020 06:32:41 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Thu, 17 Dec 2020 06:32:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Thu, 17 Dec 2020 06:32:41 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Thu, 17 Dec 2020 06:32:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 17 Dec 2020 06:32:48 GMT
CMD ["python3"]
# Thu, 17 Dec 2020 10:34:31 GMT
ENV HY_VERSION=0.19.0
# Thu, 17 Dec 2020 10:34:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 17 Dec 2020 10:34:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8de1c3121b25018c9704e77ea52a95c39db48a341e5bcf9c7bf1f7d28fa019d`  
		Last Modified: Thu, 17 Dec 2020 07:16:58 GMT  
		Size: 281.3 KB (281321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a3dcf765877209d87ec004eaef0819b71e8c5a6ba5796330583abff7f8f218`  
		Last Modified: Thu, 17 Dec 2020 07:17:00 GMT  
		Size: 11.5 MB (11483529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767678b84bbf4357d455536dfc59521dc0dcc52f31eae1629c113e269eecd38`  
		Last Modified: Thu, 17 Dec 2020 07:16:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e038f334eb03b34bd43db37de66e191142e5200cadd95f288b2712c5f2241fe4`  
		Last Modified: Thu, 17 Dec 2020 07:16:58 GMT  
		Size: 2.1 MB (2138027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded29959972f1c87c0b1ec327dd560e38d85140b40605a6d9b16a351058463a1`  
		Last Modified: Thu, 17 Dec 2020 10:38:51 GMT  
		Size: 2.9 MB (2874078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; ppc64le

```console
$ docker pull hylang@sha256:dce25942af15dc9c4b74d5ddce78cc64c275082c42faf59d58d98d9618e33104
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.1 MB (20132414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3963c93483c78a655811f580431e26e99512d6d0b4687fa8e05adeeb9df55c1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:58:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 13:58:52 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:50:25 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 11 Dec 2020 14:50:28 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 14:50:29 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 11 Dec 2020 14:58:11 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 14:58:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Dec 2020 22:40:05 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:40:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:40:19 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:41:07 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:41:14 GMT
CMD ["python3"]
# Wed, 16 Dec 2020 01:09:32 GMT
ENV HY_VERSION=0.19.0
# Wed, 16 Dec 2020 01:10:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 16 Dec 2020 01:10:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c98ec18dc78a565d5f0768349c9ceb1bb4a5e97f1de464739390efa777bc1c3`  
		Last Modified: Fri, 11 Dec 2020 16:04:28 GMT  
		Size: 283.2 KB (283206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fc070b7c78ebb64c3ed4975b02f7dcd02f30c51304dc5ef83a9f6528240268`  
		Last Modified: Fri, 11 Dec 2020 16:04:31 GMT  
		Size: 12.0 MB (12032112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62823f8613460cdd3385201be9f8d5e2328a6741574a93a0a356bee453cdf8`  
		Last Modified: Fri, 11 Dec 2020 16:04:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7d96fcae01700afe86602ab1116b7032102be92af2cd8846340bca96af8508`  
		Last Modified: Tue, 15 Dec 2020 23:01:36 GMT  
		Size: 2.1 MB (2138575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79587088355a83010551be7a7146bb0eb7348347fb9e18bfecf5154f973fa41b`  
		Last Modified: Wed, 16 Dec 2020 01:21:04 GMT  
		Size: 2.9 MB (2874865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.12` - linux; s390x

```console
$ docker pull hylang@sha256:b9dce577aaaef167f02c2116b5a525deff4e2631d9f6e23b2d87b28ed02d28cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19127277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acfe40340bc487e73b5ca72b97dad8ed8a80aa040ec4df5b8ee9f639ce6c6d1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:55:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 06:55:09 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 10:18:48 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 11 Dec 2020 10:18:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 10:18:50 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 11 Dec 2020 10:24:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 10:24:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 15 Dec 2020 22:45:23 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Tue, 15 Dec 2020 22:45:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Tue, 15 Dec 2020 22:45:23 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Tue, 15 Dec 2020 22:45:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Dec 2020 22:45:30 GMT
CMD ["python3"]
# Tue, 15 Dec 2020 23:34:55 GMT
ENV HY_VERSION=0.19.0
# Tue, 15 Dec 2020 23:34:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Dec 2020 23:35:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ae61be5a870639fe07a17526ef280cc170edf9e9daa6c916bd57b397183f01`  
		Last Modified: Fri, 11 Dec 2020 10:57:24 GMT  
		Size: 281.3 KB (281338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041bcb60246d47257dbbab4739573be68a34ef96dbe0e286f31f1db9e26ba31`  
		Last Modified: Fri, 11 Dec 2020 10:57:25 GMT  
		Size: 11.3 MB (11267243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15275ffc4982fb78b4c8deddbd7aaba762d37f34a48ec9428b4ababa94bc551d`  
		Last Modified: Fri, 11 Dec 2020 10:57:24 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79857d61a61131009cb9bacb8c7a891ca9877fb252ee4bad3f9a08df08530a2`  
		Last Modified: Tue, 15 Dec 2020 22:50:01 GMT  
		Size: 2.1 MB (2138106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4e7db19d436e9dfd9e986a1ffc448a2bdd15bd5dc96c9037885e0e300c4290`  
		Last Modified: Tue, 15 Dec 2020 23:38:02 GMT  
		Size: 2.9 MB (2874370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
