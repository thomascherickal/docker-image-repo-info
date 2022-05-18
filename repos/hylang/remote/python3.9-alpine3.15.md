## `hylang:python3.9-alpine3.15`

```console
$ docker pull hylang@sha256:f95bf34abd6f3439cd3fb95f78fa49e0c939c3e003978fe59b8b04d3e7548b51
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

### `hylang:python3.9-alpine3.15` - linux; amd64

```console
$ docker pull hylang@sha256:2cbffa1edb381a9c269ec639b3fa9ec5208c50d5fbefd740664971a4db16c98b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22855348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04cb3ad7b66a3678b0f1b9b3f568cb74108ca919dd26a06330dfbcab822d5fd1`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:55:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:50:45 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 07:50:46 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 08:57:54 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 02:33:38 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 02:38:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 18 May 2022 02:38:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 02:38:12 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 02:38:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 02:38:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:38:13 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:38:20 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:38:20 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:30:45 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:30:45 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:30:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:30:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ef3e6b7a02c0ce1d7d3ee96f273c2c5074b3f127082b4cd3f629f82097e1a8`  
		Last Modified: Tue, 05 Apr 2022 09:38:17 GMT  
		Size: 667.0 KB (667029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b7769af0709a58ec8e18c527dbf5a740a9392da6f195569a3ae94f65263f3b`  
		Last Modified: Wed, 18 May 2022 02:51:06 GMT  
		Size: 13.6 MB (13584414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeefedcfa76158549020ac809422d85bbf044313d198b47d2f938afbc7615ea`  
		Last Modified: Wed, 18 May 2022 02:51:04 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cbc3d14cc64f2b6731207dd2a11295d96cc5ed53bed2546e89e223145ca001`  
		Last Modified: Wed, 18 May 2022 02:51:05 GMT  
		Size: 2.9 MB (2871647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259b1d324aee59c141b702ffcb233150262df8c4dc5195083584554c058c3b44`  
		Last Modified: Wed, 18 May 2022 04:34:53 GMT  
		Size: 2.9 MB (2917470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; arm variant v6

```console
$ docker pull hylang@sha256:e573b215aa5def9efa165b5072d980bcf73010b978d27e9198f6c68ab38210e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.0 MB (21973206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c613bcefab68757775e31c84a9eb97747c78b9a71ebfcc620ac3ee014a17f2`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:16:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:16:39 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 07:16:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 09:54:23 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 01:12:53 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 01:24:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 18 May 2022 01:24:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 01:24:41 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 01:24:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 01:24:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 01:24:43 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 01:25:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 01:25:05 GMT
CMD ["python3"]
# Wed, 18 May 2022 02:41:28 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 02:41:28 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 02:41:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 02:41:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c148f0a21858ba6d892e5c2be6f7a4cdc7017f1eb8f0dfe07a2aa14cdcf6d2`  
		Last Modified: Tue, 05 Apr 2022 11:23:18 GMT  
		Size: 672.6 KB (672638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cff719c6ca2dbaa050c4fd8fce6b140624ed35e2051d32b2e6673c50c0db16`  
		Last Modified: Wed, 18 May 2022 01:44:19 GMT  
		Size: 12.9 MB (12888809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d1525396999f95e47c1e73536ea25f660a4b1b2b673eda1bb65ceec6aa29ac`  
		Last Modified: Wed, 18 May 2022 01:44:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a06c390b1455d103fa57e4e978811aa96f93002c491e0fff29dea1ed11cbcc`  
		Last Modified: Wed, 18 May 2022 01:44:13 GMT  
		Size: 2.9 MB (2871710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b2ca580d0eff1370cd0ec8e3856af8fb40e828d006826dc8dbd9aeff3a884`  
		Last Modified: Wed, 18 May 2022 02:46:47 GMT  
		Size: 2.9 MB (2917847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; arm variant v7

```console
$ docker pull hylang@sha256:0137c12c7922922c2d16100df7ebbf2149f3def009f8ff26fec5bae61545cef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19982969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcddbf816cf8940d1f0d59d205e11cb60112343d1d172ded07105920d9ce36a2`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:15:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 11:15:50 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:15:53 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 13:50:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 13:50:15 GMT
ENV PYTHON_VERSION=3.9.12
# Wed, 20 Apr 2022 08:41:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 08:41:13 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 08:41:14 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 08:41:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Apr 2022 08:41:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 08:41:15 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 08:41:32 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 08:41:33 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 19:25:02 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 19:25:02 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 19:25:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 19:25:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5594b60729afc7fdfa6de04dfddfc5560d7ca2510331911a8b6c27a5fd65f469`  
		Last Modified: Tue, 05 Apr 2022 15:18:31 GMT  
		Size: 664.5 KB (664505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373a9242aaabf4d9d9f5b9baa563defbe622cf8936f0034a803132f8973675d2`  
		Last Modified: Wed, 20 Apr 2022 12:52:30 GMT  
		Size: 11.1 MB (11105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd747ff5f189c0e2eafc6bd945cfde8fdda7cc2a2f11634876a5158b7ef26d0`  
		Last Modified: Wed, 20 Apr 2022 12:52:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b03f7dfba77908c35ea9e1b35a45c056fb5b941b0aa5ad15099cbe216b88a2c`  
		Last Modified: Wed, 20 Apr 2022 12:52:26 GMT  
		Size: 2.9 MB (2871819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c563f04621c088336cc7f913fb685b0719aebc75b50916a1befaa9a9b3f2f05`  
		Last Modified: Wed, 20 Apr 2022 19:34:48 GMT  
		Size: 2.9 MB (2916608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:19876e90cb43ce5959440ae5099389df46a287bc9729fe866aa74590a5980cc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22680089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ed90da686e5fdd49fe8cfe784a0b6f357d3148ebeaae1c30de6eb8afa50adf5`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:43:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:43:56 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:43:58 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 06:01:50 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 04:30:06 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 04:34:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 18 May 2022 04:34:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 04:34:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 04:34:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 04:34:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 04:34:49 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 04:34:57 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 04:34:58 GMT
CMD ["python3"]
# Wed, 18 May 2022 05:44:15 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 05:44:15 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 05:44:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 05:44:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c8fe6b300068ece063b73d7ea69bef331e0698246ebbe2abe966cf6685e1ef`  
		Last Modified: Tue, 05 Apr 2022 06:41:57 GMT  
		Size: 668.4 KB (668392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f865b1253cefccc2b838100b444f4b41c819992dcb41513bf8c80f4ca3dded2c`  
		Last Modified: Wed, 18 May 2022 04:50:47 GMT  
		Size: 13.5 MB (13508006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e4645dadd435363b9adbf0c87eae55ae02a5e0c42768a7d5a5a995be37cfe`  
		Last Modified: Wed, 18 May 2022 04:50:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1352d86eb5ca7dfe5c8a5bb8b130a79ccb1f072982023a8e368e46d49919d1`  
		Last Modified: Wed, 18 May 2022 04:50:45 GMT  
		Size: 2.9 MB (2871584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc1fbe84d070a6101aa1a62c4fb65ed9263a63ac7135ab19f4b7885e2dee78`  
		Last Modified: Wed, 18 May 2022 05:50:42 GMT  
		Size: 2.9 MB (2915400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; 386

```console
$ docker pull hylang@sha256:3233606ab29ac703077ada96fe50cacb6f5dafd167a06519883dc617e50b6daa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23050136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a414ba4c5cce96b27178c17c952bf099f481d2db44d246ee6ab7396501a164a8`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:41:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:41:33 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:41:35 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 05:43:41 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 03:04:46 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 03:09:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 18 May 2022 03:09:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 03:09:55 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 03:09:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 03:09:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:09:58 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:10:07 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:10:08 GMT
CMD ["python3"]
# Wed, 18 May 2022 03:47:42 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 03:47:43 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 03:47:48 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 03:47:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123e2fc95f4f26c5ef818012e9569da127091f4bda4bbd8d1b992ff1d9fca0f0`  
		Last Modified: Tue, 05 Apr 2022 06:24:17 GMT  
		Size: 674.8 KB (674790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ff8db6776a52cc90d87a47cd82585538b8fdd475f901fba8c325870f1161fd`  
		Last Modified: Wed, 18 May 2022 03:27:16 GMT  
		Size: 13.8 MB (13769279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1dac834d4ae946af308a3105ae5cebae4fa2c98ac7a28136a396f0e0f87ab6`  
		Last Modified: Wed, 18 May 2022 03:27:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45398f92f30acbce575a6736930dbcb7780f66bf2344893e3b0650bbee33be93`  
		Last Modified: Wed, 18 May 2022 03:27:14 GMT  
		Size: 2.9 MB (2871546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a0ce2f7f3e0b2a05bb831748db452f0da65142b79ac5a6a2f148186cf68f03`  
		Last Modified: Wed, 18 May 2022 03:54:26 GMT  
		Size: 2.9 MB (2915316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; ppc64le

```console
$ docker pull hylang@sha256:d417351d207a5a3108967f801a4c52a84ab38213f8f5e8c58b059189348d1ae7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21609501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a1fe9de742359ddfa850d5b3c44610fa35a59da6120e9876341650dc46bd86`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:00:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 16:00:44 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:00:54 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 17:54:18 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 05 Apr 2022 17:54:21 GMT
ENV PYTHON_VERSION=3.9.12
# Wed, 20 Apr 2022 05:53:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Apr 2022 05:54:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 05:54:10 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 05:54:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Apr 2022 05:54:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 05:54:33 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 05:55:00 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 05:55:05 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 15:58:45 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 15:58:54 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 15:59:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 15:59:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383b0511332251ebc07b3b84ac239f2c956371bd46dbe7229965dd10db503224`  
		Last Modified: Tue, 05 Apr 2022 19:05:19 GMT  
		Size: 676.5 KB (676534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343612bc58d1b61f605c719937f0d27c7c206c7cabcd9e34286e3ad50d4d1c95`  
		Last Modified: Wed, 20 Apr 2022 09:09:00 GMT  
		Size: 12.3 MB (12332586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b417c56dcbee0db6b6e9b97bb7c3d83b1f30237bffc2fac94a9bf372f8a4192`  
		Last Modified: Wed, 20 Apr 2022 09:08:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dc48bf64c9496ee58f1fc1b3d36c470891645568698d1eebd6b817614d0524`  
		Last Modified: Wed, 20 Apr 2022 09:08:59 GMT  
		Size: 2.9 MB (2871660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdb0ea80892f5ffdc7096831e7cfa312a1e59c5623d1b2fefd42aa133e2a1fa`  
		Last Modified: Wed, 20 Apr 2022 16:14:26 GMT  
		Size: 2.9 MB (2917304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.15` - linux; s390x

```console
$ docker pull hylang@sha256:4c539c10216b261a397c9a4c1351a7c8ad0d24175872ed9b5babe5d29280db55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22334104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8104aa1a8c37db3cd18d3d7c7714baebc37c38190dc0b14ed6fb4fe05b94ab`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:24:38 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:24:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 05 Apr 2022 05:21:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 02:51:37 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 02:56:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 18 May 2022 02:56:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 02:56:38 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 02:56:39 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 02:56:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:56:39 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:56:46 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:56:47 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:51:32 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:51:32 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:51:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:51:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e008f4836aadf966085bfc88ab008beb623e1f799da4ac849b1532735dc5b`  
		Last Modified: Tue, 05 Apr 2022 05:59:03 GMT  
		Size: 672.6 KB (672601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c43f292eba7d8f637280632d1a9a34f65dcf9b405248ca0bdc438f918e50c`  
		Last Modified: Wed, 18 May 2022 03:12:31 GMT  
		Size: 13.3 MB (13271894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f010bc003f0cd66643ed34e0be6fc5e1e1c5ea2d09e87f20101f5711658c892`  
		Last Modified: Wed, 18 May 2022 03:12:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38be0aa4aed49f5ee5d07a7be611297cac1ef6ade3a804eec3172eb2625330`  
		Last Modified: Wed, 18 May 2022 03:12:30 GMT  
		Size: 2.9 MB (2871623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530bb0f64600b16fbb55d5e02b65b624422cdd62bb5077b33a2d321de0a424d`  
		Last Modified: Wed, 18 May 2022 04:57:07 GMT  
		Size: 2.9 MB (2917382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
