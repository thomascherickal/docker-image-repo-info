## `hylang:python3.9-alpine`

```console
$ docker pull hylang@sha256:baeca7e185140e1944af8e939253a7c3de84553b95a38baf6c53ce180012cd27
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

### `hylang:python3.9-alpine` - linux; amd64

```console
$ docker pull hylang@sha256:986eedf21a348e285110474701a15d0677cab03273137e37a41050184824393c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21323150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc76f80e06659151a730b1f4b8ad0adf90d8ee23123e400137fe09a6bd0aad05`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:46:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 18:46:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 18:46:37 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 23 Mar 2022 19:20:25 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 00:42:09 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 00:48:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:48:11 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:48:11 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:48:11 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:48:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:48:11 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:48:19 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:48:19 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 01:42:49 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 01:42:49 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 01:42:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 01:42:53 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c376a57d64541d4fb26bf2ef05f4e63d8ab5428d4ba892cfd034814d8b016934`  
		Last Modified: Wed, 23 Mar 2022 19:42:18 GMT  
		Size: 667.0 KB (667007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673b199806b221ad31787e9e01099382f4d69f8591779c2f134af0530b2ff7f2`  
		Last Modified: Fri, 25 Mar 2022 00:59:43 GMT  
		Size: 12.1 MB (12055377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9e775bca1dd7124167752c99acfd2166f425a8bf77d551cc0ef284e6373343`  
		Last Modified: Fri, 25 Mar 2022 00:59:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402552d2973b1cbc8290d4ff5f295eb2a0564c6c7750b2d19cf94883e5c4ae07`  
		Last Modified: Fri, 25 Mar 2022 00:59:42 GMT  
		Size: 2.9 MB (2871715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7599889ce4e565d5941bcd0727fab9bb4d32a1cbd5853b0d56bf1d7253feff4`  
		Last Modified: Fri, 25 Mar 2022 01:47:06 GMT  
		Size: 2.9 MB (2916129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; arm variant v6

```console
$ docker pull hylang@sha256:7800ac7e37cb34366c8b550a80f6546acfb28eb8252bd7fca82a3005ffac4b79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20687370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c69945474e2cc324530cf05700c8a1da9498de82d532b53233cb17f77b4914`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:26:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 14:26:47 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:26:51 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 17:07:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 17:07:05 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 17:18:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 17:18:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 17:18:50 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 17:18:50 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 17:18:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 17:18:51 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 17:19:12 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 17:19:12 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 20:04:52 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 20:04:53 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 20:05:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 20:05:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f68fd14771c38a4aa3bf1daf0feb7f0b3c6e16162c62431333ba49edc411e6`  
		Last Modified: Tue, 29 Mar 2022 18:36:11 GMT  
		Size: 672.6 KB (672639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fb76a5aea9e622d96f6869a0c95a7fb41b2f9b7cbea618fa01f8c9a0da2582`  
		Last Modified: Tue, 29 Mar 2022 18:38:12 GMT  
		Size: 11.6 MB (11604202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a225b23d32bb43d0cda3970df364cb4bb5357fe533fb6d5e4ad9329a38c17f`  
		Last Modified: Tue, 29 Mar 2022 18:38:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d8c36d507d7cf50e3969556fd973120e2672a6e71c1f48adae7fe4e4242ba`  
		Last Modified: Tue, 29 Mar 2022 18:38:07 GMT  
		Size: 2.9 MB (2871711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8486d3161c110ba2f6c9292b8dad5b902d2b4ec5641544dee487e6c5ad92008f`  
		Last Modified: Tue, 29 Mar 2022 20:10:13 GMT  
		Size: 2.9 MB (2916642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; arm variant v7

```console
$ docker pull hylang@sha256:4b3826aa47c11b3284b91acd0e8266fffd975515c8449f27b1e7c5731a796f43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19985471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54c18990b96f500957049205fcd6b60b912dac3c4ab27c4124d1ae02992543a`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 00:04:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 00:04:25 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 00:04:29 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 24 Mar 2022 01:21:31 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 03:10:50 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 03:21:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 03:21:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 03:21:34 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 03:21:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 03:21:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 03:21:35 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 03:21:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 03:21:53 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 05:35:23 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 05:35:23 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 05:35:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 05:35:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb195b4e7b5f8402b8f04e2adf0ab694df44f873c3f8b3814dd47d4db3a66fe0`  
		Last Modified: Thu, 24 Mar 2022 02:10:52 GMT  
		Size: 664.5 KB (664480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427a809ce4f03256e34ce0adce3fbd25b7f371837a564c90bef2b247c28356da`  
		Last Modified: Fri, 25 Mar 2022 03:47:48 GMT  
		Size: 11.1 MB (11105325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48c127590ec0da6bfe0baeb386addaec52e6d7ed8659cc3e224e45a02a26f0`  
		Last Modified: Fri, 25 Mar 2022 03:47:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3861902c2c10d17da933efe9c28af400ca2b7be74198cd881cbbb4f694b81`  
		Last Modified: Fri, 25 Mar 2022 03:47:44 GMT  
		Size: 2.9 MB (2871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0635456b9b93a2c58cdeb47128e311cce7243d8196c374357c4c30a30f002b`  
		Last Modified: Fri, 25 Mar 2022 05:43:38 GMT  
		Size: 2.9 MB (2916589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a68a83b692504841f7dc27e7c451eecbeee0ccaf8c0dbb00efbba03f6b9377c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21276870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd10570c8c9fe48f6b8857b289a6f6e0ffa49569e6aca7096a79a40f7292076`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:41:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 07:29:10 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 07:29:12 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 24 Mar 2022 08:08:09 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 00:46:53 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 00:51:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:51:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:51:31 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:51:32 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:51:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:51:34 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:51:42 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:51:43 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 02:56:19 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 02:56:20 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 02:56:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 02:56:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a080f00eab238082423a2878cdffa0833b2f33a98a0d0111a910e88cee617a`  
		Last Modified: Thu, 24 Mar 2022 08:29:59 GMT  
		Size: 668.4 KB (668370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a38e45282b4a32308679f487462aa6251a5fb1195c02e522426295d7b7ea550`  
		Last Modified: Fri, 25 Mar 2022 01:03:48 GMT  
		Size: 12.1 MB (12107347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc30719b4bd3d37e3ba496f9b0f5408222a1b536f21788a9f49aee86cbf33c9`  
		Last Modified: Fri, 25 Mar 2022 01:03:47 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124c36568e389031b36b40cd3f283839231b84202aaf36a317b99e4656dfc362`  
		Last Modified: Fri, 25 Mar 2022 01:03:47 GMT  
		Size: 2.9 MB (2871540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf80d67231dfa62c06839b44df6565069727b4aefd8746cc3b3b305f59118193`  
		Last Modified: Fri, 25 Mar 2022 03:02:02 GMT  
		Size: 2.9 MB (2914660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; 386

```console
$ docker pull hylang@sha256:86fbf0488e355f4e208e9bb13a80b348b403c8ecce394fcd7efc4881ffdd954b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21518616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870d8727acd0401031ca34e466a91eb42a6eec05a3d443ff1446eb486d1ca153`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:39:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 06:39:40 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 06:39:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 08:21:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 08:21:48 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 08:26:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 08:26:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 08:26:50 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 08:26:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 08:26:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 08:26:53 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 08:27:02 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 08:27:03 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 22:59:06 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 22:59:06 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 22:59:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 22:59:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0969d3729bf15b7e264af4c0951865db24ed0edd4fcc9c71ff12987129f47243`  
		Last Modified: Tue, 29 Mar 2022 09:31:37 GMT  
		Size: 674.8 KB (674800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777f5c7fa25fb0beb3102aba5ce8cb4a0ed92e15c85d1b394f4f014695b9ea6e`  
		Last Modified: Tue, 29 Mar 2022 09:34:25 GMT  
		Size: 12.2 MB (12238310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7259878ea46430efa5c8f4a3906dc8fd27690e38b033fd6f0305e342ce5ae0`  
		Last Modified: Tue, 29 Mar 2022 09:34:23 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c8b890aa1267d800a24290f03dd22d472fec0c2e947c40dc8f8a7b00688e2`  
		Last Modified: Tue, 29 Mar 2022 09:34:24 GMT  
		Size: 2.9 MB (2871518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6efd69c86e93ade561403a855b7e30bc14f72d4bcc594aa339e2db9c5469ba`  
		Last Modified: Tue, 29 Mar 2022 23:06:52 GMT  
		Size: 2.9 MB (2914829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; ppc64le

```console
$ docker pull hylang@sha256:6269d7d93dfb637973c91ec065b634d00eb3717794d3c31baaa49fd48da31a49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21614091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58c41563c251e43ed3527d692729b443fe5b006b36832368e2854f4bb0a827df`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 00:58:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 00:59:01 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 00:59:12 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 24 Mar 2022 01:56:10 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 03:25:00 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 03:34:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 03:34:23 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 03:34:27 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 03:34:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 03:34:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 03:34:36 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 03:34:58 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 03:35:00 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 04:52:58 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 04:53:03 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 04:53:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 04:53:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f82ca06f130d1c35c8abc3d469e2e93e3659365537c04ac877ce72330c36b8b`  
		Last Modified: Thu, 24 Mar 2022 02:34:40 GMT  
		Size: 676.5 KB (676523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9260994e1922e68d6ea5bd70c26903644655ea7eed40d9221bf10aa871c2a8b4`  
		Last Modified: Fri, 25 Mar 2022 03:53:55 GMT  
		Size: 12.3 MB (12335009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca4ccfc4848fe1c9bfca8ea7cae6e13af64c195dd873578fd1bc37ec76029e0`  
		Last Modified: Fri, 25 Mar 2022 03:53:53 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0988d8fb39dfc992c43e69aa63efc14d830e0b01d6d9ff8bf23a73578e59b38`  
		Last Modified: Fri, 25 Mar 2022 03:53:54 GMT  
		Size: 2.9 MB (2871673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5aa3503ed6d41275483ff67a58c25757b0186a3496cb8c22d8a26523ce9742`  
		Last Modified: Fri, 25 Mar 2022 04:59:28 GMT  
		Size: 2.9 MB (2916612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine` - linux; s390x

```console
$ docker pull hylang@sha256:2acdb553417f2d9552595fbd6c7907a6c17cfbd090c4cf94397bb364f333e280
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21064219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafa833b8b509c1eded620ad6381711efeb488ee14aa36cc03234b656ac17559`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:47:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 11:47:33 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:47:40 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 13:14:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 13:14:51 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 13:19:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 13:19:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 13:19:41 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 13:19:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 13:19:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 13:19:42 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 13:19:49 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 13:19:49 GMT
CMD ["python3"]
# Wed, 30 Mar 2022 12:34:53 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 12:34:53 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 12:34:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 12:34:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c4b2c5f3f03430b7d61ab7e06c86d6909b6950a224b3ff225a85f23ac38639`  
		Last Modified: Tue, 29 Mar 2022 14:17:32 GMT  
		Size: 672.6 KB (672593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c4a056546183e9a1ff0b19c3d1c28703f4a7fcda92fa44288377bc7d1bba1`  
		Last Modified: Tue, 29 Mar 2022 14:36:29 GMT  
		Size: 12.0 MB (12002876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e229425167fa131d166f9935719fc719eaa0406282280957499a1786a77341`  
		Last Modified: Tue, 29 Mar 2022 14:36:29 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1040532ec126b4d1d8c037bb8dcdf0d25e233cbe85d5ab4a389d2cb159a56983`  
		Last Modified: Tue, 29 Mar 2022 14:36:29 GMT  
		Size: 2.9 MB (2871760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75e4d3549a73134c2b73259d328bb0775593b69c1bf618a55279efdb2325c00`  
		Last Modified: Wed, 30 Mar 2022 12:40:27 GMT  
		Size: 2.9 MB (2916316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
