## `hylang:alpine3.17`

```console
$ docker pull hylang@sha256:3e43dbe9e75ebf5eae991b2c325d861fe00daaad124cc4c226778c5a3a4d53b2
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

### `hylang:alpine3.17` - linux; amd64

```console
$ docker pull hylang@sha256:19ea54f85f4f023ca2aa60ca7c6f657f06bbfe7416461dd9f72338a23ad3059b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27756583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0991eabed5f49b221e430cceb7b1ddfdbb0efd1c38544b0597e051005339f58`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:05:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 20:09:04 GMT
ENV LANG=C.UTF-8
# Mon, 09 Jan 2023 20:09:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Mon, 09 Jan 2023 20:25:21 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 09 Feb 2023 01:10:29 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 09 Feb 2023 01:23:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Thu, 09 Feb 2023 01:23:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 01:23:34 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 09 Feb 2023 01:23:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 09 Feb 2023 01:23:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 01:23:34 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 01:23:41 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 01:23:41 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 02:52:16 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:52:16 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:52:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:52:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd9832a787c7d68019488dcae52ce17e79f7cc4217fb549f6ff5c3fa1e10a93`  
		Last Modified: Mon, 09 Jan 2023 21:10:29 GMT  
		Size: 622.9 KB (622912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dd72e16bfb249a8b5ff109993ea7a2cb3b9e6af2423a38b85e2b41f6f4f40e`  
		Last Modified: Thu, 09 Feb 2023 02:25:52 GMT  
		Size: 14.6 MB (14630967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c7fd8e6571a6fa0d81c4168b20583ad1b9f86035f4f83c3183c00092be9905`  
		Last Modified: Thu, 09 Feb 2023 02:25:49 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fab62934884ddb0ecd9bb1e2638105084cee1bdb85ac0afad83e6fc207200a4`  
		Last Modified: Thu, 09 Feb 2023 02:25:50 GMT  
		Size: 3.1 MB (3056450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629e245461daf9455ed53ed0ca2beb57dc32f56b70188b13abcf48d6a5b1496`  
		Last Modified: Thu, 09 Feb 2023 03:04:05 GMT  
		Size: 6.1 MB (6075397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; arm variant v6

```console
$ docker pull hylang@sha256:902ee9b02ced18954015dac4e77cc6f07efa6fbbf4e26b69104c23d6c32e573a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24957196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718fece492c4d044427779784aa1c11bc0e0d150423adcfe65fe6951315602b3`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:44:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 03:44:38 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 03:44:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 04:23:01 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 04:23:01 GMT
ENV PYTHON_VERSION=3.11.2
# Sat, 11 Feb 2023 04:41:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:41:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:41:30 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 04:41:30 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 04:41:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:41:30 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:41:37 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:41:38 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 09:42:12 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 09:42:13 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 09:42:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 09:42:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bc7384407f1883772f74c693a37ca7cbea92dd7cc7982c9f24fc04f6acf89d`  
		Last Modified: Sat, 11 Feb 2023 06:03:38 GMT  
		Size: 624.9 KB (624941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2566f42a84bff847bfc5f184d049f4f818db9d40561c4f257cff434edb62d7`  
		Last Modified: Sat, 11 Feb 2023 06:04:18 GMT  
		Size: 12.1 MB (12091997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5448eebe5a1e242d95b538ff9501c2c4b4e820d2c7aea722f4161672da2dc4bb`  
		Last Modified: Sat, 11 Feb 2023 06:04:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dc3c9f076959fdc686485cc9bb1ee89a4548fca0971fdb3ff85ba39d7c4abf`  
		Last Modified: Sat, 11 Feb 2023 06:04:17 GMT  
		Size: 3.1 MB (3056247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d00772100d4abcab3e1779007d0a841f99bc08d4171686f14e9679733e2d80`  
		Last Modified: Sat, 11 Feb 2023 09:50:29 GMT  
		Size: 6.1 MB (6072895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; arm variant v7

```console
$ docker pull hylang@sha256:b13251bf404243ab9eb89b5156066f7c0cd404b1f05712ec9658e414e9f14cde
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26033637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389efb23f02e4cbe5a890c522ca640c6d8f3c235f13e8f2dcfb67723ea857739`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 23:33:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 23:33:02 GMT
ENV LANG=C.UTF-8
# Mon, 09 Jan 2023 23:33:04 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Mon, 09 Jan 2023 23:54:03 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 09 Feb 2023 02:57:25 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 09 Feb 2023 03:15:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Thu, 09 Feb 2023 03:15:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 03:15:53 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 09 Feb 2023 03:15:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 09 Feb 2023 03:15:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 03:15:53 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 03:15:59 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 03:16:00 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 05:42:41 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 05:42:41 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 05:42:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 05:42:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195bafe2485bbd04fb274d28ba1a61517e45d8f137b6f88b96705db2ccdd1982`  
		Last Modified: Tue, 10 Jan 2023 00:53:21 GMT  
		Size: 623.9 KB (623891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2633776e3513bb1431a9e7567b7e9d4bdfa06e8b6238dcaeb5feb610dbdb943`  
		Last Modified: Thu, 09 Feb 2023 04:44:56 GMT  
		Size: 13.4 MB (13415465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e03e21e236202196e670c60b7166ea821beb831f376b3cede06a3f3c5f156`  
		Last Modified: Thu, 09 Feb 2023 04:44:53 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe543d2b0269df754225dec4f30b9ef3754c91967036d98cf6be96c4772993a`  
		Last Modified: Thu, 09 Feb 2023 04:44:55 GMT  
		Size: 3.1 MB (3056228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4eae67e8d9051bcde1798a1b660c77bc426427d84d8064b2f056a5cd9bd0752`  
		Last Modified: Thu, 09 Feb 2023 05:56:28 GMT  
		Size: 6.1 MB (6072613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:72e231a9910e690b6bb4562db3d1b295da3288c148086b7c3150a229fa108d3c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25479903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f562c7c8264c5c4a6449f0fbbb538d6d37ed7bebac3afe9655d26c41a2ef6c86`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:21:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 03:21:17 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 03:21:18 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 03:50:55 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 03:50:56 GMT
ENV PYTHON_VERSION=3.11.2
# Sat, 11 Feb 2023 04:04:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:04:08 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:04:09 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 04:04:09 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 04:04:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:04:09 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:04:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:04:15 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 08:34:47 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 08:34:47 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 08:34:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 08:34:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba2f6867522ee9d2e8dcc9b1ad3ec5bafe75da976a3e613ff26cbc98738b48`  
		Last Modified: Sat, 11 Feb 2023 05:02:08 GMT  
		Size: 624.9 KB (624860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306098e014d097054e21956106f3cc85917ed842396335da9279aaa4a1fa9052`  
		Last Modified: Sat, 11 Feb 2023 05:02:40 GMT  
		Size: 12.5 MB (12460788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0753bae182cbadc488545cafd68cfa7b04db931e00692c69801ce5230184e962`  
		Last Modified: Sat, 11 Feb 2023 05:02:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798db3ecff45d7cb801a130a357cc9a475a13b80674e76a092ccfee1e0c92d5f`  
		Last Modified: Sat, 11 Feb 2023 05:02:39 GMT  
		Size: 3.1 MB (3056458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8536f250f429c06946e40f831cf25e753886f747529bbd04842c080bf27bfa`  
		Last Modified: Sat, 11 Feb 2023 08:40:19 GMT  
		Size: 6.1 MB (6075610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; 386

```console
$ docker pull hylang@sha256:3a8a9c202b745c43359080fa9f399e0732698d044021a6593b95d6bab3340e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25846129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd6eb3e152311f24e99c46b9eade8826dccd52c6db6c534a10bd79ecd917fc8`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:41:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:41:17 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:41:19 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 01:12:50 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 01:12:51 GMT
ENV PYTHON_VERSION=3.11.2
# Sat, 11 Feb 2023 01:25:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 01:25:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 01:25:50 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 01:25:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 01:25:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 01:25:53 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 01:26:01 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 01:26:02 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 05:57:05 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 05:57:05 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 05:57:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 05:57:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d18ebabb6f744ad06852ca1e354e05d3d1db41b0c3e06758dfb23a678e0b88c`  
		Last Modified: Sat, 11 Feb 2023 02:36:23 GMT  
		Size: 623.2 KB (623161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e229903aa95c7994e57982781673c6c4272ef4958c08cdb0cbefdc89d158c3`  
		Last Modified: Sat, 11 Feb 2023 02:37:09 GMT  
		Size: 12.7 MB (12682384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a903c2a8a1341d012e196de33c1e4655bfa155bbaed089530123d54dbe1d245f`  
		Last Modified: Sat, 11 Feb 2023 02:37:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780dd85da1afe3b18d0ea631e62f7aa503aa46a98f58d8555f5be9238d2ca140`  
		Last Modified: Sat, 11 Feb 2023 02:37:07 GMT  
		Size: 3.1 MB (3054216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad250194f2c62d138a0df54d70a6f90ef44c4e7a49ce222216255ce4da23ab4`  
		Last Modified: Sat, 11 Feb 2023 06:07:39 GMT  
		Size: 6.1 MB (6073784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; ppc64le

```console
$ docker pull hylang@sha256:501523b551dcc807ba0a94c94e73dc66df8885b25c85c4b3396b405ed3d5eef2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26007298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9dd4b62f1fca37d2c7c1e92e65cdf4f2b1571e7bec7fcb4501579e8328fddc6`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:43:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:43:03 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:43:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 01:43:58 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 01:43:58 GMT
ENV PYTHON_VERSION=3.11.2
# Sat, 11 Feb 2023 02:10:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 02:10:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 02:10:27 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 02:10:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 02:10:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 02:10:29 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 02:10:40 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 02:10:41 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:34:50 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:34:51 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:35:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:35:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a413709dc452963685d247540895a4124799730691a6ec60fab72353e238035`  
		Last Modified: Sat, 11 Feb 2023 04:19:55 GMT  
		Size: 625.3 KB (625282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a407e700015fae9a57a60d95b2889fa8bc759efe3928b39ca05fb95b9233f2ee`  
		Last Modified: Sat, 11 Feb 2023 04:20:43 GMT  
		Size: 12.9 MB (12858868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9166d6296bf7c08953d9df3cbe88ff84851c53e9c1db366a118d895f04376880`  
		Last Modified: Sat, 11 Feb 2023 04:20:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e1d070dac2b54bd344d062fbe66b072bc16abe8d6dbc29211f77beafece558`  
		Last Modified: Sat, 11 Feb 2023 04:20:41 GMT  
		Size: 3.1 MB (3056537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d886ddf19eca49729765294c1bb1a75d7e76e8efa328cf7e671188f05aa4139`  
		Last Modified: Sat, 11 Feb 2023 12:47:30 GMT  
		Size: 6.1 MB (6075630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:alpine3.17` - linux; s390x

```console
$ docker pull hylang@sha256:e840c2dd31403f8cd7bfea7adb68a426391a61237d0df2f5c4dc09ba3653b6b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25450898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21eb19211fe1da365c5ab4f17f7f1ee7e5a2a5f463cb06c2141ab498b993e89`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:54:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:54:59 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 05:55:01 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 06:27:01 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 06:27:02 GMT
ENV PYTHON_VERSION=3.11.2
# Sat, 11 Feb 2023 06:42:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 06:42:36 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 06:42:37 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 06:42:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 06:42:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 06:42:39 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 06:42:48 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 06:42:50 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:44:01 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:44:01 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:44:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:44:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8eae285bdbe9d3dae44b7168ab47bdfe8ae66951ff84f7eea376d36bf16a99`  
		Last Modified: Sat, 11 Feb 2023 10:44:58 GMT  
		Size: 623.2 KB (623199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e82b9361d090bc7036fa4feb1ef6383ca1c24c2bb555765ad8d2259ee4b003`  
		Last Modified: Sat, 11 Feb 2023 10:45:29 GMT  
		Size: 12.5 MB (12520519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5516bfe02d53a5d30c3c2b803503703eb6a5a12a13981ee7367a660cbb419f83`  
		Last Modified: Sat, 11 Feb 2023 10:45:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c674b6f37394631e9b2b7719c01ad25d165b2a2a2a4363075e7196e620723c`  
		Last Modified: Sat, 11 Feb 2023 10:45:28 GMT  
		Size: 3.1 MB (3056354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59723bb41087ab26825be3c37fb7af27c5907318d7e2b313b5c2bdb18e937ae3`  
		Last Modified: Sat, 11 Feb 2023 12:50:49 GMT  
		Size: 6.1 MB (6075478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
