## `hylang:python3.8-alpine`

```console
$ docker pull hylang@sha256:2cec752557a50f9d839f2855ac4a3e31fa7bacf758ea81ac96d68953bb9212a7
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

### `hylang:python3.8-alpine` - linux; amd64

```console
$ docker pull hylang@sha256:c0dc1284bd3d0a2d943ecb3da5f4ca43528cb0a6e988f4f3709d0e7c77b4f29b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19807693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f50ded775d4101b50b4c388b48bd613f23902450e7982dfa5176d5908cb59fc1`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:27:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 23:31:48 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:49:40 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:49:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 19:50:48 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 19:58:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 19:58:47 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 19:58:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 01:13:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:31:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:31:24 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:31:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:31:30 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 01:32:18 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 01:32:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 01:32:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11246b421beac7bdab2cd3f620a098af2a8bbbf8e608bef7bf056866e710734`  
		Last Modified: Sat, 28 Aug 2021 00:16:58 GMT  
		Size: 281.5 KB (281499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6f9a3065f19547192c18fa1ed3dd5ec163a387fa47d78aec28e960f5c1097c`  
		Last Modified: Tue, 31 Aug 2021 20:13:17 GMT  
		Size: 11.2 MB (11243987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a167f2660c7a9f713d5ccff5a310c5cf7cf2869c3fa195f2296280f9be43d`  
		Last Modified: Tue, 31 Aug 2021 20:13:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99e6f9c94ec64847476b4efa0e90f74564f7fff38cf7a2885ccf09450e8a87`  
		Last Modified: Wed, 06 Oct 2021 00:39:50 GMT  
		Size: 2.3 MB (2349047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77698b7be8e8c912630a2f12c33308de5d970af5d82dcc6a1dec34d9bc34e2c1`  
		Last Modified: Wed, 06 Oct 2021 01:37:04 GMT  
		Size: 3.1 MB (3118481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm variant v6

```console
$ docker pull hylang@sha256:2e1355a19444987e9496e2f3727f23a386cf00ae119be2b5d50ae2c59a6c6f43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19211877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c45183a8c9380bf6f30f242b1f3623e06ec75d5c4af8bb8d8e17c0c1c53a50`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:42:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 22:42:06 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:08:50 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:08:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 21:40:48 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 21:51:49 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 21:51:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 21:51:52 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 01:30:00 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:50:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:50:50 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:51:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:51:07 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 01:30:26 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 01:30:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 01:30:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8e9151897ef0dc047f9ca095a7c3486bf84800e0cf22dcd437dfebbade82d6`  
		Last Modified: Fri, 27 Aug 2021 23:56:29 GMT  
		Size: 281.7 KB (281669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301f8863fef9cfc0749b56e52d4e5e08f8682c60d16837de44dac77d3c668f48`  
		Last Modified: Tue, 31 Aug 2021 22:08:59 GMT  
		Size: 10.8 MB (10834657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fba06605d613f8a3859559f5f2662c24f7de3b834b66af59157df5dda06ffd2`  
		Last Modified: Tue, 31 Aug 2021 22:08:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9950b0e4399b6644ec0d1775a97e7b55c668b7b6f85b03dfec9d382c51a0a53`  
		Last Modified: Wed, 06 Oct 2021 00:58:02 GMT  
		Size: 2.3 MB (2349115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95ae99abd53f9133eb3471f39d3efd9f472a761ce7a56d937e38e38ce3b3bfc`  
		Last Modified: Wed, 06 Oct 2021 01:36:48 GMT  
		Size: 3.1 MB (3118757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm variant v7

```console
$ docker pull hylang@sha256:a077a3f62ed15ddffb7b5e912f6de091ddf8fd299a2823c5ad5ea018d232edcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18528568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c49dabb51f19f1ae89de8b025bcde8bfabdc62bea86808d76d1c74d1bbeee91a`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:49:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Aug 2021 00:49:03 GMT
ENV LANG=C.UTF-8
# Sat, 28 Aug 2021 01:14:17 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sat, 28 Aug 2021 01:14:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 21:21:03 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 21:31:20 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 21:31:21 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 21:31:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 03:35:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 04:11:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 04:11:03 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 04:11:18 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 04:11:18 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 06:07:38 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 06:07:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 06:07:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d8e0b2f9a23d662efa5dee6f3f21f07fe8fffc2aa562b0514bbb0e47de358e`  
		Last Modified: Sat, 28 Aug 2021 02:05:42 GMT  
		Size: 280.8 KB (280818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501edc19cc45880b4a6d6123688f4693be2eded964f7b50fea7ce16bd9054d92`  
		Last Modified: Tue, 31 Aug 2021 21:58:13 GMT  
		Size: 10.3 MB (10349194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2af96004e7587c4bd25c0be429771657b65250f5f8533d9af6a7bebe23ae2d2`  
		Last Modified: Tue, 31 Aug 2021 21:58:06 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3264149ab53316cc02cfe5e59e5aedc3a5e080e41556d560188298969c1bdc`  
		Last Modified: Wed, 06 Oct 2021 04:31:23 GMT  
		Size: 2.3 MB (2349148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c722410218b77078d82b4a4d171ccf40a5d9039937fec7584de92641d43b89`  
		Last Modified: Wed, 06 Oct 2021 06:19:23 GMT  
		Size: 3.1 MB (3118760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b274a0c382b2a41fa5c69c25c18261a078e8d4cef30373686ae34bca10947eb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19763044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b99e7acdf964b8ca2ce4736b074c1428d17b672a91a050a2594f4137da0fe3`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:18:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Aug 2021 00:00:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Aug 2021 00:14:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sat, 28 Aug 2021 00:14:42 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Sep 2021 00:30:15 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 01 Sep 2021 00:36:02 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 00:36:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 00:36:03 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 01:25:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:41:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:41:21 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:41:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:41:28 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 16:57:10 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 16:57:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 16:57:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82397dd0b53e51c9238ac3da861e9862f3f01e133f3447bc318b86ede25c8bf1`  
		Last Modified: Sat, 28 Aug 2021 00:42:33 GMT  
		Size: 281.7 KB (281687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea96addd4e5a9065de10c8cc698a1cf86dffd94c88a6cefe314b684aa76c021a`  
		Last Modified: Wed, 01 Sep 2021 00:51:12 GMT  
		Size: 11.3 MB (11302413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968775df8ebc9201256291a162db868cafbe9ca1647d5579df7c6b9e5ac36ba2`  
		Last Modified: Wed, 01 Sep 2021 00:51:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0257633cbb9de69ec8cf86d81781c31c16f52e91a8ee30ebb696516e3ca623ed`  
		Last Modified: Wed, 06 Oct 2021 00:53:08 GMT  
		Size: 2.3 MB (2348962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bed8205ebdbc8946c83139bd59735c7745a2f9fdd0e7819f3a64d639e26186`  
		Last Modified: Wed, 13 Oct 2021 17:04:33 GMT  
		Size: 3.1 MB (3117926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; 386

```console
$ docker pull hylang@sha256:7268513b58acea0b4502d762a528b03dff166ad2253d1b2b1e74767f47c2c829
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (20006194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c13d05080a33edce978e283f71c508a0afc2ed61bc8d601b42a25df698e8bb1d`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:56:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 22:56:19 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:22:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:22:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 20:43:27 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 20:51:14 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 20:51:15 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 20:51:15 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 01:58:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 01:03:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 01:03:09 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 01:03:22 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 01:03:23 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 01:40:32 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 01:40:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 01:40:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc387334281d3d644874c7fa4e676cf60daf255166116e3e86f51d42c1fb1c3`  
		Last Modified: Sat, 28 Aug 2021 00:02:33 GMT  
		Size: 282.0 KB (282044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6366d56a862d9afc46f19f490be2aad447ee5bd8a243502a71f6240126dcecaa`  
		Last Modified: Tue, 31 Aug 2021 21:09:12 GMT  
		Size: 11.4 MB (11433452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1927948df88b3052218c6e6063ab72fb1f66e66d1f8bc8af04453ac2ad2a01`  
		Last Modified: Tue, 31 Aug 2021 21:09:09 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a69f5cdeb59255723bc725db20219dffd32dd45bc68ec76cbf6f414467379fa`  
		Last Modified: Wed, 06 Oct 2021 01:17:28 GMT  
		Size: 2.3 MB (2349136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e030710ea0af2d34cff88c11198b89748a78f0354a7b6286f09c786c203710b`  
		Last Modified: Wed, 06 Oct 2021 01:48:00 GMT  
		Size: 3.1 MB (3118471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; ppc64le

```console
$ docker pull hylang@sha256:194db8db7c764c0a6741946777e7c057b4fd838b3dec268201da2a78c12c09fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.1 MB (20103608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec5fffcf520ea3925c9f5fa335b96aedf32ff57af5e0b394b0bfb4ea25b97823`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:50:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Aug 2021 01:50:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 Aug 2021 02:13:13 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sat, 28 Aug 2021 02:13:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 20:57:23 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 21:06:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 21:06:20 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 21:06:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 02:55:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 07 Oct 2021 02:40:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Thu, 07 Oct 2021 02:40:50 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Thu, 07 Oct 2021 02:41:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Oct 2021 02:41:22 GMT
CMD ["python3"]
# Thu, 07 Oct 2021 03:11:54 GMT
ENV HY_VERSION=1.0a3
# Thu, 07 Oct 2021 03:12:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 07 Oct 2021 03:12:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe2654905aa17b30aba2abaf1ea3d9276357d43f46e9765bf8ee47d4fd2432`  
		Last Modified: Sat, 28 Aug 2021 02:51:08 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03111e6e80465281b412893ac14ea6e9a8b32869a86a42619091eb1fb4af7c85`  
		Last Modified: Tue, 31 Aug 2021 21:25:10 GMT  
		Size: 11.5 MB (11539392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13528ec6b56c972fe5234a1ecd40efbf9a45d717a1e28dafabde061f15ab2566`  
		Last Modified: Tue, 31 Aug 2021 21:25:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebdd6ba05d18c0dbd5f62f72fbcc2f2324a019f0fccfffad7dc76403e9c05fe`  
		Last Modified: Thu, 07 Oct 2021 03:00:07 GMT  
		Size: 2.3 MB (2349069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cae7e7dc3e5bd028a160164d0c70314f5292fda4a6ed1e7a4a28cd55bc220`  
		Last Modified: Thu, 07 Oct 2021 03:24:21 GMT  
		Size: 3.1 MB (3118991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; s390x

```console
$ docker pull hylang@sha256:64b89c1d3bf5cf43c86f3ca6987c9900c4f15c4d9aefb5045778afad1154125b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19581094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61dc2c31798517ac38e372515b931fecd691762cdb7c78d80052d0f45b69ec25`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:01:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 21:01:53 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 21:19:34 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 21:19:35 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Sep 2021 00:39:01 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 01 Sep 2021 00:45:14 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 00:45:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 00:45:17 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 01:32:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:24:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:24:13 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:24:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:24:19 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 00:56:39 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 00:56:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 00:56:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad56fe48972d40027df4420737d9917e143ca01da17e3137b85296e421a3bbd8`  
		Last Modified: Sat, 28 Aug 2021 00:39:50 GMT  
		Size: 281.9 KB (281940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d7cb30a9a85008d630160359b40b10ceb6c1f34298c9e43b89b54d78c29e9`  
		Last Modified: Wed, 01 Sep 2021 01:01:20 GMT  
		Size: 11.2 MB (11228068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7e5e50920d35ca26df7332a72550284c65c2e618390d3a7b3e7d3d6e17b7fc`  
		Last Modified: Wed, 01 Sep 2021 01:01:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3d590c9c65683ea581c45210a73a289dde2c0d277f3ea8e2388717403e8dfc`  
		Last Modified: Wed, 06 Oct 2021 00:33:33 GMT  
		Size: 2.3 MB (2348937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9485a440be628c2c2c189a7e6e629357c3f2e564124adef142c5ce146bdd649d`  
		Last Modified: Wed, 06 Oct 2021 01:02:22 GMT  
		Size: 3.1 MB (3118454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
