## `python:3-alpine`

```console
$ docker pull python@sha256:5fa8a404fc45999c2deab0c20182cf4571c4c67c1a243798ad219f8ff9c56460
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

### `python:3-alpine` - linux; amd64

```console
$ docker pull python@sha256:fd7789d5bc7b8a18f729ff3d9f9af9182b2ac8a705538aec8fd7793065666bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17523480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e97c0a01945a5c177ebfd189c8493511e48b1dadde962fd967270f2c43325a4`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:00:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:43:53 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 02:06:05 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 25 Nov 2020 02:28:12 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 08 Dec 2020 01:39:22 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 08 Dec 2020 01:48:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 08 Dec 2020 01:48:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Dec 2020 01:48:46 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Tue, 08 Dec 2020 01:48:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Tue, 08 Dec 2020 01:48:46 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Tue, 08 Dec 2020 01:48:54 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Dec 2020 01:48:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fc4dd5c37b5e49f8cc5610fc6283f49e6fd6315093319ea9ac4c9b78f4977a`  
		Last Modified: Wed, 25 Nov 2020 04:25:36 GMT  
		Size: 653.7 KB (653690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89c49ab00bcef10b0554492952f77357624129a54fc0631b015cb5f8744dc47`  
		Last Modified: Tue, 08 Dec 2020 01:51:11 GMT  
		Size: 11.9 MB (11936944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5234de9d6ef0196f19e614a38ce6b851eba13d527f902ee479f01b72e926f67`  
		Last Modified: Tue, 08 Dec 2020 01:51:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a917f113e96efd71d3f2473e274244b51c64aac0e03c519035c72c068246733a`  
		Last Modified: Tue, 08 Dec 2020 01:51:09 GMT  
		Size: 2.1 MB (2135757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; arm variant v6

```console
$ docker pull python@sha256:99c028bae462e9fca638d3772868b10193e8d08156f1f6817880fdf72fadfe19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16596821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38e80e6890cfde658864515a8f5a7be8b4d5e17e0912beb938756cad0d1ba0c`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:45:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:45:05 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 05:45:08 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 11 Dec 2020 05:56:24 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 05:56:26 GMT
ENV PYTHON_VERSION=3.9.1
# Fri, 11 Dec 2020 06:06:28 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 06:06:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 06:06:34 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 06:06:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 06:06:39 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 06:06:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 06:06:56 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533d64ad160b7b6f5bf3aaea33eeeea65233912580091d5bd37f177c13feb059`  
		Last Modified: Fri, 11 Dec 2020 06:48:21 GMT  
		Size: 657.0 KB (657049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5075d5de0154e60c0ce930f7fb4c635dd44efe792a2ca01264918522c87bdbf5`  
		Last Modified: Fri, 11 Dec 2020 06:48:40 GMT  
		Size: 11.2 MB (11201435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a86a92ce2c69212f8222d35c230434b9314f984579d5ac1d16d022cc530b146`  
		Last Modified: Fri, 11 Dec 2020 06:48:37 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f75bc7715eb746fdbb57d00fde20f14c24f3fe4aa57540c4936a4f9f6115d`  
		Last Modified: Fri, 11 Dec 2020 06:48:38 GMT  
		Size: 2.1 MB (2136112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; arm variant v7

```console
$ docker pull python@sha256:c7fb5d431d71667ecf8f461b3723abceb6bbe24f5f3bd5f2260997535e5fe5a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15448573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1737d8d182b7488c67ee272db2c558a24169a92f8f4aaa8add65e7052679e90`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 12:16:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:16:46 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:16:50 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 11 Dec 2020 12:38:21 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 12:38:22 GMT
ENV PYTHON_VERSION=3.9.1
# Fri, 11 Dec 2020 12:43:52 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 12:43:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 12:43:58 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 12:43:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 12:44:00 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 12:44:17 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 12:44:32 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e0f829ee57e990e8671964520414ee5acf960b3583a4c2e846cf91f553af91`  
		Last Modified: Fri, 11 Dec 2020 14:20:04 GMT  
		Size: 650.2 KB (650184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136b56f2b6c7d5bfe13cc29c23161818b381988c17cd0b863412e5abf4c81fa`  
		Last Modified: Fri, 11 Dec 2020 14:20:54 GMT  
		Size: 10.3 MB (10256182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc08902480f99adaed3699fff25fa3c0fa01b168073b94292ed726981d4f8a7`  
		Last Modified: Fri, 11 Dec 2020 14:20:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace64a25ec323588b25fd8f7265b27c254e8a8c361f851846951c3f585bd1839`  
		Last Modified: Fri, 11 Dec 2020 14:20:52 GMT  
		Size: 2.1 MB (2136284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; arm64 variant v8

```console
$ docker pull python@sha256:de48f64d8b87adb4ec277def9da00f676c757fd072bfdc82101bb7287b193235
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17137334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7b57cf89db3952bc566fee53b623b70663dbb8b6dc773404f09fce7c9a3890`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:50:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:23:16 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:23:21 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Fri, 11 Dec 2020 12:44:08 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 12:44:13 GMT
ENV PYTHON_VERSION=3.9.1
# Fri, 11 Dec 2020 12:52:06 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 11 Dec 2020 12:52:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 12:52:14 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 12:52:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 12:52:17 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 12:52:46 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 12:52:57 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb438ec7b95b7ee8e27a504092d41c1c8f8384912f978b02dc0a9cb71cb9237`  
		Last Modified: Fri, 11 Dec 2020 14:30:44 GMT  
		Size: 656.2 KB (656226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccceba05c47431c63d411dee72fdfe7026fe51134d0c0e1892443aa031c7a1d`  
		Last Modified: Fri, 11 Dec 2020 14:31:29 GMT  
		Size: 11.6 MB (11637970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d9aa89786a5153b724b4bbb27bc3cd4214fe8065bb704897cc7e48e622e140`  
		Last Modified: Fri, 11 Dec 2020 14:31:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc122e0dae15d5b4cb19e4e364154c287b9edbe2af6297595d2843b14343584`  
		Last Modified: Fri, 11 Dec 2020 14:31:27 GMT  
		Size: 2.1 MB (2136289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; 386

```console
$ docker pull python@sha256:c2ce66c6127b7a75c2548deb61ffa5683bee7a43e73b21814d0433768f4fd61e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17748644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13272665994a6a6f005faf567a7c08d4d86d53fd961240a484b1ad535cbb8825`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:59:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:59:41 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 02:21:57 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 25 Nov 2020 02:50:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 08 Dec 2020 02:08:16 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 08 Dec 2020 02:16:31 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 08 Dec 2020 02:16:31 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Dec 2020 02:16:32 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Tue, 08 Dec 2020 02:16:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Tue, 08 Dec 2020 02:16:32 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Tue, 08 Dec 2020 02:16:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Dec 2020 02:16:40 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2166c584b6d790928515565958449b833182fa73aeb548deb328e78e23737a`  
		Last Modified: Wed, 25 Nov 2020 05:08:03 GMT  
		Size: 659.4 KB (659383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98dd3a1397a975484bbebf90c8032ecf69a02f88e05b55aa465b79fa0df476`  
		Last Modified: Tue, 08 Dec 2020 02:19:05 GMT  
		Size: 12.2 MB (12161735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a114fc2477eb22d593ff788c04fab0358d7c6639afc6f8a301503acbe33a8fb6`  
		Last Modified: Tue, 08 Dec 2020 02:19:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72e2e03f8f7d05291fad3d4d8491da8069095e4c7ae8427c1008cd273426b3a`  
		Last Modified: Tue, 08 Dec 2020 02:19:03 GMT  
		Size: 2.1 MB (2135890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; ppc64le

```console
$ docker pull python@sha256:c0a052fafb0e93671b99c56150750ba748b48292219515c29d220231dc2834a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18318910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0cb40f47112786e1aafc038714945741d3cf6d016806dc5746719541bb049f`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 21:26:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 21:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 05:52:25 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 25 Nov 2020 06:32:08 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 08 Dec 2020 02:15:40 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 08 Dec 2020 02:24:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 08 Dec 2020 02:25:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Dec 2020 02:25:11 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Tue, 08 Dec 2020 02:25:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Tue, 08 Dec 2020 02:25:22 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Tue, 08 Dec 2020 02:25:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Dec 2020 02:25:56 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b84add859cee32c152b6e6dcabfc5aa6e14e9562e8e2b28c1364ef5f9b3066`  
		Last Modified: Wed, 25 Nov 2020 09:25:23 GMT  
		Size: 662.3 KB (662251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa1bf8466da4e85db2b1e462c30cd6c2430952e892f38b36debc1011c46f533`  
		Last Modified: Tue, 08 Dec 2020 02:29:27 GMT  
		Size: 12.7 MB (12717135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9d773497715d8db25344e6ce4b568caccbd28f91b07331dd0a114dd2c65c8`  
		Last Modified: Tue, 08 Dec 2020 02:29:25 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de9727b9c59b9d8e53fbeedb5cc745778e343e718ecab71ca37c461ea53ae6`  
		Last Modified: Tue, 08 Dec 2020 02:29:25 GMT  
		Size: 2.1 MB (2136074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-alpine` - linux; s390x

```console
$ docker pull python@sha256:ff470acd3819990e0597934ad2b2c6fa39594e796e4459d1c8047b79f25596ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17311258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ad8c4eedcbcb01f3830fa6ab88d892f46c50f4b8d3681631679f2049d0929f`
-	Default Command: `["python3"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:33:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:33:16 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 06:34:17 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 25 Nov 2020 06:52:25 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 08 Dec 2020 01:57:59 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 08 Dec 2020 02:04:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 08 Dec 2020 02:04:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Dec 2020 02:04:05 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Tue, 08 Dec 2020 02:04:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Tue, 08 Dec 2020 02:04:07 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Tue, 08 Dec 2020 02:04:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Dec 2020 02:04:14 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc428e8baea8b0fa138732b8606238e317966ebe63a2e5173651bc5ea176a081`  
		Last Modified: Wed, 25 Nov 2020 11:21:07 GMT  
		Size: 658.8 KB (658771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73da606f907008b5a50e78caa5fec37e3e23ca4f22874d3a5eb8732641198be`  
		Last Modified: Tue, 08 Dec 2020 02:06:44 GMT  
		Size: 12.0 MB (11950445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007953fa2dc3b2d18bc16d48c45c144efb4c7c288ce07a99ff86c94ed811d62`  
		Last Modified: Tue, 08 Dec 2020 02:06:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7fae0fc985ee4ee6e2122d49dc95f71cd24f768477e7c2a31666b7d7fa4cfd`  
		Last Modified: Tue, 08 Dec 2020 02:06:42 GMT  
		Size: 2.1 MB (2135983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
