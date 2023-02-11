## `hylang:0-python3.10-alpine3.16`

```console
$ docker pull hylang@sha256:fd664f7b02abe9d16d86d0e21eb25aa0cfaaef53b67ddc61701230d580bd4fad
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

### `hylang:0-python3.10-alpine3.16` - linux; amd64

```console
$ docker pull hylang@sha256:3c19517f079e8aaf570312f403f3e67d108e10e96f4cafe9ac935fad5d981fc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24810271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76d81fcffb4fdefd26f6f9119d613c9560de07847d4eb50f5cdc8ebdc86faf2d`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:56:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Nov 2022 06:39:07 GMT
ENV LANG=C.UTF-8
# Sat, 12 Nov 2022 06:39:08 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 12 Nov 2022 06:57:28 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 09 Feb 2023 02:11:15 GMT
ENV PYTHON_VERSION=3.10.10
# Thu, 09 Feb 2023 02:20:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Thu, 09 Feb 2023 02:20:42 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 02:20:42 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 09 Feb 2023 02:20:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 09 Feb 2023 02:20:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 02:20:42 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 02:20:49 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 02:20:49 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 02:53:40 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:53:41 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:53:53 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:53:54 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e124a36b9ab9caae9b9b43bffcb6f6d9f126ab89cf2a8b20b9a6f912df03d36`  
		Last Modified: Sat, 12 Nov 2022 07:47:59 GMT  
		Size: 661.8 KB (661831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd71263ccb2dea1d6e07966a253c68d4850ffbddcc4868195354f06efdb3b94`  
		Last Modified: Thu, 09 Feb 2023 02:27:32 GMT  
		Size: 14.2 MB (14165311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08ec9473861e220fec3de6abdbbd30f081fe36db9be02a40e93526a116163d8`  
		Last Modified: Thu, 09 Feb 2023 02:27:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bb172450832d4b682c9b0b9d9ce19023b7e8956900eb23f72d66722701357a`  
		Last Modified: Thu, 09 Feb 2023 02:27:31 GMT  
		Size: 3.1 MB (3056455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dea77eafffc8a2b989d359bab2907d379883b5c8538e42c912f3e480891b56a`  
		Last Modified: Thu, 09 Feb 2023 03:06:06 GMT  
		Size: 4.1 MB (4120174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; arm variant v6

```console
$ docker pull hylang@sha256:d82bb6f12a41cbe8564a3f87adb8a5337b6ff3606d8db7e367fe2d473a0fc86d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22345013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbfd838eec57a4fa9f052d8ae0cf0683b87a8db72d5cb93bad662152b39763a`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 04:01:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 04:01:25 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 04:01:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 04:41:49 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 05:15:55 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 05:28:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 05:28:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 05:28:35 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 05:28:35 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 05:28:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 05:28:35 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 05:28:43 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 05:28:43 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 09:43:32 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 09:43:33 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 09:43:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 09:43:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d5f8dddc5412cb7b693550b369415d99bc8023bb945b77ff8c104d30642a3`  
		Last Modified: Sat, 11 Feb 2023 06:03:58 GMT  
		Size: 666.2 KB (666220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058f331f8dfe8f9fba1e78c71cfc98ad785919b86a25326f2fb97b89ed2f915`  
		Last Modified: Sat, 11 Feb 2023 06:05:27 GMT  
		Size: 11.9 MB (11887639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e9e4344f6f00347001da05ab731c30c4663a916f3fb2e9895ec4f5c3327a3b`  
		Last Modified: Sat, 11 Feb 2023 06:05:24 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee773351bda9a2b567d0dc00b7f1ff0be331072af42859dff4f41a68671a309`  
		Last Modified: Sat, 11 Feb 2023 06:05:25 GMT  
		Size: 3.1 MB (3056226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91283ef822a1f47f1356ff13a3d8d0371458fa53e1a8241b0037a9361a6f9dfe`  
		Last Modified: Sat, 11 Feb 2023 09:52:35 GMT  
		Size: 4.1 MB (4117914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; arm variant v7

```console
$ docker pull hylang@sha256:176a46f0f1e6f7a5868af5758d5fd7d6e8ede721de87b89a86ab821a81e5c67d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21637617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe92e5d48c603e7b414b5c7447f6d0df9693a44fc7a35e098db26d420cdeddcf`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:32:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:32:41 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:32:44 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 03:58:42 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 04:32:36 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 04:45:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:45:16 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:45:16 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 04:45:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 04:45:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:45:16 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:45:23 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:45:23 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:30:38 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:30:38 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:30:51 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:30:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6e694c5ef6bb767ae22254bc320d2da76e3f34ea96b7da5bfc66d08664c4e1`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 659.3 KB (659305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc56bdacf61de0819b3c560f2233ce7376bd3de947921545288614d75610cf3`  
		Last Modified: Sat, 11 Feb 2023 05:23:48 GMT  
		Size: 11.4 MB (11383424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f694a8441c3dc21302ae4a90ff5882b64f50ed152b7b8c6057e2b0d5e33ccc7`  
		Last Modified: Sat, 11 Feb 2023 05:23:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ec9d38ea9c298a97455eb3388fa6745e99aa7da504d7fe9260a603237ca5e3`  
		Last Modified: Sat, 11 Feb 2023 05:23:46 GMT  
		Size: 3.1 MB (3056271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcc937130af99790c35d7f5007a65a520ccc109993b662f9106b3d30cb431dd`  
		Last Modified: Sat, 11 Feb 2023 12:40:55 GMT  
		Size: 4.1 MB (4117893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:6b219aff59c7247afcdb34ad69c9c30828073361c63911e09ccd53bfad7677e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22846400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afba32486eb0cf91ea0a47422b1e4847189599190ae2057d4c36e9f03582a986`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:34:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 03:34:25 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 03:34:26 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 04:04:19 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 04:28:57 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 04:38:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:38:23 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:38:23 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 04:38:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 04:38:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:38:23 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:38:29 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:38:29 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 08:35:31 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 08:35:31 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 08:35:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 08:35:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bfbf2be34530311efb325a41c8edbfd877067f2984a9946627a1b03fd61b58`  
		Last Modified: Sat, 11 Feb 2023 05:02:22 GMT  
		Size: 663.1 KB (663125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5add31ece1ea64838a52f439e1e352c1ebcf9608cd1cf0d33fe4f3c06242163d`  
		Last Modified: Sat, 11 Feb 2023 05:03:33 GMT  
		Size: 12.3 MB (12296859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ce95966609b7811842c5a7df3fbe84a2c4c03d6c9ee04932b7f920c799dc6d`  
		Last Modified: Sat, 11 Feb 2023 05:03:32 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a1ab0e0a7ab13993866c3bcb5a63dc00d3ac0e077cb1426a5a8c9d0653e56f`  
		Last Modified: Sat, 11 Feb 2023 05:03:33 GMT  
		Size: 3.1 MB (3056455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228e8578eefafcccc59d2f5457ed6605608bffa48975ce847843cd48f4ed5e8c`  
		Last Modified: Sat, 11 Feb 2023 08:41:47 GMT  
		Size: 4.1 MB (4120227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; 386

```console
$ docker pull hylang@sha256:bbfb39f07b8f55c2f80ba610ea12185e0f5fa56d41fe5db5b68f14c462f3a15f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23037253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b16c9750fc8361c2e5c7dc8670d2a8cef9ec3a50aa72e7ed713aabc87507ab`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:54:32 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:54:33 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:54:35 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 01:26:21 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 01:52:54 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 02:03:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 02:03:25 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 02:03:26 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 02:03:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 02:03:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 02:03:29 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 02:03:37 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 02:03:37 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 05:58:23 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 05:58:24 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 05:58:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 05:58:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f175ea2d81a85c3a34aa65fa7a6223798ad43a8d9645ec186c31d12f13a7df9b`  
		Last Modified: Sat, 11 Feb 2023 02:36:41 GMT  
		Size: 669.6 KB (669630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c81ea6d63b8b3aa5549999efb13a97e228d7a9bbd827267cac3fac6457005`  
		Last Modified: Sat, 11 Feb 2023 02:38:18 GMT  
		Size: 12.4 MB (12384888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e933a24e1b819804d7370273779a17b01f592d4fd7dcc2efa0cf1b9bd5b1dcf`  
		Last Modified: Sat, 11 Feb 2023 02:38:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bf0510d94aa8012928e7ab47c12b52b4340e2be3425ffc896e607e6c676be9`  
		Last Modified: Sat, 11 Feb 2023 02:38:17 GMT  
		Size: 3.1 MB (3054215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876c68366522ccc6f877416f73ec39995cf2d9b5bed7a9487e69b000042fa64`  
		Last Modified: Sat, 11 Feb 2023 06:09:31 GMT  
		Size: 4.1 MB (4117639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; ppc64le

```console
$ docker pull hylang@sha256:f39424a90e6f112f322f65fe37fce278acdd4b8cb7adfee083ab0ec746564ede
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23128447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76286a96b7a7667f55711b019241691a3fdf10398559d39de961a58bc719e58`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 01:09:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 01:09:03 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 01:09:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 02:10:59 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 03:03:23 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 03:24:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 03:24:10 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 03:24:11 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 03:24:11 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 03:24:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 03:24:12 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 03:24:24 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 03:24:24 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:36:42 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:36:43 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:37:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:37:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a86f30c4238772b9bbdc0285d11cbe1774498512ad8bafccaedcbf67132251`  
		Last Modified: Sat, 11 Feb 2023 04:20:17 GMT  
		Size: 670.3 KB (670300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f0c14f4916c758a64c4e8230e61bc433b135a74980ec57f6c707d8e8bc2724`  
		Last Modified: Sat, 11 Feb 2023 04:22:01 GMT  
		Size: 12.5 MB (12476666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fcb41ca7f0eabee4f0e24f1834ff80467aa3693d681d1a4cbf34466157b05d`  
		Last Modified: Sat, 11 Feb 2023 04:21:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d8a0df472a66c467005d03bdc2f383f15e282c203247411cc820544f2a7a1e`  
		Last Modified: Sat, 11 Feb 2023 04:21:59 GMT  
		Size: 3.1 MB (3056339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2b84e8e231f568de025fadb23b5a2256246458cdb5b7722027b3403a330468`  
		Last Modified: Sat, 11 Feb 2023 12:49:51 GMT  
		Size: 4.1 MB (4120283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-alpine3.16` - linux; s390x

```console
$ docker pull hylang@sha256:ce6e5a8c2a2d2087f2def581ff893bf7fd089af59f1da4cd4956daf110e2279d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22659672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8e5154026729bcf8fa0f2a3ffbd487fe790e9c377d756f52b3fc08fbdfb41c6`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:07:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 06:07:33 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 06:07:34 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 06:43:00 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 11 Feb 2023 07:13:32 GMT
ENV PYTHON_VERSION=3.10.10
# Sat, 11 Feb 2023 07:22:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 07:22:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 07:22:55 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Sat, 11 Feb 2023 07:22:55 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 11 Feb 2023 07:22:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 07:22:56 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 07:23:01 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 07:23:02 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:45:00 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:45:00 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:45:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:45:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adb0ada542e535816922b2b2d2d4ff2af513d5807aef216c21245e5a6dc576d`  
		Last Modified: Sat, 11 Feb 2023 10:45:10 GMT  
		Size: 666.7 KB (666653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fe06a3305f7e1feaf8cfd997cd0ff4bd6e5d858e9aba7c905c715201d28145`  
		Last Modified: Sat, 11 Feb 2023 10:46:15 GMT  
		Size: 12.2 MB (12222468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034644d0aef17084d01a814aa4c7d28d2a879d6a250d8409236627b975955734`  
		Last Modified: Sat, 11 Feb 2023 10:46:14 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c6c4046e2e67c6bfd712ba2e335a9720786815e9e008205d0475b3e291cca`  
		Last Modified: Sat, 11 Feb 2023 10:46:14 GMT  
		Size: 3.1 MB (3056509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b98210dc64df6f895b4e33d396859c81ceba7c69e68f77eb13b451039ea3198`  
		Last Modified: Sat, 11 Feb 2023 12:51:57 GMT  
		Size: 4.1 MB (4120232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
