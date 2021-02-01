## `python:rc-alpine`

```console
$ docker pull python@sha256:5650e9ad241649e8df7a911a11f780d8774e67159e7e4b75880ae1ab9da676ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `python:rc-alpine` - linux; amd64

```console
$ docker pull python@sha256:700e0ba870f6030d57baf6f1110def412cf3858246b4ec691c216a0b08114470
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17023779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f6276923ba2ca363d359f87f8894ede5941f5105a99a6b05b651f5d606bc72`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:38:23 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:38:26 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 01:38:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 01:50:23 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 02:00:39 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 02:00:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 25 Jan 2021 23:28:37 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:28:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:28:37 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:28:44 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 25 Jan 2021 23:28:44 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8723b2b92bec2587f3d011d9141963ee89d3c8299b013ccc5ad018e4e278f0ba`  
		Last Modified: Thu, 17 Dec 2020 08:39:21 GMT  
		Size: 653.7 KB (653694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f2e43b4c7a890099d19ae43d802f36bfc50fbb08409f47359595a8f7a247d`  
		Last Modified: Tue, 05 Jan 2021 02:04:08 GMT  
		Size: 11.4 MB (11407914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0416c13e403be55fc4b6dc68e0efbf7119b61e210ac335229c857a522096b93b`  
		Last Modified: Tue, 05 Jan 2021 02:04:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ba6eb8287aeb5ded875d14775110ae7e279e0227fcc2c1363c3b0b442a3da`  
		Last Modified: Mon, 25 Jan 2021 23:35:01 GMT  
		Size: 2.2 MB (2162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; arm variant v6

```console
$ docker pull python@sha256:7ab7292a11d2c0605f267e3180e45e7e2105b1e26f3372b6c72a2f5d9d39f4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16462399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50cd47dc2a4e181ec2b1a6a382d5e1e1547041902347fadc32c06ce7e778e27`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:10:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:10:12 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:10:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 06:10:16 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 00:52:36 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 01:02:59 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 01:03:02 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:54:04 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:54:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:54:06 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:54:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:54:26 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f247151884668eaab48d2f4695c029f264af7086834a1254e456f7b2787ced3`  
		Last Modified: Thu, 17 Dec 2020 07:44:25 GMT  
		Size: 657.0 KB (657049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84de3702df16f6f6fb95e5b9708c78e6374f0889afff4c1faff981600ae2bcf4`  
		Last Modified: Tue, 05 Jan 2021 01:04:42 GMT  
		Size: 11.0 MB (11036802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3ae32e2be0a09cd1ffaf6c265662536cedd5164108d0067d8da11f207957a7`  
		Last Modified: Tue, 05 Jan 2021 01:04:38 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f1b8542bc462ee596ba8a4fcca08a339547fac285f49e2f8cb8813f628878`  
		Last Modified: Mon, 01 Feb 2021 21:58:48 GMT  
		Size: 2.2 MB (2164151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; arm variant v7

```console
$ docker pull python@sha256:66ed1f6079d6bd5cf05a0bfbf8a9605a302be9d8dc2750a3ba55ff56985ecd25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15285143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:628d1238e646d6b9cef22288d03c766ad01e99eb1eb83a386ce541901859445d`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:50:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:50:14 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:50:18 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 06:50:19 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 01:25:50 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 01:31:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 01:31:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 22:05:05 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 22:05:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 22:05:06 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 22:05:21 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 22:05:21 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44297260d605b35d45691ba0fe7b4d28e56d0f59ac1acbacc68b73c1d6d0fb4d`  
		Last Modified: Thu, 17 Dec 2020 07:48:21 GMT  
		Size: 650.2 KB (650185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8fc0b8f94592e8954f21dffd0d64b5ba79608d7bf79e8f2fa07c4ead405c1a`  
		Last Modified: Tue, 05 Jan 2021 01:35:15 GMT  
		Size: 10.1 MB (10063125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5a411224c3477c8ae7392e5b1b2d2d866eb6419b06601021277f4fcf0f4649`  
		Last Modified: Tue, 05 Jan 2021 01:35:02 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c47bcf60e8e516407542bf2fa307f9da1d054333f68b6dd3ce6fd78c19c091`  
		Last Modified: Mon, 01 Feb 2021 22:17:55 GMT  
		Size: 2.2 MB (2164045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; arm64 variant v8

```console
$ docker pull python@sha256:e3f085a449e8ab31217201ffc0decae01fe0a79cd3d874e81a9f84fa4e6453e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17017584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c106c30161d66f4c563b3f43201cc93a2b2fe896b6cb553876979d332edf731`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:00:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 07:28:12 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 07:28:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 07:28:16 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 02:04:58 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 02:12:13 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 02:12:15 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 25 Jan 2021 23:58:56 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:58:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:58:58 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:59:16 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 25 Jan 2021 23:59:19 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391216306a83e802e59fe257ff360db71cb4501300ddb74004e1037f681d61a5`  
		Last Modified: Thu, 17 Dec 2020 08:49:11 GMT  
		Size: 656.2 KB (656212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc458505db79e7bf7f8c46c926bb9d49e80fa21661c79f9aa5f375daee4dac86`  
		Last Modified: Tue, 05 Jan 2021 02:16:09 GMT  
		Size: 11.5 MB (11489000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505b478a5040bea1336dd84bfc9591ef638b985074de8e1be5cb2f8761ac9291`  
		Last Modified: Tue, 05 Jan 2021 02:16:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9a6da0e723c085b8bb5e264f1596ff900032fb55ee2322a4f56e8a3b558ee0`  
		Last Modified: Tue, 26 Jan 2021 00:14:19 GMT  
		Size: 2.2 MB (2163094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; 386

```console
$ docker pull python@sha256:0858ece64612da097b00155c4884610adb070e0c1b67b4c55c01e7018178c740
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9941d9dc6a64e5e5ea2c8337715da34c496f9e58be667feed86676c1730ff5`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:08:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 06:08:38 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:08:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 06:08:40 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 02:10:45 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 02:18:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 02:18:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:43:03 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:43:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:43:04 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:43:12 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:43:13 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd8ebc5cea4852e6fcd46241a79b1cfdf47a37821839653681b507e9aca707d`  
		Last Modified: Thu, 17 Dec 2020 07:16:24 GMT  
		Size: 659.4 KB (659424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2debc3ead5cbdb6d1421d21ab10e76c5371d31072c4154bef5770aa96e284bb3`  
		Last Modified: Tue, 05 Jan 2021 02:22:03 GMT  
		Size: 11.6 MB (11643757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9fb753f2f38570894cf7f6419096ebe208ac9afeaf9abd9a1fad5ff3553ad`  
		Last Modified: Tue, 05 Jan 2021 02:21:59 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15831f695bb8edad8fb67eaf74505d02b5ff5be2aecb227977dfb1e2a874fd65`  
		Last Modified: Mon, 01 Feb 2021 21:50:11 GMT  
		Size: 2.2 MB (2163916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; ppc64le

```console
$ docker pull python@sha256:ce0f8d9e0c38440d9f7f075526a9f39e821aedde7b455dd458093a1ceb90be83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17827155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e246a79ab68a1fe743b9011b77c5088f552c5affdf63df5bf534a314b24feb4`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:37:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 09:37:14 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 09:37:21 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 09:37:25 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 01:54:16 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 02:04:17 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 02:04:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 25 Jan 2021 23:23:23 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:23:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:23:32 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:24:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 25 Jan 2021 23:24:12 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ebe329e1e5edf3f0bdf9357f8cd70bfae122f27b9baf5a657eb88a1d99b018`  
		Last Modified: Thu, 17 Dec 2020 11:02:28 GMT  
		Size: 662.3 KB (662267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d0b68612f9091729c8886c0f4fdbd3139c3355458c66a298b79a4fae479ee`  
		Last Modified: Tue, 05 Jan 2021 02:08:57 GMT  
		Size: 12.2 MB (12196292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adef136312722e09e958ef0a8cd85fc57b9ab0433f87d53dac534fa76ae3199f`  
		Last Modified: Tue, 05 Jan 2021 02:08:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8706f273a8257231becf2d551777e69013553317fb4180eb21b31d1497e12`  
		Last Modified: Mon, 25 Jan 2021 23:42:21 GMT  
		Size: 2.2 MB (2163139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-alpine` - linux; s390x

```console
$ docker pull python@sha256:be555ad578c46330ee70046de117faf59ca76e65aaf666f0727243227d226f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16785883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d58bbfef2e0a02c42466600aed3cf0cd05b9a158e7b8a204699b4b45e380f0f`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 08:14:16 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 08:14:19 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Thu, 17 Dec 2020 08:14:20 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 05 Jan 2021 01:59:02 GMT
ENV PYTHON_VERSION=3.10.0a4
# Tue, 05 Jan 2021 02:05:23 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 05 Jan 2021 02:05:25 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 21:47:12 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 21:47:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 21:47:13 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 21:47:22 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 21:47:24 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4172f589a51cb56b09cfa22abe5e09c19c92991a2a33a55a4f220773233311b3`  
		Last Modified: Thu, 17 Dec 2020 09:29:06 GMT  
		Size: 658.8 KB (658752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b118224417e82d2e6a7f3e4e3b90e353e12af24f1cc92f83a752095fccec99`  
		Last Modified: Tue, 05 Jan 2021 02:08:38 GMT  
		Size: 11.4 MB (11395809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55c2c13f244d8c2c9487c3b5ca06284ddc333ac532e29b5ccbda6f551083322`  
		Last Modified: Tue, 05 Jan 2021 02:08:36 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496b3bdd34bd69255f56d13fb41af487035c99958b629ba99da9fcfdcf3c7176`  
		Last Modified: Mon, 01 Feb 2021 21:53:48 GMT  
		Size: 2.2 MB (2164070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
