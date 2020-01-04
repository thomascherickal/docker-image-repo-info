## `python:3-alpine3.11`

```console
$ docker pull python@sha256:e2039b079c74c794267eb3d27f0216b3e500a52d3eeed4d0dad66fbbc7310bb1
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

### `python:3-alpine3.11` - linux; amd64

```console
$ docker pull python@sha256:f88bd4bbeff13955a7c70cdee5a9c2df083441757530caa9b31d6107d6bbd484
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c4096a65364e07b425f343ba875bb83c70d43eb51fafbe9aaecf345d0ed5ca`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 19:36:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 23:31:32 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 23:31:33 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 23:31:33 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 23:31:33 GMT
ENV PYTHON_VERSION=3.8.1
# Thu, 26 Dec 2019 23:41:37 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 26 Dec 2019 23:41:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 26 Dec 2019 23:41:39 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Thu, 26 Dec 2019 23:41:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 26 Dec 2019 23:41:40 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 26 Dec 2019 23:41:49 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Dec 2019 23:41:49 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0e9bf0cc60b2b34b282bdf7f1000d7e0f1ac24be872c7cbcc098b7a63da2f8`  
		Last Modified: Fri, 27 Dec 2019 03:37:13 GMT  
		Size: 301.3 KB (301279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22eef60a82746975d5b0eb3bf99f81ef241aeef89e6a35a8d3c3d39a5bfcd1a`  
		Last Modified: Fri, 27 Dec 2019 03:37:21 GMT  
		Size: 33.1 MB (33086664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ce47d1841c8b22f369a1bd5dcf0e8dcc23952473fe2dca90f67d180641603`  
		Last Modified: Fri, 27 Dec 2019 03:37:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59795318bcb72141f1cf29891f57f44fc9015eb6f6f9a4ff70def1892699b6`  
		Last Modified: Fri, 27 Dec 2019 03:37:13 GMT  
		Size: 1.9 MB (1870181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; arm variant v6

```console
$ docker pull python@sha256:47b56c7efb26c3d77d8afc84b73f71d0d676bfc8627cb41ebb007de7f959a92f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35127885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3680c6051c506d1cd270ef3a5fd8791e291c3aa44f240c1dc247e76362989e2a`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 23:15:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 23:15:23 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 23:15:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 23:15:26 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 23:15:26 GMT
ENV PYTHON_VERSION=3.8.1
# Fri, 03 Jan 2020 23:37:32 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 03 Jan 2020 23:37:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Jan 2020 23:37:35 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 03 Jan 2020 23:37:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 03 Jan 2020 23:37:36 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 03 Jan 2020 23:37:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Jan 2020 23:37:49 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6c16b3eec9526bd852c13a7869f2bddf5cab8e7762dac1f13fcb5c20f7d32a`  
		Last Modified: Fri, 27 Dec 2019 00:56:38 GMT  
		Size: 301.6 KB (301625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6369966885d7aef7a0c27edd0aa8545b221cf68757bd54d5a3f8556d55f6a623`  
		Last Modified: Sat, 04 Jan 2020 00:57:00 GMT  
		Size: 30.3 MB (30343509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea152af08d0fdb104e2785843fa12070ce1be93a07afa501210ca85d613f668`  
		Last Modified: Sat, 04 Jan 2020 00:56:49 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f46bc4edffa88c67407ef863fbf61bb2fa9a80e12ef053b76b77aea2ceec094`  
		Last Modified: Sat, 04 Jan 2020 00:56:49 GMT  
		Size: 1.9 MB (1870500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; arm variant v7

```console
$ docker pull python@sha256:14e7b7cb6ea8ee8e320489901c4d20134d1ec847517e367d627034b63d966a37
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.7 MB (32735016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4252690d56868c430559eaae2527ced6aefcb94d84f605bfefc7a39956a04e8b`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 22:13:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 22:13:39 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 22:13:43 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 22:13:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 22:13:45 GMT
ENV PYTHON_VERSION=3.8.1
# Thu, 26 Dec 2019 22:19:18 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 26 Dec 2019 22:19:21 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 26 Dec 2019 22:19:22 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Thu, 26 Dec 2019 22:19:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 26 Dec 2019 22:19:23 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 26 Dec 2019 22:19:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Dec 2019 22:19:39 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e33fe6f3eabc840eabfab0d12c478333be31020e983e99be72b2e0346ca87a`  
		Last Modified: Thu, 26 Dec 2019 23:36:44 GMT  
		Size: 300.6 KB (300588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1d964630397dbca5d6230238b1f19e28556252133a07b4d88769d72158b526`  
		Last Modified: Thu, 26 Dec 2019 23:36:55 GMT  
		Size: 28.1 MB (28147041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4a001916b2f327c2a7a3981d4fe852a35b33b9177ae78d904f85f6ddc86468`  
		Last Modified: Thu, 26 Dec 2019 23:36:44 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6346394f0e0cef9858273efb60cc46cbe72b5384b257ebf6b3fd33d5f092523`  
		Last Modified: Thu, 26 Dec 2019 23:36:45 GMT  
		Size: 1.9 MB (1870457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull python@sha256:f84e1ccd08998c5576cceaca5f0a644c513350f9112d5982c4dd96e6fc5a628e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37127418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81db7973e2e3547a792098bbeebe2f572ab7b99b7dd599fb79f618c2e0662e0d`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:49:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 23:05:44 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 23:05:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 23:05:48 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 23:05:49 GMT
ENV PYTHON_VERSION=3.8.1
# Thu, 26 Dec 2019 23:12:52 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 26 Dec 2019 23:12:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 26 Dec 2019 23:12:55 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Thu, 26 Dec 2019 23:12:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 26 Dec 2019 23:12:57 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 26 Dec 2019 23:13:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Dec 2019 23:13:07 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf707181fc01cce5042d8f1f4e804bcb036f9372fcb92040455a0ea66418510`  
		Last Modified: Fri, 27 Dec 2019 00:35:28 GMT  
		Size: 301.8 KB (301750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe68a7e952376fc8f55bfa427bc0a1595fc175a7e792115a64eb51dc1521e70f`  
		Last Modified: Fri, 27 Dec 2019 00:35:39 GMT  
		Size: 32.2 MB (32235860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29989814dcf7a1e224ebb4e72df3c13706abf2d5aa661fe81487d9381892af26`  
		Last Modified: Fri, 27 Dec 2019 00:35:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fd6aa716441a57676e055f04186cbc09474629a93db1321401f59fbe6643b`  
		Last Modified: Fri, 27 Dec 2019 00:35:29 GMT  
		Size: 1.9 MB (1870394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; 386

```console
$ docker pull python@sha256:27de090aa4708880848382a75b771b80d3e5a73cf8271e7e4ff5d3df9513b4a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36212701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9004db0e75e9008364c3603a21c4f9ff5b557cfdef6c99873802ab6f573bfac`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Fri, 27 Dec 2019 00:13:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Dec 2019 00:13:09 GMT
ENV LANG=C.UTF-8
# Fri, 27 Dec 2019 00:13:11 GMT
RUN apk add --no-cache ca-certificates
# Fri, 27 Dec 2019 00:13:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 27 Dec 2019 00:13:11 GMT
ENV PYTHON_VERSION=3.8.1
# Fri, 27 Dec 2019 00:20:33 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 27 Dec 2019 00:20:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 27 Dec 2019 00:20:34 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 27 Dec 2019 00:20:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 27 Dec 2019 00:20:34 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 27 Dec 2019 00:20:40 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 27 Dec 2019 00:20:40 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de240d6a1653e8f4fee6d2e829ab2076b8e8e04e235bad27b7f4c2959c5959a`  
		Last Modified: Fri, 27 Dec 2019 01:25:06 GMT  
		Size: 301.9 KB (301907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bce064f2a4b2832298aaab1843ff967e7d076f3520e4814ff3dd745245be8d`  
		Last Modified: Fri, 27 Dec 2019 01:25:13 GMT  
		Size: 31.2 MB (31235154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7d52e1445a00a25599fd35d535bb54f82c5b2c4a7861636533f2236cb381bf`  
		Last Modified: Fri, 27 Dec 2019 01:25:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892555404b1287e0a33a1b72fb440293db01e2030e362c4222af85ae4150ceb`  
		Last Modified: Fri, 27 Dec 2019 01:25:06 GMT  
		Size: 1.9 MB (1870263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; ppc64le

```console
$ docker pull python@sha256:34dfc441423e5004878bf970624f77716be27e64537fabd19ef622099dd4333e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3957ee9b05abd29cd883b82630d2c2491d3324a35ca76adb6b3296b721ac20`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 23:28:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 23:28:17 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 23:28:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 23:28:28 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 23:28:31 GMT
ENV PYTHON_VERSION=3.8.1
# Thu, 26 Dec 2019 23:36:17 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 26 Dec 2019 23:36:21 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 26 Dec 2019 23:36:22 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Thu, 26 Dec 2019 23:36:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 26 Dec 2019 23:36:27 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 26 Dec 2019 23:36:40 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Dec 2019 23:36:42 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a400f52b82528f8f0ac06d322e07d03bbca37c2866f93dad91af385ca7ec95`  
		Last Modified: Fri, 27 Dec 2019 00:54:25 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b333f6f0e1fcd34086829cbb0cf36ba77c1957f6ee7897e08d20a81dcac1a1cc`  
		Last Modified: Fri, 27 Dec 2019 00:54:41 GMT  
		Size: 34.0 MB (33983859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad91df71432ccf76ed0c93faf17e3fe8efb8b78b72eab4c25cc63baa155092d`  
		Last Modified: Fri, 27 Dec 2019 00:54:25 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2300114ee377e3d31e13909d5a44f7d1ce1e443527eddac8bc351dce0124ba8`  
		Last Modified: Fri, 27 Dec 2019 00:54:27 GMT  
		Size: 1.9 MB (1870410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.11` - linux; s390x

```console
$ docker pull python@sha256:67bc80a0bdac809451d0aab9949e03b569174efe56b26b847f5dc1aa1c0106a6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37696762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42d22bdb2d1f24b3c75c81315aa199818b0939633fb251f0dd733418a549ecc`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 24 Dec 2019 20:16:56 GMT
ADD file:d26fbcd308b78da175af74382b16ee1f7a3370ab9d618b306d604d292e72c560 in / 
# Tue, 24 Dec 2019 20:16:56 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 20:58:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 20:58:42 GMT
ENV LANG=C.UTF-8
# Thu, 26 Dec 2019 20:58:43 GMT
RUN apk add --no-cache ca-certificates
# Thu, 26 Dec 2019 20:58:43 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 26 Dec 2019 20:58:43 GMT
ENV PYTHON_VERSION=3.8.1
# Thu, 26 Dec 2019 21:02:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Thu, 26 Dec 2019 21:02:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 26 Dec 2019 21:02:36 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Thu, 26 Dec 2019 21:02:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Thu, 26 Dec 2019 21:02:36 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Thu, 26 Dec 2019 21:02:41 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Dec 2019 21:02:41 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:bca389ebb9be8103bf737251d68f962104771b2f9c1fff1f7ae0207458fa4c86`  
		Last Modified: Tue, 24 Dec 2019 20:17:18 GMT  
		Size: 2.6 MB (2579591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99351cde69b117e324b26a9046122853e0ba8cfb2f8101e5b6219fdfe3cf16ff`  
		Last Modified: Fri, 27 Dec 2019 00:36:29 GMT  
		Size: 301.8 KB (301803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42da90f36c29c34028b6e44eaa7c947d1d4a3023d3b62ddb693992f011bbf034`  
		Last Modified: Fri, 27 Dec 2019 00:36:35 GMT  
		Size: 32.9 MB (32945099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8ff0f987e483372a205f642f14090142cb72f0c61e76482cdb02dc27ba8ae`  
		Last Modified: Fri, 27 Dec 2019 00:36:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb838689d49c0db8e14550894957d78f1a187f0443602943797182633ae4e2`  
		Last Modified: Fri, 27 Dec 2019 00:36:29 GMT  
		Size: 1.9 MB (1870041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
