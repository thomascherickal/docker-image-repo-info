## `hylang:python3.8-alpine`

```console
$ docker pull hylang@sha256:fe97e8e40514e6c7f09230adb3aca5e4013abfac021e5403e8cafc2b8d47abb6
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
$ docker pull hylang@sha256:6b90cbf71e7f63ccafb56431374f723dd9c53919bc200574c787bec5690deb70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.9 MB (21905403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305f7eafe3c23c502f555bf8d06bd999c0d8d64b23fdcef4f363c045e8817d59`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:35:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 01:33:42 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 01:33:43 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 07 Oct 2022 02:34:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 14 Oct 2022 00:40:34 GMT
ENV PYTHON_VERSION=3.8.15
# Fri, 14 Oct 2022 00:44:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 14 Oct 2022 00:45:00 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 14 Oct 2022 00:45:00 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 14 Oct 2022 00:45:00 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 01:02:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 01:02:05 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 01:02:12 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 01:02:12 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:35:26 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:35:26 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:35:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:35:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47858aee13bf9c7c2b62cfaccdc9ce2524efef339df0c0ed8935c6587a376d60`  
		Last Modified: Fri, 07 Oct 2022 03:10:01 GMT  
		Size: 673.2 KB (673188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d75fc19f119d842e1df4b5ce622841d1df39120927fb251ffe00da24c02572`  
		Last Modified: Fri, 14 Oct 2022 00:55:41 GMT  
		Size: 11.8 MB (11761839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c19eb2e4aa754811974b4addcfc9be3f163e97a3d73b1b3ebb7db29565a874`  
		Last Modified: Fri, 14 Oct 2022 00:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce46bf71d46b9cc3ee2acad01e61ee8b7a872ddde7016608688faf412f604a0`  
		Last Modified: Tue, 25 Oct 2022 01:10:12 GMT  
		Size: 2.9 MB (2885804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41ec9da09b0ab052ddea8e62e55698408f0d425e18b628622cce4427e9e8b83`  
		Last Modified: Wed, 09 Nov 2022 00:49:18 GMT  
		Size: 3.8 MB (3778288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm variant v6

```console
$ docker pull hylang@sha256:78cc73d6cf73ee9d5eee8c574fae8fbe96372f5b45f8044f81bcf1992fedc1a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21252003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e2d980d5a80132d395de480315d45facafd82cf7cf65b656a76b02481204285`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:13:11 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:13:12 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 25 Oct 2022 04:40:28 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 04:53:56 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 05:00:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 25 Oct 2022 05:00:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 05:00:05 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 05:00:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 05:00:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 05:00:05 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 05:00:12 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 05:00:12 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 01:09:14 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 01:09:15 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 01:09:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 01:09:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8109934ad0ecb55a616ebe9b507495a756689c8b0d54d1ae718260d2cfe5`  
		Last Modified: Tue, 25 Oct 2022 05:26:37 GMT  
		Size: 677.3 KB (677314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b36c0e2576133a644a7694cda75b32062667a3e1c57ff98f31d26cce33298`  
		Last Modified: Tue, 25 Oct 2022 05:28:45 GMT  
		Size: 11.3 MB (11298378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb9dcafbad51bf410fb2b5a9a7124c83dd8d215b8834c4f985e373c8f6bae24`  
		Last Modified: Tue, 25 Oct 2022 05:28:42 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7327c2da80c8cfc242646ddfdda45e5e4265b6aab63c1420c21feffb408258b5`  
		Last Modified: Tue, 25 Oct 2022 05:28:43 GMT  
		Size: 2.9 MB (2885620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f411dbeb955b8d101c98604632a50c295857180572f7631702998ddbbaa4ab2`  
		Last Modified: Wed, 09 Nov 2022 01:17:58 GMT  
		Size: 3.8 MB (3776495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm variant v7

```console
$ docker pull hylang@sha256:c1f8deb2b60675d5177a68057d3167b48c859c0dd15f098c033af310e9432508
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91ed25501f1f51101c1618aab2dd99d70bf701b5048dd0518d069d088d7e52b`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 05:18:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 05:18:15 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 05:18:16 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 25 Oct 2022 08:16:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 09:02:13 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 09:08:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 25 Oct 2022 09:08:23 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 09:08:23 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 09:08:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 09:08:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 09:08:23 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 09:08:29 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 09:08:30 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:11:25 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:11:25 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:11:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:11:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb59b4321d1a11fe77ce73b05c0eacb9c7523a4726a77acc99613022244a0671`  
		Last Modified: Tue, 25 Oct 2022 10:14:00 GMT  
		Size: 670.3 KB (670273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54263c65ef5e00c6f5e80eaff5232ae5c35e903805c97a2fd87d4e5ad94102af`  
		Last Modified: Tue, 25 Oct 2022 10:19:39 GMT  
		Size: 10.8 MB (10827834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d92e127d0ef0e25b06e72ce9e7af3411c39b788aa6a2d550e997540e6438bf3`  
		Last Modified: Tue, 25 Oct 2022 10:19:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20432f5634b9c6049293ec28997760cfa94600689e214a6a9059238bdb59f2c`  
		Last Modified: Tue, 25 Oct 2022 10:19:37 GMT  
		Size: 2.9 MB (2885640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f903af2b794454db8db3329a98f8de454dff105ed7fb620af691b1f085c8543`  
		Last Modified: Wed, 09 Nov 2022 03:26:55 GMT  
		Size: 3.8 MB (3776509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:03020b47637125ee4eedb7c3839229622c38c68cbeaa91a8c69217356c351846
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.8 MB (21831987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af91b2fac43df512e90ece8e4348a27546b5cc832b3605f76797d78e4e1e23dc`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:43:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 01:43:19 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 01:43:19 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 25 Oct 2022 03:37:23 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 04:03:25 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 04:06:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 25 Oct 2022 04:06:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 04:06:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 04:06:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 04:06:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 04:06:52 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 04:06:57 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 04:06:57 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:56:23 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:56:23 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:56:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:56:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6633159d7b96f4da53636e263dc14779ebe40e93e3237ceab5ef6c5f6285b`  
		Last Modified: Tue, 25 Oct 2022 04:50:47 GMT  
		Size: 673.9 KB (673939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4a2a3325e2efe4d9014207d8eb03250d25275a8d73e71272f74d7a3ca0d6`  
		Last Modified: Tue, 25 Oct 2022 04:54:54 GMT  
		Size: 11.8 MB (11786069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127d46fae82215768610f3d95558a78d9cfb5d830a833c6b5828b1b2bde9474`  
		Last Modified: Tue, 25 Oct 2022 04:54:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225cd9edda422e041e38dfb50584adcc41a8c59c22100a95f983816b7657e335`  
		Last Modified: Tue, 25 Oct 2022 04:54:53 GMT  
		Size: 2.9 MB (2885817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defee6a06310b0643d256fd757df264d00ae459290d40964d0c50be99d08b083`  
		Last Modified: Wed, 09 Nov 2022 01:09:42 GMT  
		Size: 3.8 MB (3778272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; 386

```console
$ docker pull hylang@sha256:1cbb5ee1dc0728b9bb0f68c2594094a04b65a075f7f6d0b5f5c6423fbd564dfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.1 MB (22062920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0e296f2d9ad576c41cd0ea22865d8a8c424f84b080782b34f767d5ea35be99`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:27:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 23:27:31 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 23:27:33 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 07 Oct 2022 00:34:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 14 Oct 2022 01:14:51 GMT
ENV PYTHON_VERSION=3.8.15
# Fri, 14 Oct 2022 01:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 14 Oct 2022 01:20:08 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 14 Oct 2022 01:20:09 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 14 Oct 2022 01:20:10 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 02:00:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 02:00:25 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 02:00:33 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 02:00:34 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:50:02 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:50:03 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:50:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:50:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea141995d554d7b4181165068a4e8417a838580fd74919feb331359beb7cabf`  
		Last Modified: Fri, 07 Oct 2022 01:17:54 GMT  
		Size: 680.2 KB (680219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17e9094e8137285b00d3779300f0a94bda3ca4263b641ff6110a7f6b7dd0bc1`  
		Last Modified: Fri, 14 Oct 2022 01:34:29 GMT  
		Size: 11.9 MB (11912857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e051c9be6feef0da57bde2006a9d3204f6da233ec528ea7b4a393f9393b575c1`  
		Last Modified: Fri, 14 Oct 2022 01:34:27 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0d1495bf6ebd25b017a4ddbb7fecfca1be2b1a4694a8aafaa7e9a8b36ae7d`  
		Last Modified: Tue, 25 Oct 2022 02:11:57 GMT  
		Size: 2.9 MB (2885684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2167a345b822aa630c19255d3021790d2f02875539e5747a70fbd8d019e0df5e`  
		Last Modified: Wed, 09 Nov 2022 01:09:41 GMT  
		Size: 3.8 MB (3776806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; ppc64le

```console
$ docker pull hylang@sha256:6da808aaa3956dbe5479f7921ceed07217817eb111615645680025e67a096e6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22193278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e787789c2e8843eacf1b2de5a6232935d9ed091f53da144af85ab45ae6a203a`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:58:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 02:58:54 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 02:58:57 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 07 Oct 2022 05:10:48 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 14 Oct 2022 01:42:27 GMT
ENV PYTHON_VERSION=3.8.15
# Fri, 14 Oct 2022 01:50:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 14 Oct 2022 01:50:36 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 14 Oct 2022 01:50:36 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 14 Oct 2022 01:50:37 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 02:19:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 02:19:24 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 02:19:37 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 02:19:37 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:40:57 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:40:57 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:41:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:41:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d112c63e4aad1e5ab498645b305fa598dbf16e8eb4bebcfdf7d60025dd71ac7`  
		Last Modified: Fri, 07 Oct 2022 06:39:54 GMT  
		Size: 682.0 KB (681974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260cf7bcd89d11666ae4c8f2931caa81b4dcda7cfe0f2fae5f72ea2b8f11e7be`  
		Last Modified: Fri, 14 Oct 2022 02:06:04 GMT  
		Size: 12.0 MB (12043527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb799a5c7cd01dc8623b69a1f5c79b18d924f497333e371c573f30a898a826`  
		Last Modified: Fri, 14 Oct 2022 02:06:00 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214a4a883172658653386c2081c9a6f7591d27308bfea2b797fdbe254becc4cb`  
		Last Modified: Tue, 25 Oct 2022 02:28:59 GMT  
		Size: 2.9 MB (2885830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab25a88c4eda6c256bcc0b5c8ea9845fc8d9c6002c914cc70d2d1181839197`  
		Last Modified: Wed, 09 Nov 2022 00:53:55 GMT  
		Size: 3.8 MB (3778393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine` - linux; s390x

```console
$ docker pull hylang@sha256:d7ce52a986bcc511cbed20fbb1cfd73befd751bd4b2e3656484f7a8ccb85b2ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21646939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8016d65e9685aab9156ee1c574b66beedcceb4e0b4183d14055720fd3ecccdaa`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:06:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 04:06:08 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 04:06:11 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 07 Oct 2022 05:25:21 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 13 Oct 2022 23:59:37 GMT
ENV PYTHON_VERSION=3.8.15
# Fri, 14 Oct 2022 00:04:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 14 Oct 2022 00:04:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 14 Oct 2022 00:04:24 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 14 Oct 2022 00:04:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 00:51:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 00:51:27 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 00:51:32 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 00:51:33 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:34:50 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:34:51 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:35:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:35:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0ca99e03dc565a767bfc7a4b927c0748fed621008bcdd93e42dd6fa9feceb`  
		Last Modified: Fri, 07 Oct 2022 08:59:24 GMT  
		Size: 677.5 KB (677495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d60efa7500e38d50a6de8cb16a4e719e50d70a3a5aa4c310bad6032ffc8e52`  
		Last Modified: Fri, 14 Oct 2022 00:15:19 GMT  
		Size: 11.7 MB (11714472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e159c93b8b9b3c591661f0df4d405d83bf11566bccccbd6e0962fef8700eb71`  
		Last Modified: Fri, 14 Oct 2022 00:15:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46435bec9df541482b19c7210ac7a84e38889b9f35b15991c0438da3ecd1cbff`  
		Last Modified: Tue, 25 Oct 2022 00:57:56 GMT  
		Size: 2.9 MB (2885886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edea3251b9727750d066ad3074e1b3c384795275652873e3bc63a79453cb0f3`  
		Last Modified: Wed, 09 Nov 2022 03:43:33 GMT  
		Size: 3.8 MB (3778258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
