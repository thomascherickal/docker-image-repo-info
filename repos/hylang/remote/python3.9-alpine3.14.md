## `hylang:python3.9-alpine3.14`

```console
$ docker pull hylang@sha256:1684d56fb97e1574b72b6cbc91656cf6b8f8a2edf790b2a65053bcc06a80d4d0
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

### `hylang:python3.9-alpine3.14` - linux; amd64

```console
$ docker pull hylang@sha256:4c0b86e1c310a2ace6976c3ad6538b65cfc926bf7a2bf4335f9c22b5f23e8a6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21350520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fe96fc64f14dbc848cc09693e4b7c5024d16cd58adadadb7d458ba9ceb8fa4`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 15:27:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 15:27:36 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 15:27:37 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 18 Mar 2022 16:55:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 00:48:32 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 00:54:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:54:31 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:54:31 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:54:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:54:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:54:31 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:54:39 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:54:39 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 01:42:56 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 01:42:56 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 01:42:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 01:42:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe6f338a463b42c8e60c869cee7dbd81d60c1c8361204c25427c28bb4cfef1`  
		Last Modified: Fri, 18 Mar 2022 17:59:39 GMT  
		Size: 666.7 KB (666677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48f6951f0f9c30313c07215285ef42268ce00a291f098ff460e1a7e41cfa1a4`  
		Last Modified: Fri, 25 Mar 2022 00:59:59 GMT  
		Size: 12.1 MB (12079547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fe78d3805ef3c9f3da85aeafd52999ac3d050ff6ba3f1092d5cfac4f71998e`  
		Last Modified: Fri, 25 Mar 2022 00:59:57 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6434deb4616243c773a442f462adbf74da2e4bbc348bcf49cc1f8600dd1afff9`  
		Last Modified: Fri, 25 Mar 2022 00:59:58 GMT  
		Size: 2.9 MB (2871647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f96ee89e7e600a8db3e7658007130a274a8b1a7f20a4b5a3a15a6173e15d0f2`  
		Last Modified: Fri, 25 Mar 2022 01:47:23 GMT  
		Size: 2.9 MB (2916248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; arm variant v6

```console
$ docker pull hylang@sha256:c172927f42b6f118db90b6a544ddbff90ebb63a3abfabfd6a3cf43faca8a70fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20723494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e383ee6124a5b7d69926d68f2b1e31d03a8e62a0682dee535e0a20a7f16bcec`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:14:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 15:14:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:14:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 17:19:35 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 17:19:35 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 17:31:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 17:31:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 17:31:33 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 17:31:33 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 17:31:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 17:31:34 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 17:31:54 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 17:31:54 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 20:05:16 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 20:05:16 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 20:05:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 20:05:26 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e4187cbdf033a13195933b602650fa47d8d303341c38a6a91f8e42ca3b58e1`  
		Last Modified: Tue, 29 Mar 2022 18:36:38 GMT  
		Size: 672.5 KB (672502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a855079353a52b4119295cc15c891fa5cfb55b6d06aa4344218140e9c4d39f`  
		Last Modified: Tue, 29 Mar 2022 18:38:38 GMT  
		Size: 11.6 MB (11636427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3fb205ec7a2ff31661d34c359552affda1fdc0826bad324f52b99f4843f4b1`  
		Last Modified: Tue, 29 Mar 2022 18:38:31 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13358e3b754edd04697c4e1c26a34871a0912a4fcbd7a6be652c7c582f30b9ec`  
		Last Modified: Tue, 29 Mar 2022 18:38:34 GMT  
		Size: 2.9 MB (2871752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc0f83672127d988873502af30c8bb59f21bf0af20fa70c319ca30e09839adc`  
		Last Modified: Tue, 29 Mar 2022 20:10:35 GMT  
		Size: 2.9 MB (2916561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; arm variant v7

```console
$ docker pull hylang@sha256:a71f02849981789a1f85c794a378651eb5bc5c5344542db3955bbb32d2570a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (20023970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374e7075fd3c41255f25a4fcabd90fd972742ad1466b047f99403e3f05cbe248`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 11:33:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 11:33:59 GMT
ENV LANG=C.UTF-8
# Sat, 19 Mar 2022 11:34:02 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 19 Mar 2022 14:40:13 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 03:22:06 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 03:32:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 03:32:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 03:32:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 03:32:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 03:32:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 03:32:54 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 03:33:11 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 03:33:12 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 05:35:46 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 05:35:47 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 05:35:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 05:35:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d839284ee3314935fb29c42acdccb927fbf5f879c8ce17c6369974dd32fe71a`  
		Last Modified: Sat, 19 Mar 2022 16:49:52 GMT  
		Size: 664.4 KB (664427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faab28f385a9100e73ff7b52e3c476e7e0c05a40842326e6b42957c7d62109f`  
		Last Modified: Fri, 25 Mar 2022 03:48:14 GMT  
		Size: 11.1 MB (11140408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1ab19d90c8cbc83a28eca14c756fd1133656183e42d1970e84a61f7b8d52c`  
		Last Modified: Fri, 25 Mar 2022 03:48:07 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254ed2e31f5dad86ba5f229848800c9b6cbe7505427d4f83fad4e7c09ba3bef4`  
		Last Modified: Fri, 25 Mar 2022 03:48:10 GMT  
		Size: 2.9 MB (2871777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc464ec31a6b6941fd2c53d39c7f493faae4ce223d9f15164b4445d6560d5b6f`  
		Last Modified: Fri, 25 Mar 2022 05:44:01 GMT  
		Size: 2.9 MB (2916661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d982998a03502ad64f2529a14852b68e59dc3bb1abcb4876a53f87e68017905c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21316974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2783b7c54bc6c29c548ccc433bd7710aba0f0fef2690ae017faf5ef6e4384b79`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 04:26:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 04:26:59 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 04:27:01 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 18 Mar 2022 05:48:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 00:51:51 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 00:56:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:56:31 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:56:32 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:56:33 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:56:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:56:35 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:56:43 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:56:43 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 02:56:31 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 02:56:32 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 02:56:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 02:56:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212d96083e235548e3ae17e997f58425427cdaccc78363a1c71f874ec79ddd4d`  
		Last Modified: Fri, 18 Mar 2022 06:42:03 GMT  
		Size: 668.3 KB (668277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f917a446ac6ceeabd04f167963187f4e734aeb73a6d94b69c6dddb5bac2b6d9d`  
		Last Modified: Fri, 25 Mar 2022 01:04:06 GMT  
		Size: 12.1 MB (12146365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbf7e9d89923feebbb3413ce54f5c5e1d9d79d448f779796a6070fbc3000ad2`  
		Last Modified: Fri, 25 Mar 2022 01:04:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7019aeffcd4d8b6ca96ffabc19971262ec3d98bc554e7cc3d831f5a2b5ce4d`  
		Last Modified: Fri, 25 Mar 2022 01:04:05 GMT  
		Size: 2.9 MB (2871478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3e1f3cec28cf0348013448655bfbbd88d826b57c06f95eb4862e6184af5cb`  
		Last Modified: Fri, 25 Mar 2022 03:02:23 GMT  
		Size: 2.9 MB (2914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; 386

```console
$ docker pull hylang@sha256:8111756050dd8dedec178e991a3591f16a835b86b33dd1316fedfed5953d9cf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21550397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92215d3c742fc6d3ce0279f5e5364636ba8a241008ce9d2a348e6c61ca286ad0`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:57:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 06:57:43 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 06:57:45 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 08:27:15 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 08:27:16 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 08:32:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 08:32:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 08:32:18 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 08:32:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 08:32:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 08:32:21 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 08:32:30 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 08:32:31 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 22:59:18 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 22:59:18 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 22:59:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 22:59:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df808929e022bc82e56c7c612aaf4129d2af6e04f67b6c734ec7b32f0f9e598a`  
		Last Modified: Tue, 29 Mar 2022 09:31:55 GMT  
		Size: 674.6 KB (674570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba012e5dbe0f2d330fa85d9606ea8a6cf99e40cf10fd68973ca2c8bcbfcd0b`  
		Last Modified: Tue, 29 Mar 2022 09:34:43 GMT  
		Size: 12.3 MB (12268223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ae5f7d99c67f456aa1a4c7e31583e60f2ddc347ef18f4a2cd53d785598bb28`  
		Last Modified: Tue, 29 Mar 2022 09:34:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a971891b06cfa497e59bf6f03ef7f894ef45a71f255f78a266aa19386983ee`  
		Last Modified: Tue, 29 Mar 2022 09:34:42 GMT  
		Size: 2.9 MB (2871517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28c43bbcf2d1cd8706cf87ac0e1d1684e859ed19bb7c6b2ce7d17ddd36ade52`  
		Last Modified: Tue, 29 Mar 2022 23:07:11 GMT  
		Size: 2.9 MB (2914789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; ppc64le

```console
$ docker pull hylang@sha256:e340689dd3d2f28f3f414e6503547fe3e058f3ced8ae8a9190e87a97f4703179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21665042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a12e854afeac4704858fccaf39fcd27ffd22d259e1ee2b315f9f296e8250297`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 13:12:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 13:12:12 GMT
ENV LANG=C.UTF-8
# Sat, 19 Mar 2022 13:12:20 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 19 Mar 2022 15:09:48 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 25 Mar 2022 03:35:11 GMT
ENV PYTHON_VERSION=3.9.12
# Fri, 25 Mar 2022 03:44:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 03:44:19 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 03:44:21 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 03:44:25 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 03:44:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 03:44:32 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 03:44:56 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 03:45:01 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 04:53:39 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 04:53:46 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 04:54:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 04:54:19 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e6a863c7656e70ade52d4774499f0e542c35668757116413d21206b072a942`  
		Last Modified: Sat, 19 Mar 2022 16:34:33 GMT  
		Size: 676.4 KB (676412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565be7384c8ddf248fb55f10daafcf440cbbded6dcc15c471a9a0e4a21acf7cf`  
		Last Modified: Fri, 25 Mar 2022 03:54:17 GMT  
		Size: 12.4 MB (12382839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106ecb0bca8a71a913d434a240acc55792f01b85dd85247d95c36513001bc69f`  
		Last Modified: Fri, 25 Mar 2022 03:54:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3447fd872c0711e1059cee05d95fe1f4492317e58b80c694099c74207798c84`  
		Last Modified: Fri, 25 Mar 2022 03:54:16 GMT  
		Size: 2.9 MB (2871698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84f6bdd5ecd00fcab62bf48080aadcd0577ec5309e26c95ddc4d721b6dc0cc8`  
		Last Modified: Fri, 25 Mar 2022 04:59:55 GMT  
		Size: 2.9 MB (2916579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-alpine3.14` - linux; s390x

```console
$ docker pull hylang@sha256:75ae775b74a478a567b0658d008717104f44879cb87f935bf862fa435cb91f09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21120916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb2785dc8f9170f3b2a9685c798f03d4d61d4c91a21b95c157100acd41bd915`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:04:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 12:04:11 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 12:04:12 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 29 Mar 2022 13:19:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 29 Mar 2022 13:19:59 GMT
ENV PYTHON_VERSION=3.9.12
# Tue, 29 Mar 2022 13:24:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 13:24:48 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 13:24:48 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 13:24:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 13:24:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 13:24:49 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 13:24:56 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 13:24:56 GMT
CMD ["python3"]
# Wed, 30 Mar 2022 12:35:04 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 12:35:04 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 12:35:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 12:35:09 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403c68e18e921f9feaa216298865985f4e74a43fe1a3be64b610d34ff0da0b5a`  
		Last Modified: Tue, 29 Mar 2022 14:19:32 GMT  
		Size: 672.5 KB (672494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81a083d5ab7b7a5666d7cb0a030cb1f0805bdd99940cc99ee3a79eea707212`  
		Last Modified: Tue, 29 Mar 2022 14:38:35 GMT  
		Size: 12.1 MB (12056053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75677dc9a64f144275a469236f6b98475d532bb8c632cf2eac83f61d8d05cc6`  
		Last Modified: Tue, 29 Mar 2022 14:38:35 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ebbb245a3b07acf998931760402591e5d6d5b87a94a02b319302ec89328fb6`  
		Last Modified: Tue, 29 Mar 2022 14:38:35 GMT  
		Size: 2.9 MB (2871761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df0b484c67c86f86f4a106a0995979603692d7c747f4bad9b4ada9423ff60f4`  
		Last Modified: Wed, 30 Mar 2022 12:40:38 GMT  
		Size: 2.9 MB (2916278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
