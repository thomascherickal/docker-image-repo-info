## `hylang:python3.8-alpine3.14`

```console
$ docker pull hylang@sha256:77c65d59f1d201c7bb20144324b8c4e3bf4bec8bf3d6a597ee528c21e9136a41
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

### `hylang:python3.8-alpine3.14` - linux; amd64

```console
$ docker pull hylang@sha256:d6373ddc915acd5d1298802886d031bacd4222a1cebd0bb4b54871f81605f0cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21126616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef71f355105a4f65b51f6c70064eb939898e5d4d534c274171dd8b214d787d2`
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
# Fri, 18 Mar 2022 17:22:51 GMT
ENV PYTHON_VERSION=3.8.13
# Fri, 18 Mar 2022 17:29:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 18 Mar 2022 17:29:56 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 18 Mar 2022 17:29:56 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 18 Mar 2022 17:29:57 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 18 Mar 2022 17:29:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 18 Mar 2022 17:29:57 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 18 Mar 2022 17:30:09 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 18 Mar 2022 17:30:09 GMT
CMD ["python3"]
# Fri, 18 Mar 2022 22:21:25 GMT
ENV HY_VERSION=1.0a4
# Fri, 18 Mar 2022 22:21:25 GMT
ENV HYRULE_VERSION=0.1
# Fri, 18 Mar 2022 22:21:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 18 Mar 2022 22:21:29 GMT
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
	-	`sha256:e2407fb2ba7ebbc6f5c26198c41383bd9709acd0f3278ab86e25e8d5a688208f`  
		Last Modified: Fri, 18 Mar 2022 18:02:23 GMT  
		Size: 11.8 MB (11833636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b6c92ad448fca0f0d09b4cb819a77528ee663db6caf3fd05c5a33b5daa067`  
		Last Modified: Fri, 18 Mar 2022 18:02:21 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0389a326a22c02fcb9d8dc2e372d9348630127ba0f175a0ef88efa56a37e4c63`  
		Last Modified: Fri, 18 Mar 2022 18:02:22 GMT  
		Size: 2.9 MB (2874005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058939accc9d9e331f23903a40a1ec25faac9a93fdedb52d2498694e37c0830`  
		Last Modified: Fri, 18 Mar 2022 22:24:37 GMT  
		Size: 2.9 MB (2935895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm variant v6

```console
$ docker pull hylang@sha256:26eefdc377db0e448865015baf1313154fddf6a6cfe76e619b261a573289efd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.5 MB (20522710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b0262dba7eb5f666149a5be05b249265f202bc25a4f27f7954c232daeb4c3b`
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
# Tue, 29 Mar 2022 17:43:48 GMT
ENV PYTHON_VERSION=3.8.13
# Tue, 29 Mar 2022 17:54:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 17:54:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 17:54:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 17:54:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 29 Mar 2022 17:54:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 17:54:54 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 17:55:10 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 17:55:11 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 20:06:01 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 20:06:01 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 20:06:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 20:06:10 GMT
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
	-	`sha256:7bba95bed30f9adaddd9771df86211160d7fc23dea20bafadea486537f89b366`  
		Last Modified: Tue, 29 Mar 2022 18:39:21 GMT  
		Size: 11.4 MB (11413789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272c696052903b27a3b3c574175312e50329b9ee8f0b5f7d3bc220167b130fe`  
		Last Modified: Tue, 29 Mar 2022 18:39:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badf8bd024ab25522dc14c0769cb89c0663094c566f61b7f315599e48ab23f58`  
		Last Modified: Tue, 29 Mar 2022 18:39:18 GMT  
		Size: 2.9 MB (2874002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f4485fe0aeba06755618a83164862a08579004ba9d5cced0f025dc56d80d09`  
		Last Modified: Tue, 29 Mar 2022 20:11:11 GMT  
		Size: 2.9 MB (2936167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm variant v7

```console
$ docker pull hylang@sha256:3f8d89f96e0e2b364e88f1e2b4909706b68be94e1b15f85a0586ed8bd61fa25c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19838057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cedb64a686475b8d143d5caf16e55e7bac330b89f423cf081dfe3e6ed5184b1`
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
# Sat, 19 Mar 2022 15:30:01 GMT
ENV PYTHON_VERSION=3.8.13
# Sat, 19 Mar 2022 15:39:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 19 Mar 2022 15:39:58 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 19 Mar 2022 15:39:58 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 19 Mar 2022 15:39:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 19 Mar 2022 15:39:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Sat, 19 Mar 2022 15:40:00 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Sat, 19 Mar 2022 15:40:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 19 Mar 2022 15:40:15 GMT
CMD ["python3"]
# Sat, 19 Mar 2022 17:01:25 GMT
ENV HY_VERSION=1.0a4
# Sat, 19 Mar 2022 17:01:26 GMT
ENV HYRULE_VERSION=0.1
# Sat, 19 Mar 2022 17:01:33 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 19 Mar 2022 17:01:34 GMT
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
	-	`sha256:fb9bca863643cf9b51c7521630b8fc346be3c1eac7dbf97b855834436337a2bd`  
		Last Modified: Sat, 19 Mar 2022 16:54:34 GMT  
		Size: 10.9 MB (10932610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910a6a8ae7473bdb9ad192d5bfff18248b4cdf9791fd9d656d2397d70cb4b56`  
		Last Modified: Sat, 19 Mar 2022 16:54:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59333191d00013a4533305c7a4731b0b47f6a55f75542a76c5fb7423a3fa71f`  
		Last Modified: Sat, 19 Mar 2022 16:54:30 GMT  
		Size: 2.9 MB (2874106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5068fbe969502692c16f92df8b1f9a51a1915023be4f26b76542efa4821ce84a`  
		Last Modified: Sat, 19 Mar 2022 17:07:47 GMT  
		Size: 2.9 MB (2936222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d6559bd41b3f0a6556521ca2d989b43d4eada4bf0cd387374eae66f5472822e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21084064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed713cdb6f5c91149c296240a9a8124d7435a0bbfb5b29c9a5003be4a420d06`
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
# Fri, 18 Mar 2022 06:03:52 GMT
ENV PYTHON_VERSION=3.8.13
# Fri, 18 Mar 2022 06:08:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Fri, 18 Mar 2022 06:08:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Fri, 18 Mar 2022 06:08:18 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 18 Mar 2022 06:08:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 18 Mar 2022 06:08:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Fri, 18 Mar 2022 06:08:21 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Fri, 18 Mar 2022 06:08:28 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 18 Mar 2022 06:08:29 GMT
CMD ["python3"]
# Fri, 18 Mar 2022 06:48:39 GMT
ENV HY_VERSION=1.0a4
# Fri, 18 Mar 2022 06:48:40 GMT
ENV HYRULE_VERSION=0.1
# Fri, 18 Mar 2022 06:48:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 18 Mar 2022 06:48:44 GMT
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
	-	`sha256:fb0d5a90ce4f2d10d2229b329471e51172c51f4fb07345928a2695bde9de2b9b`  
		Last Modified: Fri, 18 Mar 2022 06:45:16 GMT  
		Size: 11.9 MB (11890082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f69f9b89d53e8226a9ea30bd791048bd489f71437b0d8aa148fb5d83d4daf10`  
		Last Modified: Fri, 18 Mar 2022 06:45:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82b6f2f061b4a852b722d102a6b2f0f38f01c81c452b58264847db05328c045`  
		Last Modified: Fri, 18 Mar 2022 06:45:15 GMT  
		Size: 2.9 MB (2873445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea03f4f8b4131ca855c840346dd09a869f0001fcc020ed9af51c1b8b0d528b91`  
		Last Modified: Fri, 18 Mar 2022 06:54:13 GMT  
		Size: 2.9 MB (2936139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; 386

```console
$ docker pull hylang@sha256:90a3f4b2dba86732e7712e03dc90230cfa92ef0aa8dfc401744a8fc4d3be7b07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.3 MB (21325456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62278c24bc77c81d3935961160a5bf88efefbf482681778e083e1563331f05a7`
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
# Tue, 29 Mar 2022 08:51:31 GMT
ENV PYTHON_VERSION=3.8.13
# Tue, 29 Mar 2022 08:56:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 08:56:10 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 08:56:11 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 08:56:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 29 Mar 2022 08:56:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 08:56:14 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 08:56:22 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 08:56:22 GMT
CMD ["python3"]
# Tue, 29 Mar 2022 23:00:04 GMT
ENV HY_VERSION=1.0a4
# Tue, 29 Mar 2022 23:00:04 GMT
ENV HYRULE_VERSION=0.1
# Tue, 29 Mar 2022 23:00:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 29 Mar 2022 23:00:09 GMT
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
	-	`sha256:ae458cd86a79a226589734c81382254568593e94423b7181038f49925d577af1`  
		Last Modified: Tue, 29 Mar 2022 09:35:48 GMT  
		Size: 12.0 MB (12019778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8413cceb0a3475b760f552492eefc6996910abfa29d36f57cfec97695875e`  
		Last Modified: Tue, 29 Mar 2022 09:35:46 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9672ba0e859b3dd3c43e6360fbab75de8fc0b7da1d37081ac31f13b3955e2`  
		Last Modified: Tue, 29 Mar 2022 09:35:47 GMT  
		Size: 2.9 MB (2873544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab609cc8289e5e3ae3c3b290936316364efa2bb356964355f24065626865933`  
		Last Modified: Tue, 29 Mar 2022 23:08:06 GMT  
		Size: 2.9 MB (2936266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; ppc64le

```console
$ docker pull hylang@sha256:406a9b56c4e8d390fdd9b86222c8db54ea854b6997288baf81c23c813c3d9279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21434202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9d9bc391faf431d3d140b0c0b6425bbf7910f5c4670afcc59dc100ae74736b`
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
# Sat, 19 Mar 2022 15:40:26 GMT
ENV PYTHON_VERSION=3.8.13
# Sat, 19 Mar 2022 15:48:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 19 Mar 2022 15:48:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 19 Mar 2022 15:49:01 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 19 Mar 2022 15:49:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 19 Mar 2022 15:49:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Sat, 19 Mar 2022 15:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Sat, 19 Mar 2022 15:49:23 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 19 Mar 2022 15:49:26 GMT
CMD ["python3"]
# Sat, 19 Mar 2022 16:45:04 GMT
ENV HY_VERSION=1.0a4
# Sat, 19 Mar 2022 16:45:07 GMT
ENV HYRULE_VERSION=0.1
# Sat, 19 Mar 2022 16:45:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 19 Mar 2022 16:45:23 GMT
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
	-	`sha256:ce8167fcaf905d024cb742420a25be1f7e893f0b356379731d3394d3cacc72f3`  
		Last Modified: Sat, 19 Mar 2022 16:39:41 GMT  
		Size: 12.1 MB (12130046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7805a5b4fe4ce73633ed4c341c3e7f8eafe82a46a673ebe72b2c00722d0ef5`  
		Last Modified: Sat, 19 Mar 2022 16:39:39 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0646eb28256b117e81ffc61477f51f61b941b3fc6638dfb5ec96765d9ad45308`  
		Last Modified: Sat, 19 Mar 2022 16:39:40 GMT  
		Size: 2.9 MB (2874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83ddb140babc886612d9c654e982f549eaaa99a73f8d8ad30993a85c4eff7c6`  
		Last Modified: Sat, 19 Mar 2022 16:49:38 GMT  
		Size: 2.9 MB (2936186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-alpine3.14` - linux; s390x

```console
$ docker pull hylang@sha256:d6e109182542ea242ce49974d9b9f4075d986b2d29bfb818bd303e30ec935feb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.9 MB (20900819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97fdd371210fc560de0dc6153ebf06281902be5dcbf74f09416767910b68096`
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
# Tue, 29 Mar 2022 13:40:26 GMT
ENV PYTHON_VERSION=3.8.13
# Tue, 29 Mar 2022 13:44:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 29 Mar 2022 13:44:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 29 Mar 2022 13:44:49 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 29 Mar 2022 13:44:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 29 Mar 2022 13:44:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Tue, 29 Mar 2022 13:44:49 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Tue, 29 Mar 2022 13:44:55 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 29 Mar 2022 13:44:55 GMT
CMD ["python3"]
# Wed, 30 Mar 2022 12:35:46 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 12:35:46 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 12:35:49 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 12:35:50 GMT
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
	-	`sha256:dfe2636d3ffff14f31816700046a7208e50a62f17f5c24d88ba9c11ac3a9eb1e`  
		Last Modified: Tue, 29 Mar 2022 14:45:53 GMT  
		Size: 11.8 MB (11814176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197ddfea5c1e23bc1be26548409ccd4cb6152e0ca09543fe5d0a7ecee19e03cf`  
		Last Modified: Tue, 29 Mar 2022 14:45:53 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd93e0f22c202100c7fbd13102aec43678b99df17cb910a5033da626cbbf6a3`  
		Last Modified: Tue, 29 Mar 2022 14:45:53 GMT  
		Size: 2.9 MB (2874000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b9a3e1e3dd024423b5b2e8f6a59a167079cb26ca5a2f76b96cdb0fb318650`  
		Last Modified: Wed, 30 Mar 2022 12:41:10 GMT  
		Size: 2.9 MB (2935822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
