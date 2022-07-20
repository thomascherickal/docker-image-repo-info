## `python:alpine3.15`

```console
$ docker pull python@sha256:4daf5b7266b05d25aa65f39b9b96b9b6bb4428fed2837ebfb75688c9d2d95853
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

### `python:alpine3.15` - linux; amd64

```console
$ docker pull python@sha256:fbee5312e64b18cf6a91f93e26286f706dd7182cbb5842fdb54ddeeadce37f68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18602807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fc3c8dd611f7bddec5040dd6d6878470edd88c987f6ea84f2034400ea6ccfa`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 00:55:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 00:55:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 00:55:50 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 00:55:50 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 01:15:10 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 01:27:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 01:27:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 01:27:15 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 01:27:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 01:27:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 01:27:16 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 01:27:23 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 01:27:23 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104c00f00fd409ba0bcd53013de4550f2fa8c11643bf08c73bfe912dfaa7173f`  
		Last Modified: Wed, 20 Jul 2022 01:46:17 GMT  
		Size: 667.0 KB (667029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bb4199dd008e2d8181fc9170df6149312411b8ad72b2751ebabec1546b0c21`  
		Last Modified: Wed, 20 Jul 2022 01:46:40 GMT  
		Size: 12.2 MB (12249175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282d7b44528b2363df9590c02dfa89d03dc8c8e07641f9e99b04feadcbeedd4f`  
		Last Modified: Wed, 20 Jul 2022 01:46:38 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72eaecd995e7165a04a2bdc7e310fd9c109a1d235624018e46a0501f9fa82f22`  
		Last Modified: Wed, 20 Jul 2022 01:46:38 GMT  
		Size: 2.9 MB (2871726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; arm variant v6

```console
$ docker pull python@sha256:c4ff16f436ba8efb925af39355dcf6d18c8c1b020255c7246d5fee0646d7bccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (18023090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe29cc8019a2523bfbdab59655ed76d32843c996359ad2507a3a0e15ad958864`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:15:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 02:15:53 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 02:15:57 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 02:15:57 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 03:08:51 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 03:40:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 03:40:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 03:40:29 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 03:40:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 03:40:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 03:40:30 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 03:40:49 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 03:40:49 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95496765c3eea135bec54cd474e3f227324e161b2048725f814b5d79b65139c6`  
		Last Modified: Wed, 20 Jul 2022 04:26:53 GMT  
		Size: 672.6 KB (672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da0af7dcb94acfda97f0967a833ddfa5e8b765b8b430f7b72edbeaa8173e164`  
		Last Modified: Wed, 20 Jul 2022 04:27:30 GMT  
		Size: 11.9 MB (11856094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374204206ca201475319596e94be769996dfe31e91d431525b5925bd34714501`  
		Last Modified: Wed, 20 Jul 2022 04:27:22 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6775977d1f1eb984d6ffd379240e591af5d96f9db9fcdc02198680154116176a`  
		Last Modified: Wed, 20 Jul 2022 04:27:25 GMT  
		Size: 2.9 MB (2871731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; arm variant v7

```console
$ docker pull python@sha256:f87c125d7801e8a92c4ffe42aaddda833ffa162323f38b08365561da34f0d3ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17284674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df72f71d546ad2c9511a5458a8b43a946668d21512836e6a96f5c7e4264f5e9`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:17:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 04:17:34 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 04:17:38 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 04:17:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 05:09:44 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 05:39:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 05:39:43 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 05:39:44 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 05:39:45 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 05:39:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 05:39:46 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 05:40:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 05:40:05 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b4e08adc6c51be71918c2499f44e7ce288aa814bb612695fef35f9513c1e14`  
		Last Modified: Wed, 20 Jul 2022 06:29:55 GMT  
		Size: 664.5 KB (664511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff47b636245cff2a041e2b34fac96658eff98ad00be2fc6953e8f97d489c4fd`  
		Last Modified: Wed, 20 Jul 2022 06:30:59 GMT  
		Size: 11.3 MB (11323563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3822e811a2c11bc97634c26facab7dccdb08d9d9da49e3a04cc4d245da5c8`  
		Last Modified: Wed, 20 Jul 2022 06:30:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7c94939462bad97b36a1c0ce26a4d70b109ffc88d1981491924a7d71afa9d2`  
		Last Modified: Wed, 20 Jul 2022 06:30:55 GMT  
		Size: 2.9 MB (2871819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull python@sha256:3dc7ccb610f7315ad3406c68e6a844a532bae0de32c57bda513261c08288d0a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18600530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ce1dbe47fd2f5c3ddd5ea52982873531350fa145b6aac3cac4ffedeb6ded1b`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:57:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 02:10:42 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 02:10:44 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 02:10:45 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 02:35:48 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 02:50:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 02:50:17 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 02:50:18 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 02:50:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 02:50:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 02:50:21 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 02:50:29 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 02:50:29 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6938290767f83c2e8755b418b6149f6a587370f4c9b69e1e12b1c0df232351`  
		Last Modified: Wed, 20 Jul 2022 03:13:01 GMT  
		Size: 668.4 KB (668425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b314e2ee58f5820a5bd4f72ad07be371370abedadd87633460a4acedb0008524`  
		Last Modified: Wed, 20 Jul 2022 03:13:35 GMT  
		Size: 12.3 MB (12343445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051f7d29766484de762b1a007b0304ad3c8dd0300c2932e5879e0f1cc466f54`  
		Last Modified: Wed, 20 Jul 2022 03:13:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c15be516c5352e4f040152a930ed1118aca3079de3146a671e061263b401a`  
		Last Modified: Wed, 20 Jul 2022 03:13:34 GMT  
		Size: 2.9 MB (2871539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; 386

```console
$ docker pull python@sha256:df4e93ab5356bb6e24a3fbc8ae02d853e5466d72c5e8ea2e2fe16a76cd391731
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18826813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3454767c6165fa3e7ffa69c550df9f2eb4f5f247ab63b01c73f07f8b78856a31`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 01:05:29 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 01:05:30 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 01:05:32 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 01:05:33 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 01:25:03 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 01:37:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 01:37:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 01:37:06 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 01:37:07 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 01:37:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 01:37:09 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 01:37:17 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 01:37:18 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fad5fdc3628ec3ae8e826916d0011c98c35fdae07ae64520a9a3abb5e03a8c`  
		Last Modified: Wed, 20 Jul 2022 01:59:58 GMT  
		Size: 674.8 KB (674836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8256bcd1973120bf361920ec0ecfdadbaf47359c54837b1b9ae14caee642fe`  
		Last Modified: Wed, 20 Jul 2022 02:00:35 GMT  
		Size: 12.5 MB (12460874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3bbdda5532881fa472e6f97b16bd30beb8f032971d437ed243eb01862c68c1`  
		Last Modified: Wed, 20 Jul 2022 02:00:33 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a096bcbfb54b38059a35a8a673784980fc0a837d69306726b29311bd7f2efe5b`  
		Last Modified: Wed, 20 Jul 2022 02:00:33 GMT  
		Size: 2.9 MB (2871509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; ppc64le

```console
$ docker pull python@sha256:1bee46063403458d16ce7334940acfc62c18e07acd27013a01bd9c20d8888640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18891869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50575ec71f32d80af921f141d3c8ea4ddc95db39467bb67a92133904fdc1e008`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:19:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jul 2022 02:19:50 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 02:20:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 20 Jul 2022 02:20:09 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 02:56:10 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 03:17:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 03:17:48 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 03:17:54 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 03:18:00 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 03:18:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 03:18:14 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 03:18:43 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 03:18:48 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082a962dd58d4da7e735b94dea1262a5dcd1295279e6a5e9c8bdf164a21873e7`  
		Last Modified: Wed, 20 Jul 2022 04:00:58 GMT  
		Size: 676.5 KB (676527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ae9fe43806e1685cd6c0d03365621fb4cf79007152d477ec5a9247b5f1e4ca`  
		Last Modified: Wed, 20 Jul 2022 04:01:38 GMT  
		Size: 12.5 MB (12531761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedb794881ec06e52663c7ffdcbf724a40059b4c275403ca518c9bd9acf47228`  
		Last Modified: Wed, 20 Jul 2022 04:01:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367fde6a7d7c9fa19da2c9cb956b733966c5d2190e5b16609a5a1ec77131620a`  
		Last Modified: Wed, 20 Jul 2022 04:01:36 GMT  
		Size: 2.9 MB (2871709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:alpine3.15` - linux; s390x

```console
$ docker pull python@sha256:51bfa9569ddeda4eaaf8355bb70a460db335452b21e5e2fcd31e626940916c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18353849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef69755d71daf7abcdbb1438f86ecd3cfb30320d4eb305bc65c9ba123c02580`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 19 Jul 2022 22:41:55 GMT
ADD file:9671b14d87fd7602279c1b3d1148babaa2c411e4ab0570d294d95324fa19210c in / 
# Tue, 19 Jul 2022 22:41:56 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:43:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Jul 2022 23:43:39 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 23:43:41 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 19 Jul 2022 23:43:43 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 20 Jul 2022 00:08:24 GMT
ENV PYTHON_VERSION=3.10.5
# Wed, 20 Jul 2022 00:28:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 20 Jul 2022 00:28:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Jul 2022 00:28:43 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Jul 2022 00:28:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 20 Jul 2022 00:28:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 20 Jul 2022 00:28:45 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 20 Jul 2022 00:28:54 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Jul 2022 00:28:57 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ef614dc1febe442e84bcc0f287628aea0f6547a0f322d7bed0a46ffabd5e0a50`  
		Last Modified: Tue, 19 Jul 2022 22:43:17 GMT  
		Size: 2.6 MB (2600789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419e43a45321b88539b62ef9c20295d0aca1152bc94775af95b63fa6b9492b1c`  
		Last Modified: Wed, 20 Jul 2022 01:00:34 GMT  
		Size: 672.6 KB (672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce0914a684026d73142fb3ba70b006cb656802826e5fb36f2d8b9366f775214`  
		Last Modified: Wed, 20 Jul 2022 01:01:13 GMT  
		Size: 12.2 MB (12208528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae4bcc4743bc72bbef6c82ad0ce13e209e9183d25d86f5977fa02ed20b2ddd0`  
		Last Modified: Wed, 20 Jul 2022 01:01:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e987af1977cf25f16ff2fa9881add656e0696c33a90bbeec3a8d7ddd1647a4`  
		Last Modified: Wed, 20 Jul 2022 01:01:12 GMT  
		Size: 2.9 MB (2871711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
