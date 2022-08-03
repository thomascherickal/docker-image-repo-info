## `python:3-alpine3.16`

```console
$ docker pull python@sha256:01126f0a13659e9365ea058078ccfb057155b205f4fba630845552b7e2a72e9e
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

### `python:3-alpine3.16` - linux; amd64

```console
$ docker pull python@sha256:c37301b8439432638163231fd441845fce3511dde0ec6f2e7e131b5b91e6ffea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (19018085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d057565b53c254724ac12f006d7497d5e7167a628f9cadd68fd2b4d43116387`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:14:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Jul 2022 02:01:52 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 02:01:54 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 19 Jul 2022 02:01:54 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 03 Aug 2022 10:48:21 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 03 Aug 2022 11:00:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 03 Aug 2022 11:00:14 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 03 Aug 2022 11:00:14 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 03 Aug 2022 11:00:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 03 Aug 2022 11:00:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 03 Aug 2022 11:00:14 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 03 Aug 2022 11:00:21 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 03 Aug 2022 11:00:21 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c14b1a767335de44f2bc926cb52487979a0fe602ac5429643dbb238f297fb`  
		Last Modified: Tue, 19 Jul 2022 02:56:13 GMT  
		Size: 666.8 KB (666769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571274b8543b548747b5e9bef700a89692fe9403cc364be8d6e8a0792ccfe2b4`  
		Last Modified: Wed, 03 Aug 2022 11:19:35 GMT  
		Size: 12.5 MB (12508608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f79a08255af5d614c7b4b81e358b5bb607bdcb14a6475c836d3d4f92f094846`  
		Last Modified: Wed, 03 Aug 2022 11:19:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b20e3f6abd46292c29437a6917dc82b769ebb239e2d971aedb6695e057715`  
		Last Modified: Wed, 03 Aug 2022 11:19:34 GMT  
		Size: 3.0 MB (3043671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; arm variant v6

```console
$ docker pull python@sha256:a484a0249a1313347284e5210c73cf8961c671a2be5ac84f1a0d75e1405bf8a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18407711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:839e9ef254141f37be3c86a40481762deb9816e3d1145cab0bd0eea18ba77157`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 00:30:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 00:30:05 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jul 2022 00:30:07 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 27 Jul 2022 00:30:07 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 02 Aug 2022 19:50:04 GMT
ENV PYTHON_VERSION=3.10.6
# Tue, 02 Aug 2022 20:30:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 02 Aug 2022 20:30:08 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 02 Aug 2022 20:30:08 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Tue, 02 Aug 2022 20:30:08 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 02 Aug 2022 20:30:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Tue, 02 Aug 2022 20:30:08 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Tue, 02 Aug 2022 20:30:20 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 02 Aug 2022 20:30:20 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ebe8e3a2f83d0ddc301c9b9d6405376eecb906b92082e05d5e257eff5f6293`  
		Last Modified: Wed, 27 Jul 2022 11:08:23 GMT  
		Size: 672.3 KB (672287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b647934af90a736595f675559fd3aebbcdbcfc67277de68401980916f3c217d7`  
		Last Modified: Wed, 03 Aug 2022 00:13:17 GMT  
		Size: 12.1 MB (12085055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaef313095ff837d4848dec2c5e458a33e59ee4e1ab7a9d4e3d244d20b92fbf`  
		Last Modified: Wed, 03 Aug 2022 00:13:12 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba453d098c35b58faf7cc2ac6a90a0e9a8941dc90611ee397d12af0a546bbe87`  
		Last Modified: Wed, 03 Aug 2022 00:13:15 GMT  
		Size: 3.0 MB (3043708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; arm variant v7

```console
$ docker pull python@sha256:4fd92f2e513daeaf98b9a3c0e54b6428830f1a5c4cd2c042ed0c1f093352dbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17679029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e758a4821ee3b2ff1b2b0392d756ae2ac58d70d6c0e0523be0ef6573c56a5f58`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 03:57:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 03:57:44 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jul 2022 03:57:46 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 27 Jul 2022 03:57:46 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 03 Aug 2022 07:37:59 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 03 Aug 2022 08:07:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 03 Aug 2022 08:07:43 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 03 Aug 2022 08:07:43 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 03 Aug 2022 08:07:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 03 Aug 2022 08:07:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 03 Aug 2022 08:07:43 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 03 Aug 2022 08:07:50 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 03 Aug 2022 08:07:51 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d826ef3e3e077607452c51ac5332613cc0a20903abe17b56af4b973f31f0e9b7`  
		Last Modified: Wed, 27 Jul 2022 10:54:47 GMT  
		Size: 664.1 KB (664079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116f12212b7e97cde5b72713f0f3a3025a9ef6dffccdc353cd4d15407d343a72`  
		Last Modified: Wed, 03 Aug 2022 11:22:41 GMT  
		Size: 11.6 MB (11558755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2affe775c9998dea9fd354aa8d4b6e97117d2092c84f1401265b9f9528bf7`  
		Last Modified: Wed, 03 Aug 2022 11:22:38 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032af4833525c8884057f85c0da98a7f2dedc337784e4ce3645fad79e6633b26`  
		Last Modified: Wed, 03 Aug 2022 11:22:39 GMT  
		Size: 3.0 MB (3043658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull python@sha256:5bbde516455ce8afad45d2be7b60d237ac59350aa22d755ad4ee1d367f60530f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18987008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:076c91fc96c500ad5c7747b3e9816e6655589842efeaa81be14db8886e8a291f`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:10:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Jul 2022 01:53:04 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 01:53:05 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 19 Jul 2022 01:53:06 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 03 Aug 2022 09:50:39 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 03 Aug 2022 10:05:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 03 Aug 2022 10:05:10 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 03 Aug 2022 10:05:11 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 03 Aug 2022 10:05:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 03 Aug 2022 10:05:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 03 Aug 2022 10:05:14 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 03 Aug 2022 10:05:21 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 03 Aug 2022 10:05:22 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c36086fc9356a3d9879c8427af90dd86ad6fd35b3929bab2af384e98d0571c`  
		Last Modified: Tue, 19 Jul 2022 02:56:56 GMT  
		Size: 668.0 KB (668022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255e9c7248a65c9bb1f14e3ffaf6aad2e14b965bfd9196b30e8c1efc8ddd1747`  
		Last Modified: Wed, 03 Aug 2022 10:34:00 GMT  
		Size: 12.6 MB (12579036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32815e9cd0f789447579f484cec5ed6ff5b006c50c121a5e314519ffad01d5`  
		Last Modified: Wed, 03 Aug 2022 10:33:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c6e4018f23818adb74c050daeddb28d2efddbabe1135f85ed3ef29b17ec7b`  
		Last Modified: Wed, 03 Aug 2022 10:32:56 GMT  
		Size: 3.0 MB (3045000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; 386

```console
$ docker pull python@sha256:b0e8ee0f00711ece5c32003a70bfc6c9bf6913a5c57018fecfc8eccc51ad4ce5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19226302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac76a1061b7429a36de011bdfcb540133155f3ef50cf9a72ceec2ecaa2e52d3`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:21:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:21:05 GMT
ENV LANG=C.UTF-8
# Mon, 18 Jul 2022 23:21:07 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Mon, 18 Jul 2022 23:21:08 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 02 Aug 2022 21:30:55 GMT
ENV PYTHON_VERSION=3.10.6
# Tue, 02 Aug 2022 21:44:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 02 Aug 2022 21:44:14 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 02 Aug 2022 21:44:15 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Tue, 02 Aug 2022 21:44:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 02 Aug 2022 21:44:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Tue, 02 Aug 2022 21:44:18 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Tue, 02 Aug 2022 21:44:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 02 Aug 2022 21:44:26 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81add88e4983e2c8a2a8a58ebbbe1fdd9bcc102840a2f963deb15868c8a5dc5`  
		Last Modified: Tue, 19 Jul 2022 00:21:43 GMT  
		Size: 675.7 KB (675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06d29fc7dfe4c15953dc4b894e3fd84f395f2c98607760c63b77ded01a90c35`  
		Last Modified: Tue, 02 Aug 2022 22:16:11 GMT  
		Size: 12.7 MB (12703125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ef7077067b36dff6e31c389c6c9c78003548b9399f64c63fb2bb387d58854e`  
		Last Modified: Tue, 02 Aug 2022 22:16:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fd884297ae0dcf9b37beeef0efc186bc1f732aadb7045796566fc904f0db4d`  
		Last Modified: Tue, 02 Aug 2022 22:16:09 GMT  
		Size: 3.0 MB (3044958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; ppc64le

```console
$ docker pull python@sha256:86dede11287c60729d0804df7386caad7058ba93bf4690fb82cfe9a3efc5d226
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18834533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cba334ac8a68a8625080fde03fbe26230f222bc9a4ea43808a4fbbb5b805313`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 04:30:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 04:30:31 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jul 2022 04:30:33 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 27 Jul 2022 04:30:33 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 27 Jul 2022 07:53:21 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 27 Jul 2022 08:18:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 27 Jul 2022 08:18:06 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 27 Jul 2022 08:18:06 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 27 Jul 2022 08:18:06 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 27 Jul 2022 08:18:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/49ca29908cfd49683da12f2d5a4fa5689539f9d9/public/get-pip.py
# Wed, 27 Jul 2022 08:18:07 GMT
ENV PYTHON_GET_PIP_SHA256=d077d469ce4c0beaf9cc97b73f8164ad20e68e0519f14dd886ce35d053721501
# Wed, 27 Jul 2022 08:18:18 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 27 Jul 2022 08:18:18 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6556a4bf6509d5fd24900f56a6175bd811b9dd8c6f4f51e2732b6888a2b8933`  
		Last Modified: Wed, 27 Jul 2022 13:49:16 GMT  
		Size: 677.0 KB (676971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c806c2bc68469734bbe706125e270bbf738f2696c21bf2e80b05d857a178e84`  
		Last Modified: Wed, 27 Jul 2022 13:51:45 GMT  
		Size: 12.5 MB (12485244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1acb5176ea379d6e3e4b82b59eaff423597d4177ff2392a6a83f57acd65d36`  
		Last Modified: Wed, 27 Jul 2022 13:51:42 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b3566ad9507965fe8d31128837465f149b92fc9f155a3140130bcaa2e3e0d`  
		Last Modified: Wed, 27 Jul 2022 13:51:43 GMT  
		Size: 2.9 MB (2882166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine3.16` - linux; s390x

```console
$ docker pull python@sha256:c1217cc2b126e4a68f78f1aaa3d19054e062b8a00b1aab67845b0702a1b24f46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18747823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaff54291e6034b11a3bd48c7e50f1a7d7ab90093caeddfb47a9db6a117b5f0`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 04:09:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Jul 2022 04:09:38 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 04:09:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 19 Jul 2022 04:09:43 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 02 Aug 2022 22:37:37 GMT
ENV PYTHON_VERSION=3.10.6
# Tue, 02 Aug 2022 22:50:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 02 Aug 2022 22:50:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 02 Aug 2022 22:50:18 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Tue, 02 Aug 2022 22:50:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 02 Aug 2022 22:50:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Tue, 02 Aug 2022 22:50:19 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Tue, 02 Aug 2022 22:50:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 02 Aug 2022 22:50:27 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6100d7a8cfed816e1755b4b85c302a33fe998ae286d22da0f48d519f3a08b6a`  
		Last Modified: Tue, 19 Jul 2022 05:17:06 GMT  
		Size: 672.6 KB (672554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925c960932b8f1328d255a78ae29cfae53d2504f03cf448e89dde21360c90d3`  
		Last Modified: Tue, 02 Aug 2022 23:24:37 GMT  
		Size: 12.5 MB (12450561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a7cd244e09a9d22e57bf6c91dd8ca6287b368647a7dceafb844fe4324c8772`  
		Last Modified: Tue, 02 Aug 2022 23:24:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d55f4112770d8deaf33220641ede07d09d11e03c231388209e3fdcd45bd873`  
		Last Modified: Tue, 02 Aug 2022 23:24:36 GMT  
		Size: 3.0 MB (3043680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
