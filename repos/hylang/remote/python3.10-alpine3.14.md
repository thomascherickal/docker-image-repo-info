## `hylang:python3.10-alpine3.14`

```console
$ docker pull hylang@sha256:320c093b6827907adf0ce768f7bf66e2dba0c40c2fe1c5214bb58b10d5c2626b
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

### `hylang:python3.10-alpine3.14` - linux; amd64

```console
$ docker pull hylang@sha256:09b86519d00e21da02de54bb3b199a9dcb88a3aabfe49dcae4e28373cde6b0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21748472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0491e4f07a7237e7573a4c9394f6d6f8430515682a7002c727b51ef782d0c0e5`
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
# Fri, 18 Mar 2022 15:27:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 24 Mar 2022 23:56:41 GMT
ENV PYTHON_VERSION=3.10.4
# Fri, 25 Mar 2022 00:10:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:10:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:10:18 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:10:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:10:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:10:18 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:10:25 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:10:25 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 01:42:30 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 01:42:30 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 01:42:33 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 01:42:33 GMT
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
	-	`sha256:b6680225b790c9297c59f4e3da0438623527025a0e79162656c8e89c38a739f7`  
		Last Modified: Fri, 25 Mar 2022 00:58:36 GMT  
		Size: 12.3 MB (12275773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f3128d2689716565645beebd11df8f80f11cf0ab753b9b65c02e91f4ba9255`  
		Last Modified: Fri, 25 Mar 2022 00:58:34 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb556506e8c9dca17079ad92a2197e5de6d43c5253f708697480b2fdc3efbcf3`  
		Last Modified: Fri, 25 Mar 2022 00:58:35 GMT  
		Size: 2.9 MB (2871637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbae89aa4c69b5fb2e128ddb8486197b32d3b515f608566f1b521d8cf2acc31e`  
		Last Modified: Fri, 25 Mar 2022 01:46:28 GMT  
		Size: 3.1 MB (3117983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; arm variant v6

```console
$ docker pull hylang@sha256:1b416c8b2b55f7e8d9d3029c15e6acc671a0a3fac9176c4b8e268525faa28920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9a12803ae6d82834d611eb24379353cc811a43e66fd9b7cc38daa7e1fcc86fc`
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
# Tue, 29 Mar 2022 15:14:40 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 29 Mar 2022 16:34:59 GMT
ENV PYTHON_VERSION=3.10.4
# Tue, 29 Mar 2022 17:06:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 17:06:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 17:06:28 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 17:06:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 17:06:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 17:06:29 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 17:06:49 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 17:06:50 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 20:04:28 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 20:04:29 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 20:04:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 20:04:39 GMT
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
	-	`sha256:8dfcc0d6dd2d0656946d8432a97bb3c58ac0163e5d8d19dc70131c13d47f032b`  
		Last Modified: Tue, 29 Mar 2022 18:37:46 GMT  
		Size: 11.9 MB (11887834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5472a61088c7c07840ca1cd23bd32fdfa759c49dad23920ed6b36b8cd7346db`  
		Last Modified: Tue, 29 Mar 2022 18:37:38 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312a6fd17667c4ac9ea9ff01faedda76cacb5c05e510d88543886ccadd802e4`  
		Last Modified: Tue, 29 Mar 2022 18:37:41 GMT  
		Size: 2.9 MB (2871782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33909aaf621a7ac3cb68d209986038bcbedd8f19a35cac7492aba98edd4f53f4`  
		Last Modified: Tue, 29 Mar 2022 20:09:51 GMT  
		Size: 3.1 MB (3118243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; arm variant v7

```console
$ docker pull hylang@sha256:d8256fe09c7636d1968d1f51b2d12c2b90772e9261478d3f33a35148fc77a6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20437941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f50a1c6d2b1187dc94c50b5fd944c53ecb5de2c52aa7f2c8febb4f56879ccd2`
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
# Sat, 19 Mar 2022 11:34:03 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 25 Mar 2022 01:12:46 GMT
ENV PYTHON_VERSION=3.10.4
# Fri, 25 Mar 2022 01:42:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 01:42:04 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 01:42:04 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 01:42:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 01:42:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 01:42:06 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 01:42:22 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 01:42:22 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 05:34:17 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 05:34:17 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 05:34:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 05:34:26 GMT
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
	-	`sha256:9d858b82afbe38a889a054ef21a19676c65089ed4ae19819c94d3c79664acdb2`  
		Last Modified: Fri, 25 Mar 2022 03:45:50 GMT  
		Size: 11.4 MB (11352923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8563287d8de0ee11a4e36faf5090ced60d557969d2583d57f4addd94620eca0`  
		Last Modified: Fri, 25 Mar 2022 03:45:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0473c14f7d7cef8b67c0b344cc0a53aa25e0ffe29a62fb9631ac39198e2d42b`  
		Last Modified: Fri, 25 Mar 2022 03:45:46 GMT  
		Size: 2.9 MB (2871683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bc5dbe8a2aff2f911e6700d4254344895c8ed47565937994e8992b1caa16e5`  
		Last Modified: Fri, 25 Mar 2022 05:42:47 GMT  
		Size: 3.1 MB (3118216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:1fe9d4750680ebac341c8aac0411f399b26df1af3edb0b43569fc95d9cb79d3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.8 MB (21754841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095907dad101a4967f2771cdaabb39c1f84c9b7c234235037aea10c90f451b08`
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
# Fri, 18 Mar 2022 04:27:02 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 25 Mar 2022 00:09:43 GMT
ENV PYTHON_VERSION=3.10.4
# Fri, 25 Mar 2022 00:24:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 00:24:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 00:24:30 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 00:24:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 00:24:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 00:24:33 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 00:24:41 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 00:24:41 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 02:55:46 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 02:55:47 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 02:55:51 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 02:55:52 GMT
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
	-	`sha256:14c6d8eaf6a3b302c148b3119dde8f1acd79c2096461ef9a229f1eed1883b3bf`  
		Last Modified: Fri, 25 Mar 2022 01:02:26 GMT  
		Size: 12.4 MB (12382691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c470a67df08283d747df4a73f285f99fef59558968bab4fbced32098e5b874`  
		Last Modified: Fri, 25 Mar 2022 01:02:24 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4e8e5bb6ceec4fd16c084c98239a223dc692988b9aa166f2f741ba4df7bdf3`  
		Last Modified: Fri, 25 Mar 2022 01:02:25 GMT  
		Size: 2.9 MB (2871487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb232c00102c7c58a76085764261dc509d014099073f4df0156ec1710300906d`  
		Last Modified: Fri, 25 Mar 2022 03:01:19 GMT  
		Size: 3.1 MB (3116266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; 386

```console
$ docker pull hylang@sha256:89abb43820b220a78a3262178a7b4a2df77f2d61ec397baf1c8a1c61afe4c2a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.0 MB (21974298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfa8007a801104cf6b627a2d531b8db31ca2b6f8a0d9d0849c7dac54124740b`
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
# Tue, 29 Mar 2022 06:57:46 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 29 Mar 2022 07:54:31 GMT
ENV PYTHON_VERSION=3.10.4
# Tue, 29 Mar 2022 08:06:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 08:06:25 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 08:06:26 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 08:06:27 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 08:06:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 08:06:29 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 08:06:37 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 08:06:38 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 22:58:30 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 22:58:31 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 22:58:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 22:58:36 GMT
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
	-	`sha256:78486b03fabdcd62cf5041db10a2c26a31170326f96856dd19a57fc183f75a1f`  
		Last Modified: Tue, 29 Mar 2022 09:33:33 GMT  
		Size: 12.5 MB (12490656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc72129e6e8cefebf8a709ab310526309317e6a0f488c7cae40f90200ed90b0f`  
		Last Modified: Tue, 29 Mar 2022 09:33:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2829210d240368400aec6a70e3cc4ea1071359ecd36d0d968d7c0bcd32abdc`  
		Last Modified: Tue, 29 Mar 2022 09:33:32 GMT  
		Size: 2.9 MB (2871497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e1d39a340e4a080009e92d3c1764239ab123aab3004374b611b7ec4935e264`  
		Last Modified: Tue, 29 Mar 2022 23:06:08 GMT  
		Size: 3.1 MB (3116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; ppc64le

```console
$ docker pull hylang@sha256:0a193ed58b10e5b3347a3c603ba2b14134d5cae3e985f595afc3bdd3021f8eec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.1 MB (22062691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7f6b914478b64456e81e10075ba45869af6635f8860a34ae5f96ada543a083d`
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
# Sat, 19 Mar 2022 13:12:22 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 25 Mar 2022 01:48:25 GMT
ENV PYTHON_VERSION=3.10.4
# Fri, 25 Mar 2022 02:10:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 25 Mar 2022 02:10:16 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 25 Mar 2022 02:10:20 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 25 Mar 2022 02:10:22 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 25 Mar 2022 02:10:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 25 Mar 2022 02:10:34 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 25 Mar 2022 02:10:57 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 25 Mar 2022 02:11:01 GMT
CMD ["python3"]
# Fri, 25 Mar 2022 04:50:39 GMT
ENV HY_VERSION=1.0a4
# Fri, 25 Mar 2022 04:50:42 GMT
ENV HYRULE_VERSION=0.1
# Fri, 25 Mar 2022 04:51:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 25 Mar 2022 04:51:07 GMT
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
	-	`sha256:f86c21f411d6f95c33b952d756b6482dcfd01432902e7f527ed2bd9300ec350b`  
		Last Modified: Fri, 25 Mar 2022 03:52:22 GMT  
		Size: 12.6 MB (12578932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a9283eb3650344ce80d806fe04d3c8d916f62e1c899ab1f8e4a75661d4644`  
		Last Modified: Fri, 25 Mar 2022 03:52:20 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940517cfef84e080880baf60c88f21ea491e056f7dcc7b38e9ccce6bdf1e2465`  
		Last Modified: Fri, 25 Mar 2022 03:52:20 GMT  
		Size: 2.9 MB (2871717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003070c630ed508eec874305bc3927b120423f519f89fd8e959e88d393d6a52`  
		Last Modified: Fri, 25 Mar 2022 04:58:31 GMT  
		Size: 3.1 MB (3118113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-alpine3.14` - linux; s390x

```console
$ docker pull hylang@sha256:0a20743bb57beddb19d905f588b671b5ce4bf97676f7fac79d27257e5d3474d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21508291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0448051e6c1875a9f9b8d6e6f080fad1daa856f177d4f4a2e1be4c15543a311c`
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
# Tue, 29 Mar 2022 12:04:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 29 Mar 2022 12:51:35 GMT
ENV PYTHON_VERSION=3.10.4
# Tue, 29 Mar 2022 13:02:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 13:02:46 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 13:02:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 13:02:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 29 Mar 2022 13:02:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 13:02:46 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 13:02:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 13:02:52 GMT
CMD ["python3"]
# Wed, 30 Mar 2022 12:34:21 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 12:34:21 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 12:34:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 12:34:25 GMT
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
	-	`sha256:7ed5238c609aad901180ed5f9faefede18a7348586246e07497938dfd662f729`  
		Last Modified: Tue, 29 Mar 2022 14:30:24 GMT  
		Size: 12.2 MB (12241957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d00ffc1cf1d1df383fa9559e446f690361d595cb0e4e8c931a8a25afdb9b61d`  
		Last Modified: Tue, 29 Mar 2022 14:30:24 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337811109ee9d5ec7d1d6bfd08142a957c3df674bc37fe4319fcd3a9a2b9e919`  
		Last Modified: Tue, 29 Mar 2022 14:30:29 GMT  
		Size: 2.9 MB (2871691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a330d51b932b4a835cb85f33b583fcc47a6303efcb92239f13a50eaaf95d1be1`  
		Last Modified: Wed, 30 Mar 2022 12:40:03 GMT  
		Size: 3.1 MB (3117822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
