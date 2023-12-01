## `python:3-alpine3.17`

```console
$ docker pull python@sha256:b0ede8b1d04a5899f51ce87789ddd94192cc1ef74760d128f88db627cb8d194c
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
$ docker pull python@sha256:d4c5ac5fba5979a5394adeea46fe8d57ac06816437df453bdd534415f5f22a2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20443216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcef40e467f74d55fcad70daf7baea388b0f2887a6f4ec4a69844b922cb3551`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
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
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92a8a636ed19fb650cdc43c55b45f818016f87d29f8fcc5a2aec118fe834f13e`  
		Last Modified: Wed, 29 Nov 2023 06:26:34 GMT  
		Size: 622.6 KB (622611 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bae06e7e8d633c283339c84be4d0ce12113a2fe37fbcfdf5aa9c42fb1f956b4`  
		Last Modified: Wed, 29 Nov 2023 06:27:18 GMT  
		Size: 13.8 MB (13765766 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73c1f1dd9faf67f79e7ca6bf7ea5119f6c36c0c057f7a7ac73a55ac7d35eb64c`  
		Last Modified: Wed, 29 Nov 2023 06:27:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8081f28fa3673f2160071f524b4c65c7d97c002ff3ab5c989f320611a7f901`  
		Last Modified: Wed, 29 Nov 2023 06:27:17 GMT  
		Size: 2.7 MB (2676002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:5106de38dfb2d120b869e25217914533bc7f409754e4f57bff3a7c49bdfcde69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **877.0 KB (876980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ddf2811a9c67f8925e1d3d604e6da125b19c90287bcaf22945119d153362cd`

```dockerfile
```

-	Layers:
	-	`sha256:8fa2052919e5ca0930239a3b34edca923132f86d02655fb0a07dcae60fc545c2`  
		Last Modified: Wed, 29 Nov 2023 06:27:17 GMT  
		Size: 853.9 KB (853859 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:df9715847cf40671dd02dba3edf949b5063df24aa2acc103f97289beaae754d6`  
		Last Modified: Wed, 29 Nov 2023 06:27:17 GMT  
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
$ docker pull python@sha256:a901e157895945917bc582e0646302eded4be79376493e829d8a443646f22a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18682412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4ca3679714c838e299e22cd539729e06257598469b675f4b92883623c0d2df`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
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
	-	`sha256:b82e4fd40279a40aa2eecd301fabb2dca254727cc09daa8d0caf69ac28c44af1`  
		Last Modified: Mon, 07 Aug 2023 19:58:08 GMT  
		Size: 2.9 MB (2869425 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0faf0dfb497db35e9a29b91b2c4381af732a686e61fe8893d27e229fa58d796a`  
		Last Modified: Wed, 29 Nov 2023 10:11:38 GMT  
		Size: 623.8 KB (623768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d73c37be4e778f02f463bb727dfb92319c2d06a2f1a5621b909977146ab3196`  
		Last Modified: Wed, 29 Nov 2023 10:12:20 GMT  
		Size: 12.5 MB (12512926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4abc91cd4fddefd802fdd53dc9d8ded40aabc396a8c47b92e6addab54fda9e09`  
		Last Modified: Wed, 29 Nov 2023 10:12:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c0a0c3d9377117708456dcf62192364a06fb2345cffb93cb9230adc22a5003d`  
		Last Modified: Wed, 29 Nov 2023 10:12:19 GMT  
		Size: 2.7 MB (2676063 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:a2aee8fd22fc76f54b44742402ab6efb02810f2047bab10c344172a1ef89cebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **879.6 KB (879553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1cb81ce13cbf018f86cc705d734241172da959636309d66a759e7ab90dcdc3`

```dockerfile
```

-	Layers:
	-	`sha256:18b0b9c239031cfc33c3b627789f4909450212b14a8c35bcb7ddfd5815934153`  
		Last Modified: Wed, 29 Nov 2023 10:12:20 GMT  
		Size: 856.3 KB (856345 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5bd2089041412a7f9f406668c6fcb926dba58173ce4f065debe053cf10b31673`  
		Last Modified: Wed, 29 Nov 2023 10:12:19 GMT  
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
$ docker pull python@sha256:9b849bfb011fcfca23577d7e274855b26c8a7a4ad4c8f3c9f8888722a257d43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.8 MB (20799757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d723f0d1d08adcf5e7426d15de40e90f4453843f329c8a9e6cf9205f82418ea3`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
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
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:83746fdf4894210bc24e6397c9c9b318de98d8e8d13da8cceff2a8edfa836990`  
		Last Modified: Wed, 29 Nov 2023 08:22:01 GMT  
		Size: 625.0 KB (625028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:944c9c5bf84a29a35bfe91ae3beeb2c7d66cbefffe2ae989594bada3e020fdc0`  
		Last Modified: Wed, 29 Nov 2023 08:22:44 GMT  
		Size: 14.1 MB (14107138 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e59a0454e93f3273553580eafd66d4f7b8da67d6bae3b64579f470ebe3b3f9a2`  
		Last Modified: Wed, 29 Nov 2023 08:22:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4d91df2b6c49cbaaac8d5ad16369105b99ded24d35725a5c7ebd96a34003480`  
		Last Modified: Wed, 29 Nov 2023 08:22:44 GMT  
		Size: 2.7 MB (2676013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:bc46144504c3c217369e6e53b100878ba3899bb63c6b9b7b873ee5c116649e49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **875.4 KB (875386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5cca5cc31442c60ea3e05405e9a980fed9abefe172b8140629adb7a245d32b`

```dockerfile
```

-	Layers:
	-	`sha256:e485e82045d03e61630c27edbe12c9189b8f22ea44e3c895796cd17cab29231e`  
		Last Modified: Wed, 29 Nov 2023 08:22:44 GMT  
		Size: 852.2 KB (852239 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1a618717a1deae320578290c77a2059926b5a2f63a264fe1dfd2fc6378d92675`  
		Last Modified: Wed, 29 Nov 2023 08:22:43 GMT  
		Size: 23.1 KB (23147 bytes)  
		MIME: application/vnd.in-toto+json

### `python:3-alpine3.17` - linux; s390x

```console
$ docker pull python@sha256:6edac41660933d16437c0d19c4c26767d5595bb22b546ea0cd00569555e4e7a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (20041177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45c0cd48b2089a59885bf4a693574e83d1cb4b67ab2fa959d3b28fa02cb4d0b`
-	Default Command: `["python3"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
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
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a6354c7ad8393363e8fe771f3d1b3cb48512755dff9e4e0f6c4f015d1b19cfd`  
		Last Modified: Wed, 29 Nov 2023 06:23:29 GMT  
		Size: 622.9 KB (622889 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e69e2002e9eb28c78fe554fe8ff964b1a37f78daa7ee8b2af92f2092acda1a5`  
		Last Modified: Wed, 29 Nov 2023 06:24:05 GMT  
		Size: 13.6 MB (13566060 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ef3f661acea74321203ec976cce9bda9170a91f8b309a09ee449c596b08bb0`  
		Last Modified: Wed, 29 Nov 2023 06:24:04 GMT  
		Size: 229.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e5ba57389397ecb45ffdfad008e284693764008fa5eccfb3e0d6606dbbb7538`  
		Last Modified: Wed, 29 Nov 2023 06:24:04 GMT  
		Size: 2.7 MB (2676025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `python:3-alpine3.17` - unknown; unknown

```console
$ docker pull python@sha256:3e01ca4067e887c137e2947a91327005d2c39d33f2ccc07d760bdccd8b77c26c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **875.3 KB (875344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a51134a305497c1feb79aa558dbf2244911aecd4897c831cffd678176c713f6`

```dockerfile
```

-	Layers:
	-	`sha256:14211264855b6ca27b77f26c495273b952c11f92ddd2152d9f3f97fd7dcb1e89`  
		Last Modified: Wed, 29 Nov 2023 06:24:04 GMT  
		Size: 852.2 KB (852223 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2dc221b83c0f06967a1b1fc5261d5e9d73e5473c147e6427fe37464f3d2fe9bb`  
		Last Modified: Wed, 29 Nov 2023 06:24:04 GMT  
		Size: 23.1 KB (23121 bytes)  
		MIME: application/vnd.in-toto+json
