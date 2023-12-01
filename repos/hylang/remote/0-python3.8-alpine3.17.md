## `hylang:0-python3.8-alpine3.17`

```console
$ docker pull hylang@sha256:112d19b12e372689124f3fc03daaad3d59ea508af4bd12cdf492261859cba009
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

### `hylang:0-python3.8-alpine3.17` - linux; amd64

```console
$ docker pull hylang@sha256:e70f98dc0a25b552b5ba5aac0cfd4c12e3496401e6e372e39569061856ab7f6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26031467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671bd08273e89fa31c85a45b121d344af28fbaa9a5fce7797e18891b58bbb46a`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:15:27 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_VERSION=3.8.18
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
CMD ["python3"]
# Thu, 19 Oct 2023 09:05:11 GMT
ENV HY_VERSION=0.27.0
# Thu, 19 Oct 2023 09:05:11 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 19 Oct 2023 09:05:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 19 Oct 2023 09:05:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512e36fc6765173e4b462f83c6b68a91d79520aa809e4677ccdb5f484b4573d6`  
		Last Modified: Thu, 19 Oct 2023 06:33:19 GMT  
		Size: 622.5 KB (622458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf6227f2bc321c88066b9abbd38d91f503e56e767977dd69531bc1f908e09d0`  
		Last Modified: Thu, 19 Oct 2023 06:39:25 GMT  
		Size: 15.5 MB (15477925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb148fb3c85d7bade287d9b713675a755ac1e9c637e3a4700b6eca7588cab5`  
		Last Modified: Thu, 19 Oct 2023 06:39:23 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b038584dc4e5f02ca8f28b85a8f5df428c8b8b90ffa8030f882b2b0428b63031`  
		Last Modified: Thu, 19 Oct 2023 06:39:24 GMT  
		Size: 2.9 MB (2851467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0412d41d2f335e26d52a12622b9ee8f79ce6df70e167799d997811bc9bcb5704`  
		Last Modified: Thu, 19 Oct 2023 09:14:07 GMT  
		Size: 3.7 MB (3700768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; arm variant v6

```console
$ docker pull hylang@sha256:5f58044cc1c546c0e07f9140f4ce707703542ab0a02b6c6dcd8bb7fff37554de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25139128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6175fdb81069dc13ec303407315bd16425c93cb07ffb70855c4dea176b706e3`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Wed, 29 Nov 2023 06:26:20 GMT
ENV HY_VERSION=0.27.0
# Wed, 29 Nov 2023 06:26:21 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 29 Nov 2023 06:26:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 29 Nov 2023 06:26:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdc3a4bb2ecfaa095fc7200cf71c3e3053f136295948db01de3c1fc1dd21d2e`  
		Last Modified: Wed, 29 Nov 2023 06:07:44 GMT  
		Size: 624.8 KB (624773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2264efc5925e7a42b1c43203f0c97d4afecad44d627afaf56b947e3f69aeb513`  
		Last Modified: Wed, 29 Nov 2023 06:08:37 GMT  
		Size: 14.8 MB (14848326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f15a4cdaca39a2e6ba29598a6457ecd8f04044d4065d817b5e6868c4b830d4c`  
		Last Modified: Wed, 29 Nov 2023 06:08:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f1c49644acec0f02312428bd8701677f0d86e6ce4ccccd0baa99ff964ee01b`  
		Last Modified: Wed, 29 Nov 2023 06:08:36 GMT  
		Size: 2.9 MB (2851399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de8d97423de9c9b206f3e0b6a4a1f8bef6f6a36f0a47555122bc0668195461`  
		Last Modified: Wed, 29 Nov 2023 06:30:15 GMT  
		Size: 3.7 MB (3701953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; arm variant v7

```console
$ docker pull hylang@sha256:4c0a09f971ecca6b46d1570bf49b3d49dbd292c3984d3d36993f5639bf91fd09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22682598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce517a9f342dffba39bf9e2fe260ff61ff3d5cc83d7bb20e30f035be46a50b30`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:02a6ccbee2a71a547141a8480f3a3912c7bb0934df31124f4a4720204d326698 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:54:13 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:54:13 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:54:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:54:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d4ee79c42f17f258e1c67dc32e0776c934799d208cd0a9b6264f65d60f1a26fc`  
		Last Modified: Thu, 30 Nov 2023 22:50:08 GMT  
		Size: 2.9 MB (2869713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f1360fd2e691e916d990e509541719fb6fccbb47b4a49d758853c2ef805ba`  
		Last Modified: Fri, 01 Dec 2023 02:30:18 GMT  
		Size: 623.8 KB (623783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe677da4e5afc8c4f2a6bb62bc90cadc133dd843745d892a9b85098f0632ca3`  
		Last Modified: Fri, 01 Dec 2023 02:31:30 GMT  
		Size: 12.6 MB (12635126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cab928bb3102f693da0c28ebf4d8838fd37a74262b311b6e73af0e5f44688b1`  
		Last Modified: Fri, 01 Dec 2023 02:31:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80017ea0a869ac1afb86b8be5a4a033f5f94f68bda193180b5242d0a9108e11f`  
		Last Modified: Fri, 01 Dec 2023 02:31:30 GMT  
		Size: 2.9 MB (2851434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a21e08b6a76cc4521e8c12dc5979832b08fd31eb0709b465b980e3f32b83f`  
		Last Modified: Fri, 01 Dec 2023 20:01:35 GMT  
		Size: 3.7 MB (3702314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:7625b8d27df977de88206f6c245fae17ffddc2182770f598d3a7461096e36d94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25771630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f835e6d026db4d9d0edc56892c41455816a94824135134e822ce8be1ca2dd5cf`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:15:27 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_VERSION=3.8.18
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
CMD ["python3"]
# Thu, 19 Oct 2023 07:58:14 GMT
ENV HY_VERSION=0.27.0
# Thu, 19 Oct 2023 07:58:14 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 19 Oct 2023 07:58:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 19 Oct 2023 07:58:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa3157032416a690bdc151c5412520eeb6f77c62d4b493063d96ccffc9a89c`  
		Last Modified: Thu, 19 Oct 2023 07:23:12 GMT  
		Size: 624.4 KB (624437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cdfd57945150b49d684505f60f78e9b7c555fefc9e0f7ba755f3dc47fa4654`  
		Last Modified: Thu, 19 Oct 2023 07:29:03 GMT  
		Size: 15.3 MB (15336733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5436a1c9d27ca6c1a495633c0d69438d4a9ec0c1ca23da96db1e06e27f8d72`  
		Last Modified: Thu, 19 Oct 2023 07:29:01 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ddd225efde8c9e170498d367a55b0727c4060da2d852f0d77fe4919567a9aa`  
		Last Modified: Thu, 19 Oct 2023 07:29:02 GMT  
		Size: 2.9 MB (2851447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b47939f628407a62d5b54f7ef42e3e770929de03b00bbf9f216c27c048c658`  
		Last Modified: Thu, 19 Oct 2023 08:05:47 GMT  
		Size: 3.7 MB (3700483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; 386

```console
$ docker pull hylang@sha256:1fbac3b949155873d030006d460db99605b9f896c0214a403fcbb375ae628c72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.3 MB (26341761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739455da66d6499cc7613b36d7a9ed2cb37d4b50c76813142679b90160204857`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:15:27 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_VERSION=3.8.18
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
CMD ["python3"]
# Thu, 19 Oct 2023 07:44:01 GMT
ENV HY_VERSION=0.27.0
# Thu, 19 Oct 2023 07:44:01 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 19 Oct 2023 07:44:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 19 Oct 2023 07:44:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6983af1d337dbcd10e91f64df5a882f1f5294244b2d713e568708a4745381e8`  
		Last Modified: Thu, 19 Oct 2023 07:10:59 GMT  
		Size: 622.8 KB (622799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032aa2d3713c38e5e0577e5d488db47bee2201f1fc8715db174193b068e2e921`  
		Last Modified: Thu, 19 Oct 2023 07:17:28 GMT  
		Size: 15.8 MB (15752773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acfa2bd44dd3b5d67b9a83e180d50b736fc9a0b3b3931745bf395fec899693f`  
		Last Modified: Thu, 19 Oct 2023 07:17:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9699e718b9d208ac82cec2f1f5b487d17224546942eae416c4f3eb3837a00cdd`  
		Last Modified: Thu, 19 Oct 2023 07:17:25 GMT  
		Size: 2.9 MB (2851473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a47bca5aa0544c7f9efe62e4d7331cc038e2590b30c37aeab81b00f2bed535`  
		Last Modified: Thu, 19 Oct 2023 07:51:57 GMT  
		Size: 3.7 MB (3700697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; ppc64le

```console
$ docker pull hylang@sha256:5f3c2eff308eb01d6f23a3d1d9581ebf07caaaff2cd089f7ff00f396148082ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26361931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ab5f7bcadc6561b59140c3b20690acf9c9bed062764738931dbf479e992126`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:15:27 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_VERSION=3.8.18
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
CMD ["python3"]
# Thu, 19 Oct 2023 07:48:53 GMT
ENV HY_VERSION=0.27.0
# Thu, 19 Oct 2023 07:48:54 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 19 Oct 2023 07:49:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 19 Oct 2023 07:49:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912a5b65c8f67ac1f419fc4bdd0bffaf9c3dcf6af91ec0b82646ad4bcaabfeeb`  
		Last Modified: Thu, 19 Oct 2023 06:57:35 GMT  
		Size: 624.8 KB (624822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa304c49b0ab63337f03ec48679afdd8055f0be43d5b6f9e09a8862194317c6b`  
		Last Modified: Thu, 19 Oct 2023 07:04:20 GMT  
		Size: 15.8 MB (15793222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec286a76a6fec7ef567d9910e09ce3209767a4ef167c492b744a89ef1778970`  
		Last Modified: Thu, 19 Oct 2023 07:04:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c05158e082044cfe3d76ae7df6555c8d8c0051fa34f4781a4b85e3bbdd47874`  
		Last Modified: Thu, 19 Oct 2023 07:04:19 GMT  
		Size: 2.9 MB (2851466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ab654e957c0b6dabcb21b1c6fe5867b8b0d6d68f66918798ef7be742885dc`  
		Last Modified: Thu, 19 Oct 2023 07:57:04 GMT  
		Size: 3.7 MB (3700829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-alpine3.17` - linux; s390x

```console
$ docker pull hylang@sha256:ca8f1916a52b306aabf9965132275cb6d828f7efce989c375f3a1ee55ba5b3e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25627531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772769785b8fa8740de6dc8e73662106fa55c246cae42a8a4c9394bf2f3168f7`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:15:27 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_VERSION=3.8.18
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:15:27 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:15:27 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:15:27 GMT
CMD ["python3"]
# Thu, 19 Oct 2023 06:59:20 GMT
ENV HY_VERSION=0.27.0
# Thu, 19 Oct 2023 06:59:21 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 19 Oct 2023 06:59:33 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 19 Oct 2023 06:59:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafb531e653257ad976a95622521f7b264a6cfcd7d181b7e509658dcf29c7bad`  
		Last Modified: Thu, 19 Oct 2023 06:21:38 GMT  
		Size: 622.7 KB (622742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c9051d2013c1ffcd280f5860ad5a0d9c7e549279b5d50b3e90713ebd6d9047`  
		Last Modified: Thu, 19 Oct 2023 06:25:54 GMT  
		Size: 15.3 MB (15276975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b9433eda73028f07619a794af1217b273a955205e89b5a409b6a7e535f308`  
		Last Modified: Thu, 19 Oct 2023 06:25:52 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f16b98ccde3e94fcbfdf56c138fdd8bbbfb7b5e9bfa4784b7b38e044287322d`  
		Last Modified: Thu, 19 Oct 2023 06:25:53 GMT  
		Size: 2.9 MB (2851325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baaf3d2391019e7ac2b4e4f0334b2d9a2ccb713202ee15fcefabefcfc7063e1`  
		Last Modified: Thu, 19 Oct 2023 07:04:42 GMT  
		Size: 3.7 MB (3700273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
