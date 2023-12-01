## `python:3-alpine3.17`

```console
$ docker pull python@sha256:d168b8be48725ffd7749239bd1b4575c16ff81a30a317bf36224f7f74bb9b160
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `python:3-alpine3.17` - linux; amd64

```console
$ docker pull python@sha256:30c381c3a0dcd20215c433cd35378dde11c0a07a3e656139be7e886f30ff5e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18277611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14ea96ddd53cfcc0907a7cabfa0d29f73d1597c436eb6fcb4ebe95219931627`
-	Default Command: `["python3"]`

```dockerfile
# Sat, 21 Oct 2023 18:46:15 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3c7bc1de87416dec0f281eccd0b87cdc6eaf1b885647bab3db0d695d6a783f3`  
		Last Modified: Fri, 01 Dec 2023 02:41:47 GMT  
		Size: 622.6 KB (622587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18dfb1d5a53f5f356135a3ad3365fdedd9c301a56b4d4053309cfe7805b610b7`  
		Last Modified: Fri, 01 Dec 2023 02:42:07 GMT  
		Size: 11.6 MB (11599454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:813fee53afe112e078071735ce3cfe4f1ccae92662ba3b612bab7edc4f031c0f`  
		Last Modified: Fri, 01 Dec 2023 02:42:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc33fb833569f915f5e8dbb03b860c2dfca68cc9c8ca546e6f1e5fc0676068ac`  
		Last Modified: Fri, 01 Dec 2023 02:42:06 GMT  
		Size: 2.7 MB (2676017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:2cf48a084d7f3cf1b9bf56ce30d19413a33f63cac6adab942ef12a26fbfaa557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **877.0 KB (876980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3055b7cdf7c2220269e7331d6bbc6f28133fd8195ce5b44c8d38a8f4410a29d`

```dockerfile
```

-	Layers:
	-	`sha256:6a63bdae1637c620e8f4a0d4ccb927b4812bc431ed7cab33f5724d5215f30c28`  
		Last Modified: Fri, 01 Dec 2023 02:42:06 GMT  
		Size: 853.9 KB (853859 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1576caf7f940883a5af6b5446effe9cafcd28fc8caa75d2a02ff07e2992e0232`  
		Last Modified: Fri, 01 Dec 2023 02:42:05 GMT  
		Size: 23.1 KB (23121 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; arm variant v6

```console
$ docker pull python@sha256:82ca98db86494e64a1ead00fbe2589b1878002c4a65bb9615c962ebf8ebef181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda04f8d4fbc68e8a28ead2b9456dffd5141dcdd820b60787720812e9837583d`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccdc3a4bb2ecfaa095fc7200cf71c3e3053f136295948db01de3c1fc1dd21d2e`  
		Last Modified: Wed, 29 Nov 2023 06:07:44 GMT  
		Size: 624.8 KB (624773 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49d295fad078426557718c63b36d3c9f29d46ccf4b405a7a48269deade4ee893`  
		Last Modified: Wed, 29 Nov 2023 06:07:59 GMT  
		Size: 13.0 MB (13035703 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:329bb7a6026483e336b82a054d0bccd6a0c207d7d329824eef2804f8638ba1f8`  
		Last Modified: Wed, 29 Nov 2023 06:07:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5493569bb5c6a8be288dbd9faed90c928f5d74565e73cae8bbc718f367821`  
		Last Modified: Wed, 29 Nov 2023 06:07:59 GMT  
		Size: 2.7 MB (2675996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:0b89706b58e63176d886f7217ebed95aef32b80e1fb621be5bdb727452bd595b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **879.6 KB (879553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcf7eedbf6e27e43abe15d3bd5cca33cecc67f4291c23503a35e00cf9b5273de`

```dockerfile
```

-	Layers:
	-	`sha256:cdb2f8546cde20037e141790d86ddb166bf9fd1ffd8e4e0705065e3b426c4567`  
		Last Modified: Wed, 29 Nov 2023 06:07:59 GMT  
		Size: 856.3 KB (856345 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:80e4b5897c7337f68105ceab5d58ecbc638813b1c08de7b33cb331f96e8e4f59`  
		Last Modified: Wed, 29 Nov 2023 06:07:58 GMT  
		Size: 23.2 KB (23208 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; arm variant v7

```console
$ docker pull python@sha256:155d63c9e3011a744921a5b1235cb10d7f1f8ae11c585cf7ff63c6fafece5962
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16958635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e02a4a973697878b12238aac2d588b71405fe0e61acb2df4b634e554bf2bcea`
-	Default Command: `["python3"]`

```dockerfile
# Sat, 21 Oct 2023 18:46:15 GMT
ADD file:02a6ccbee2a71a547141a8480f3a3912c7bb0934df31124f4a4720204d326698 in / 
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d4ee79c42f17f258e1c67dc32e0776c934799d208cd0a9b6264f65d60f1a26fc`  
		Last Modified: Thu, 30 Nov 2023 22:50:08 GMT  
		Size: 2.9 MB (2869713 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:150f1360fd2e691e916d990e509541719fb6fccbb47b4a49d758853c2ef805ba`  
		Last Modified: Fri, 01 Dec 2023 02:30:18 GMT  
		Size: 623.8 KB (623783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4491f38243462ac36ac69ed46e9983f3f07466f81e992003f0f0e29355cd02b`  
		Last Modified: Fri, 01 Dec 2023 02:30:37 GMT  
		Size: 10.8 MB (10788901 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2adcca3230703d7c98a0583a04cf3e8a735a34cac93040f78d1e01175a4df38b`  
		Last Modified: Fri, 01 Dec 2023 02:30:36 GMT  
		Size: 229.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5168a683e2078c18a6a1cf2516653649dfd2e43dcce151bef3f960e9d3d0b3bd`  
		Last Modified: Fri, 01 Dec 2023 02:30:36 GMT  
		Size: 2.7 MB (2676009 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:c2de3ffa0fba0d127b7300ac3815af3813a365dd1d91292ab2d12b76d797d08d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **879.6 KB (879553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff0b43ce49d37001d853895cb27bd90b7cb76c18c2dbb6d99af4409fa3009f1`

```dockerfile
```

-	Layers:
	-	`sha256:162635d7f5dba739cf540da719cb80fc014c6e79362e4c23c63943ccb07aca4b`  
		Last Modified: Fri, 01 Dec 2023 02:30:36 GMT  
		Size: 856.3 KB (856345 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb97835b34f5ce37f540ebc2f1e4f72f64a5d7d12a72c459ca2d784d02dc8a3b`  
		Last Modified: Fri, 01 Dec 2023 02:30:36 GMT  
		Size: 23.2 KB (23208 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull python@sha256:1eefec142e876ab0f0cc2b4ddd7938a404a9eca426493e2fc7fbfaec48a6c37a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20160096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461328f2c9c983f0dc73c3eb0431bdbcc9a6f41133d259a658004c3ee7fd8dcc`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:908ffe9cdedf78821f28c2912c9cb38bad6606802eecf25875c1c2cc261791e1`  
		Last Modified: Wed, 29 Nov 2023 05:41:34 GMT  
		Size: 624.6 KB (624648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8c2f2ee6326e227d4e71235801432ee792bff440b23aef74cba4f2d2a822c9b`  
		Last Modified: Wed, 29 Nov 2023 05:42:16 GMT  
		Size: 13.6 MB (13600928 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b4ab21d9d77c513468c701d9a39a638aeacc6ae21aca55b256037860b0b2d21`  
		Last Modified: Wed, 29 Nov 2023 05:42:14 GMT  
		Size: 230.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a5f4afdaa79875da51c366850f802e3c81074db6fe9520f95f1602146ed64d8`  
		Last Modified: Wed, 29 Nov 2023 05:42:14 GMT  
		Size: 2.7 MB (2676000 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:2c6d07262536b7c921f05bd2e95cf2cdfc97ef07e798c30d4d8a6ab2b6b87fbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **877.0 KB (876981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8761046a89aa976a04e1abe9e411bc4192adbad6dc88c691456e4cba45d9876`

```dockerfile
```

-	Layers:
	-	`sha256:d995376fa08b8c27dd223b1acadb6f250585a30a20db1d6bd5264584c3127e8f`  
		Last Modified: Thu, 30 Nov 2023 23:26:10 GMT  
		Size: 853.9 KB (853860 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:827596d930c77559e42d87e6813c97745edc748321656dfb5068f818986a1336`  
		Last Modified: Thu, 30 Nov 2023 23:26:09 GMT  
		Size: 23.1 KB (23121 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; 386

```console
$ docker pull python@sha256:5a89d02694f2f65afa1b21b6491a1f8b1deceda155baa336bc3c165318394afc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20705567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1fb5c53ed545b54cfce884227a2ede2a644843f43d15ebbbef1f8c455157a44`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a62e7a1361b0ce8437f27ccab59ef90aebfd5e71bb11015540a7a3407e5761cd`  
		Last Modified: Wed, 29 Nov 2023 10:17:58 GMT  
		Size: 623.0 KB (622964 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01aeb5c6a8a87de8c430e32eac61cc6d9b5247cb73d179c97962da7f2a87b592`  
		Last Modified: Wed, 29 Nov 2023 10:18:40 GMT  
		Size: 14.0 MB (13992587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dde8de0fb8677b3a22ebd542215e5ed07867b1c64782c41875bd18bba87e1eda`  
		Last Modified: Wed, 29 Nov 2023 10:18:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e00da6d98c5c2397109e512ee02155edbd8da5f05e3f455221a8d984989ac6a`  
		Last Modified: Wed, 29 Nov 2023 10:18:40 GMT  
		Size: 2.7 MB (2676009 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:1f9e6530119127ab244f1e7cd102284129afabfd3c6bf35cbdbdfbe1fbfd9341
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **876.9 KB (876942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de9dd844afafd1e6f0385fde59d0e29062e5d638021377f9f207a66cf63d748`

```dockerfile
```

-	Layers:
	-	`sha256:ad337e3f71ec75484915fc0d0169c0c8b316f00fad974f3e1343969cfc181ed7`  
		Last Modified: Wed, 29 Nov 2023 10:18:40 GMT  
		Size: 853.8 KB (853847 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:58c5373b2ba633ce7c58f6ee918b37ff55832178d904ac50333aa25df2d912d2`  
		Last Modified: Wed, 29 Nov 2023 10:18:39 GMT  
		Size: 23.1 KB (23095 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; ppc64le

```console
$ docker pull python@sha256:3ea04b6fbc5dcb897f4a3b1034626dda9d1db09f88565bbbbcb805111060e035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18674598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18104c043da37f500005dc1d2882d62c84adbab64343ce07ec231524fe4fc325`
-	Default Command: `["python3"]`

```dockerfile
# Sat, 21 Oct 2023 18:46:15 GMT
ADD file:e3eb0ea4f652282ad08228d0d146f33998b9e93641756d780ac0205aa828c070 in / 
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c7d387f1f267ea360529df8d70b246f949e1afdb2317cdf84b028cda80a093d1`  
		Last Modified: Thu, 30 Nov 2023 23:20:17 GMT  
		Size: 3.4 MB (3391875 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a004ba37d88223a300024b1e8b487623463145eac66bd4bdcd32a38c0197c58`  
		Last Modified: Fri, 01 Dec 2023 03:44:49 GMT  
		Size: 625.0 KB (625038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1e4c5f087c02bb6a8c900f047da29839a18d38060c581029b9b3042f8fc503d`  
		Last Modified: Fri, 01 Dec 2023 03:45:08 GMT  
		Size: 12.0 MB (11981405 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b2a39cbeb57a49c3f56208e3a0d799582bddc3a2b6d31b86b21b1ec88c99844b`  
		Last Modified: Fri, 01 Dec 2023 03:45:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebfbb490c1b0568e7d7afc1b7f212e62ce6ca39f6fab0bc00e735bebf7014287`  
		Last Modified: Fri, 01 Dec 2023 03:45:07 GMT  
		Size: 2.7 MB (2676050 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:14f705b37205e69e1f626bdca8a9a2aeea7cff582cbe45dad004a1fa24c246d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **875.4 KB (875386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8d2ea14b5d07d564f2c6c05b9febc05c3bf9baef5d6300f8033d57f7496f73`

```dockerfile
```

-	Layers:
	-	`sha256:1b6010d98445d0b3a9311475a94a0429cec63ca03c112b72aab8f9e124dff926`  
		Last Modified: Fri, 01 Dec 2023 03:45:07 GMT  
		Size: 852.2 KB (852239 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ef32335108245f496bcbc9950e074c4821fc90dd37ae7bdedd73099736ab1888`  
		Last Modified: Fri, 01 Dec 2023 03:45:07 GMT  
		Size: 23.1 KB (23147 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; s390x

```console
$ docker pull python@sha256:1c5e1d04ae32d6d2c9a886c2c79f05bc73914c195ed6a07533fb38c32ffd0ce4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18125502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac0b1868846f2cd3b1ca40eaae26602e5e7280275b1f9237b0dc661b045ea793`
-	Default Command: `["python3"]`

```dockerfile
# Sat, 21 Oct 2023 18:46:15 GMT
ADD file:bf416048d22b9a0deecb508385355d79b8d5d12b655c600dbdc0948f7dcbb2c2 in / 
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 18:46:15 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV GPG_KEY=7169605F62C751356D054A26A821E680E5FA6305
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_VERSION=3.12.0
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_PIP_VERSION=23.2.1
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 18:46:15 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 18:46:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 18:46:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:7e9e7e53b618240d2e82e8cab6b677eab6786c4210dcc2b1a35bfd4cb492757e`  
		Last Modified: Thu, 30 Nov 2023 22:43:01 GMT  
		Size: 3.2 MB (3176332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23a5260fc11fc98d3d3f073ba28ca56dad71831f7308cdeac837087945276340`  
		Last Modified: Fri, 01 Dec 2023 02:09:41 GMT  
		Size: 622.9 KB (622885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58a54a775f1cb9344cb98bfcdec77aa5332975de0e60d30c1cc5916b5a3793ef`  
		Last Modified: Fri, 01 Dec 2023 02:09:55 GMT  
		Size: 11.7 MB (11650059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8f448e6a694aac1a97af2bd0f720c771978c922421e2a6eb0b5809d15245f0f`  
		Last Modified: Fri, 01 Dec 2023 02:09:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ad380921d9dd012bfec64a37e9cf8def25cc3bd11f4489e242c13078b1a3252`  
		Last Modified: Fri, 01 Dec 2023 02:09:55 GMT  
		Size: 2.7 MB (2675996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:b76b9e0d44579d99f44cdc088de16e2988b6651b13fb771d3e622aed1ef22520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **875.3 KB (875344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e054e912784a90c94a61b2e273294e60b20f560d00d5ac8789f796788745d7`

```dockerfile
```

-	Layers:
	-	`sha256:3a3b03e70d1c6532c62004c1203e455a5bc7ab024846609f07aa11b1490205f4`  
		Last Modified: Fri, 01 Dec 2023 02:09:55 GMT  
		Size: 852.2 KB (852223 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:dc076f7da350a22aacecd0b3cc5fdb2c52b86ab6d65934dd7332a3480b651423`  
		Last Modified: Fri, 01 Dec 2023 02:09:54 GMT  
		Size: 23.1 KB (23121 bytes)  
		MIME: application/vnd.in-toto+json
