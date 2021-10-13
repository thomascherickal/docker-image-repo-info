## `hylang:alpine3.13`

```console
$ docker pull hylang@sha256:df001fdf30629fee18f2b1218318bc8253da68488cabcfc1ea3e921e2b348247
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
$ docker pull hylang@sha256:c5cadd87bcbb69858b978a0cd98ce298cd95013761cc553fdc438e47939bb052
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20713254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e82df63b767a9288a70dcae7e596e2643dc4545cc91d86b5a7c1066b5799dce3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:43:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 03:15:52 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 03:15:54 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 03:15:54 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 00:19:21 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 00:27:49 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 00:27:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 00:27:50 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 00:27:50 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:27:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:27:51 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:27:58 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:27:58 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 21:55:56 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 21:56:01 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 21:56:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d1de1f04a6f93fee3a72b9e7af8ef615eaeeafcb72d57303b2ded0d46fbe10`  
		Last Modified: Wed, 01 Sep 2021 03:57:40 GMT  
		Size: 656.2 KB (656243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff691cf107ce75c8db266bb4ea1a2d3329b7b2c0799be850c47c3d171a0e6d10`  
		Last Modified: Wed, 06 Oct 2021 00:37:32 GMT  
		Size: 11.6 MB (11628906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd60cd2951f13475285d0afa0ee038688a2d40b3d1cc39756ec3099a93f2c86`  
		Last Modified: Wed, 06 Oct 2021 00:37:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981025110961ad291cd27abde2bd6d5aa6e01437ac377ef3c984b278fd9b6247`  
		Last Modified: Wed, 06 Oct 2021 00:37:31 GMT  
		Size: 2.3 MB (2349029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf8fe8c4e127c90dacbbee0208ae076dfc3978f6c105cef086efcc9c6231234`  
		Last Modified: Wed, 06 Oct 2021 21:59:22 GMT  
		Size: 3.3 MB (3264767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm variant v6

```console
$ docker pull hylang@sha256:5cc35dea162e749289afc9d94afa819d68339b9ead68bdcaffea0f0cc9673158
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.1 MB (20070299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b832148ba78a40b84f290464c6c1e9056b0130e352697c3f0576f37b0ec34a`
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
# Tue, 31 Aug 2021 23:06:15 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 00:36:34 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 00:49:12 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 00:49:13 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 00:49:14 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 00:49:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:49:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:49:15 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:49:34 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:49:35 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 19:06:32 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 19:06:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 19:06:46 GMT
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
	-	`sha256:380f74f93348d752e4ed26fdf370a2a410910d9f0bdbbf3a0d01feba2e96ca65`  
		Last Modified: Wed, 06 Oct 2021 00:57:06 GMT  
		Size: 11.2 MB (11170273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c8cbd2cda94d0b63eafff5ae9f1d1a99ccbe8251d34fa3f310185d6dec8ba`  
		Last Modified: Wed, 06 Oct 2021 00:56:59 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9038aa84633c2b5b09984726e017aba9831e9380d3d85aecd76e4e534e7904`  
		Last Modified: Wed, 06 Oct 2021 00:57:01 GMT  
		Size: 2.3 MB (2349207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a5496d64c00a7e29be814c1219c12e6ffedffe265a01ab12e225098160dc2b`  
		Last Modified: Wed, 06 Oct 2021 19:11:43 GMT  
		Size: 3.3 MB (3265068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm variant v7

```console
$ docker pull hylang@sha256:4013a7e9f31abdff1de5da31ae55a6f666fcb7ba948b9b814d38d1b32077fabf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19360846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4caad2bdb10eda27c74554ff04c3cf133472e84388465843086972338bc5a5`
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
# Wed, 01 Sep 2021 01:31:23 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 03:53:32 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 04:04:55 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 04:04:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 04:04:57 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 04:04:57 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 04:04:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 04:04:58 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 04:05:15 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 04:05:15 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 21:11:58 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 21:12:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 21:12:10 GMT
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
	-	`sha256:eeccd4e4e855c96b07046974bd6d7b3e5ec8ac51317290502c5125b2f7cd3f26`  
		Last Modified: Wed, 06 Oct 2021 04:28:20 GMT  
		Size: 10.7 MB (10665958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b292f69cc61306be805ddcae230c4cb5e716c14f3c9af404dc2183dc8a3152`  
		Last Modified: Wed, 06 Oct 2021 04:28:13 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cace58069d4b8711acc3b47ab899088c00ddff94732e2bf1f0aeab8c2913cde`  
		Last Modified: Wed, 06 Oct 2021 04:28:15 GMT  
		Size: 2.3 MB (2349217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9004c923f1fc4c3c5bf6708cf4b9f4f59104a3bba4c11d0831ddd850d840e25`  
		Last Modified: Wed, 06 Oct 2021 21:21:46 GMT  
		Size: 3.3 MB (3264995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a4eb1ec4e25400ca58b838df34bef696c0a4d67fda0063cd49dba2ad4389a3da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20669758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6437793cfb5ebac4349c28edd16e1dc5f5c07c09e8f33bfb559358b9a830561d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 09:24:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 09:24:00 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 09:24:01 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 09:24:02 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 00:31:45 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 00:38:29 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 00:38:30 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 00:38:30 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 00:38:30 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:38:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:38:30 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:38:38 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:38:38 GMT
CMD ["python3"]
# Wed, 13 Oct 2021 16:55:53 GMT
ENV HY_VERSION=1.0a3
# Wed, 13 Oct 2021 16:55:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 13 Oct 2021 16:55:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104a7a367d019f51bf46f87898cc6dcbf80d9a86a462d9c7bd236e7d75ec5c51`  
		Last Modified: Wed, 01 Sep 2021 10:04:45 GMT  
		Size: 658.6 KB (658585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9b63ad3fa4982999e1595f254f6b8a36b4f67c109d7ce81ce022096a8192d`  
		Last Modified: Wed, 06 Oct 2021 00:50:31 GMT  
		Size: 11.7 MB (11685313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b425d3d03835e4d46c14f6e25ddfdaad1e892c2923f305de1aa1a2e4425d13dd`  
		Last Modified: Wed, 06 Oct 2021 00:50:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43006c5859f8d8f7718c0869d760371e7a4dddaebc9d59fffd6c66d616c0b9e`  
		Last Modified: Wed, 06 Oct 2021 00:50:31 GMT  
		Size: 2.3 MB (2348984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417c18e29617230b424f8854c7a52255df5c763e0da0652a7658e1560bd2288b`  
		Last Modified: Wed, 13 Oct 2021 17:02:58 GMT  
		Size: 3.3 MB (3263638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; 386

```console
$ docker pull hylang@sha256:b58f28e921e0e7fe6456b6180836b38879b13aa53515caf8544697efa08a388a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.9 MB (20928135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4470b80244c28684778a7fb99aa6f4cf1299513b58446f280459da33c059cad`
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
# Wed, 01 Sep 2021 02:08:17 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 00:50:05 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 00:59:16 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 00:59:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 00:59:17 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 00:59:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:59:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:59:18 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:59:26 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:59:27 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 19:12:49 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 19:12:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 19:12:56 GMT
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
	-	`sha256:58fd25cc2023ab72d43b7b029b9da330f3c31476d54252de750fb86b2c5fed80`  
		Last Modified: Wed, 06 Oct 2021 01:14:53 GMT  
		Size: 11.8 MB (11828928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ab0481aed3019771136580ed8b0eeb908ec1541faed8c6291bb7af5f226c7`  
		Last Modified: Wed, 06 Oct 2021 01:14:50 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2505ea16a53b9b438878b7b49ce137d0455e052d72b05f15a705e7cf7b732af9`  
		Last Modified: Wed, 06 Oct 2021 01:14:51 GMT  
		Size: 2.3 MB (2349096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e11f6ace80ff916ea7f57577edea80a0af3a214b9c5be8580162c010e1c053a`  
		Last Modified: Wed, 06 Oct 2021 19:19:21 GMT  
		Size: 3.3 MB (3264811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; ppc64le

```console
$ docker pull hylang@sha256:480815e9c858dbe9bdfc715bc8e8aaab5d0a36f3464b1489ee1d7e17b6d7f01d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21023453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301ab41843a0504b75915ddb663bf7c436b4a72f5fadfaf3d1b5515cdd3280c9`
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
# Wed, 01 Sep 2021 02:46:09 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 07 Oct 2021 02:19:23 GMT
ENV PYTHON_VERSION=3.10.0
# Thu, 07 Oct 2021 02:29:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 07 Oct 2021 02:29:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 07 Oct 2021 02:29:15 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Thu, 07 Oct 2021 02:29:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 07 Oct 2021 02:29:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Thu, 07 Oct 2021 02:29:25 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Thu, 07 Oct 2021 02:29:44 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 07 Oct 2021 02:29:49 GMT
CMD ["python3"]
# Thu, 07 Oct 2021 03:06:37 GMT
ENV HY_VERSION=1.0a3
# Thu, 07 Oct 2021 03:06:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 07 Oct 2021 03:07:00 GMT
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
	-	`sha256:418e428fde1bfe48f2d590bd07a3885cf3fe03d8aa0905138f8abf986883c998`  
		Last Modified: Thu, 07 Oct 2021 02:57:37 GMT  
		Size: 11.9 MB (11929581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628403f72dbca254b290be883ab70bc8f32d4a776e3ed5be856c0a191ca4f53`  
		Last Modified: Thu, 07 Oct 2021 02:57:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b1c82975647f10d7f21d8bbac4c112aaccc33cd9bc83db5b2b7914d0db05a8`  
		Last Modified: Thu, 07 Oct 2021 02:57:36 GMT  
		Size: 2.3 MB (2349163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b99e883461210c578259aa9dc985f1d0044787d6d6b8b657910a44c74e50d`  
		Last Modified: Thu, 07 Oct 2021 03:22:39 GMT  
		Size: 3.3 MB (3264880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.13` - linux; s390x

```console
$ docker pull hylang@sha256:a3043c787abb553af932772c865b4136c8cd14b7c0ce2d9f9a07e244113a02ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.5 MB (20468284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b72892518fea2990e4fe5b0c64c09f41157c8e85c7432f493efe6d013014850`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 08:06:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 08:06:39 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 08:06:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 01 Sep 2021 08:06:42 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 06 Oct 2021 00:16:36 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 06 Oct 2021 00:21:27 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 06 Oct 2021 00:21:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 06 Oct 2021 00:21:28 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 06 Oct 2021 00:21:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 06 Oct 2021 00:21:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 06 Oct 2021 00:21:28 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 06 Oct 2021 00:21:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 06 Oct 2021 00:21:35 GMT
CMD ["python3"]
# Wed, 06 Oct 2021 19:08:31 GMT
ENV HY_VERSION=1.0a3
# Wed, 06 Oct 2021 19:08:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 06 Oct 2021 19:08:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707fc57521a23ff9f084a3843189199752aec401dcc262466860b002b8ff8676`  
		Last Modified: Wed, 01 Sep 2021 11:50:40 GMT  
		Size: 661.5 KB (661529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344bfebefbeab378622e7b84f4e435f49acd6a06206b9d3684bf0fb3fa4abab0`  
		Last Modified: Wed, 06 Oct 2021 00:32:00 GMT  
		Size: 11.6 MB (11588375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9aa5d6686497f7fbb8db73803cfdd84b6efec2016ae7d56ddd5e55d4078b40`  
		Last Modified: Wed, 06 Oct 2021 00:31:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec300616477b9d80495ba13d66ca7b8fa6cce43b3ffe1bc74b88c93219974cc`  
		Last Modified: Wed, 06 Oct 2021 00:31:59 GMT  
		Size: 2.3 MB (2348974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aafe80a9c15b3d27184f3617e4f09ad22eb4fac474f7b35687f6419d735259f`  
		Last Modified: Wed, 06 Oct 2021 19:14:15 GMT  
		Size: 3.3 MB (3264786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
