## `python:3-alpine3.15`

```console
$ docker pull python@sha256:acd274c3570f74941e4fffa11868977e56885da69b93cbeff47249b12953f243
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

### `python:3-alpine3.15` - linux; amd64

```console
$ docker pull python@sha256:8ce0a21b7d85c4e4c4d7673313300b281dc1f186eb559f70532401a2f58d69f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19128460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d2b99d7d12ae258ead417b7b4e4133f5b738ce5fa48054b01bd12ca7d7cd153`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:34:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 23:52:37 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 23:52:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 23:52:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 00:23:04 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 00:34:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 00:34:42 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 00:34:42 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 00:34:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 00:34:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 00:34:42 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 00:34:49 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 10 Aug 2022 00:34:49 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abed0206f3914209d0e7a549b92f3b0c85b421285ab998e63ea64d093f71289f`  
		Last Modified: Wed, 10 Aug 2022 01:10:37 GMT  
		Size: 681.7 KB (681669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0ae0fe5b972748ea6475feec4cd2238797fd89b8870a9f4a572f29488e5f88`  
		Last Modified: Wed, 10 Aug 2022 01:11:25 GMT  
		Size: 12.6 MB (12579372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8792c1c2edc87ab51a97c35dd511344734a625d1e67e3fd27dcfaa37ebe8eaf`  
		Last Modified: Wed, 10 Aug 2022 01:11:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c3163263951b8db5f16b425ff9fa11c0d27ac386dfaa17e7c9bfd0762140c5`  
		Last Modified: Wed, 10 Aug 2022 01:11:24 GMT  
		Size: 3.0 MB (3043676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; arm variant v6

```console
$ docker pull python@sha256:5c89427bc49bfda7a517b0df9cd0992bb5289705e3d1057ce07c85db68f99637
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18543579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec18ac0cae8ee561dd70ab91cc478508a8fe505372ce8fbda57d4c324bd548f0`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 18:18:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 18:18:14 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 18:18:16 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 18:18:17 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 19:20:04 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 19:42:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 19:42:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 19:42:45 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 19:42:45 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 19:42:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 19:42:46 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 19:42:54 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 10 Aug 2022 19:42:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ffb5a5eb61dba811bebee42c028e0f7aef3d3df8e5c47384f70d407bde2b92`  
		Last Modified: Wed, 10 Aug 2022 23:49:25 GMT  
		Size: 686.0 KB (686047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9061da9f860abfa7fbfbe7e7e8d4653c1902ce8f7307b0db6202a3ae04951f92`  
		Last Modified: Wed, 10 Aug 2022 23:50:12 GMT  
		Size: 12.2 MB (12182510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e438f718776db2c7c16c027c5a1b07c41c307f5e6de01df502cd64b33c9b2c16`  
		Last Modified: Wed, 10 Aug 2022 23:50:09 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbeac1c88ab2c0973af18646fbfd167b14788a564f89a91e01cb917a24279ef`  
		Last Modified: Wed, 10 Aug 2022 23:50:10 GMT  
		Size: 3.0 MB (3043664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; arm variant v7

```console
$ docker pull python@sha256:501506f0231e7304c9749aa90a471794ccb55419b6967a4cca04383a2187d11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17783237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e96d2d2a25731d3a0dd95419f77ec4d83d107f214fba5c0385b296d4c91b5d`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 04:57:41 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jul 2022 04:57:43 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 27 Jul 2022 04:57:43 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 03 Aug 2022 08:08:09 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 03 Aug 2022 08:36:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 03 Aug 2022 08:36:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 03 Aug 2022 08:36:34 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 03 Aug 2022 08:36:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 03 Aug 2022 08:36:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 03 Aug 2022 08:36:34 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 03 Aug 2022 08:36:42 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 03 Aug 2022 08:36:42 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160bb0cf7786cf6b48cf804a1d4042e10c1a858aec2d9924fd3a1686331cdc9`  
		Last Modified: Wed, 27 Jul 2022 10:55:07 GMT  
		Size: 664.4 KB (664428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f021678d328a222599b0f84455c3ce258d40b2c5ec887db89205c49c8dd53fc`  
		Last Modified: Wed, 03 Aug 2022 11:23:17 GMT  
		Size: 11.7 MB (11650342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb0c812a990c93a5c3791cef2149fbee3cbe0dd63e810300445d417bfc70229`  
		Last Modified: Wed, 03 Aug 2022 11:23:14 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb0ae1fbdb7be8343185c49d0de8268b5161dfec452c10a87a6906b935f5786`  
		Last Modified: Wed, 03 Aug 2022 11:23:16 GMT  
		Size: 3.0 MB (3043684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull python@sha256:4c8c8a288aadf5825e5321b225cfb1ed2a4c084660b908ba4c265990044b7140
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19118554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d0b1e1972a19769bc495833d03d89de0564bf3c0e2badca2b440d7986dd7d1`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:34:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 03:18:22 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 03:18:24 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 03:18:25 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 03:58:24 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 04:12:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 04:12:44 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 04:12:44 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 04:12:45 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 04:12:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 04:12:47 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 04:12:55 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 10 Aug 2022 04:12:55 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e18021c0d0bf0a6f79a44bbbd33f12adeb2ef1358b140d8e7ef36e20c1e63b3`  
		Last Modified: Wed, 10 Aug 2022 04:54:58 GMT  
		Size: 682.4 KB (682394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e9f93fe23985a1f4d1d090e4ced82c31b2fabd4922b7761e42cfe7b56b9d7`  
		Last Modified: Wed, 10 Aug 2022 04:55:55 GMT  
		Size: 12.7 MB (12672520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025a0ca8e87cb11983c19a8a09007c64a9ebe5d2f9efe96b36658d2221721b7`  
		Last Modified: Wed, 10 Aug 2022 04:55:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f9478f8adde516d76ac795893ebdd57bef837bde7fb060ec7bb45bbddf28a4`  
		Last Modified: Wed, 10 Aug 2022 04:55:54 GMT  
		Size: 3.0 MB (3044970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; 386

```console
$ docker pull python@sha256:b192844b2f3ed52c4bd27eae51f32c59b2c94220499c820ebb6f44123c5eb0c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19352393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f4f02bbee919d92d62ba600acb457b3e8e36a01475b53a7e871e612f5ad631`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:43:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 21:43:33 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 21:43:35 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 21:43:35 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 09 Aug 2022 22:16:44 GMT
ENV PYTHON_VERSION=3.10.6
# Tue, 09 Aug 2022 22:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 09 Aug 2022 22:28:46 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 09 Aug 2022 22:28:47 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Tue, 09 Aug 2022 22:28:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 09 Aug 2022 22:28:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Tue, 09 Aug 2022 22:28:50 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Tue, 09 Aug 2022 22:28:58 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 09 Aug 2022 22:28:58 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85493f06a4d298771cbb909dbd9b1d57f7b880cba7ae03576fbca04d8f72aac`  
		Last Modified: Tue, 09 Aug 2022 23:12:42 GMT  
		Size: 688.4 KB (688444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b2654af5e715020f30fc205902ed73673461fbc6e5a03e4cb568e5a768c8c5`  
		Last Modified: Tue, 09 Aug 2022 23:13:44 GMT  
		Size: 12.8 MB (12790216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca50f32ce6ff078672a17817ea255f70385341971ecba82de3107147443a7`  
		Last Modified: Tue, 09 Aug 2022 23:13:42 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9c6bbba3ab51211b0620fe30af3a47142ba795593985ff5c8d1faf42a3fa75`  
		Last Modified: Tue, 09 Aug 2022 23:13:43 GMT  
		Size: 3.0 MB (3044986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; ppc64le

```console
$ docker pull python@sha256:9a0b4991f0e98c982c7ac9e2134b2aa870c363887d043e0be209f5ecce557195
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19408095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73fddc54633d5d7fc3190f3918361c0c79d2746763ba2bfb5ea8a8172368f276`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:25:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 23:25:33 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 23:25:36 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 23:25:36 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 00:31:18 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 00:55:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 00:55:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 00:55:50 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 00:55:50 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 00:55:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 00:55:50 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 00:56:01 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 10 Aug 2022 00:56:02 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed23ac268a650a18b29c43bba4ed3f8bf6e5965204891186cd09aa3ef25e36b`  
		Last Modified: Wed, 10 Aug 2022 02:04:48 GMT  
		Size: 689.5 KB (689462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82318c7ff0e498a2fd1b6026f3b543fcecd6769b84e76495174506a4f4bb97d8`  
		Last Modified: Wed, 10 Aug 2022 02:05:58 GMT  
		Size: 12.9 MB (12861742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43102fd2469865d778d5fa6c8c0b10a87a49f8b74ff9d4cebe8b61e35409f3b4`  
		Last Modified: Wed, 10 Aug 2022 02:05:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1b0f0aaf6003a3e0acd1b53b977e9f9649779a4a953cce1d47031d54264025`  
		Last Modified: Wed, 10 Aug 2022 02:05:56 GMT  
		Size: 3.0 MB (3043671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.15` - linux; s390x

```console
$ docker pull python@sha256:76d33e2fe85a9459650c8325f34b649e9de0ee2c6d029e98a6e2c01e563debfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18868556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbd721a1beb11d44e08056be60a52df9fd29d8e839a41f61f61ad785abc69e5`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 03:48:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 03:48:06 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 03:48:07 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 03:48:08 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 04:17:44 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 04:28:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 04:28:42 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 04:28:42 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 04:28:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 04:28:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 04:28:43 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 04:28:48 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 10 Aug 2022 04:28:49 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee37501817aef5de6d1dac4638e5a31f15dc46a5e04537e47809034a7d4e51bb`  
		Last Modified: Wed, 10 Aug 2022 05:10:23 GMT  
		Size: 686.5 KB (686538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ca4b275e260c95893ad56ac5d5c8615809f71b0d6dfe1f02427665122c97e`  
		Last Modified: Wed, 10 Aug 2022 05:16:11 GMT  
		Size: 12.5 MB (12532019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b2b39654fdd7f952d9618725c805bc9fce31bab251bb3311d44839c5673c4b`  
		Last Modified: Wed, 10 Aug 2022 05:16:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6e97a8d92150bb5e77f69be6d52c10f0f7ad7471c135dab9de97310d27ee7a`  
		Last Modified: Wed, 10 Aug 2022 05:16:11 GMT  
		Size: 3.0 MB (3043681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
