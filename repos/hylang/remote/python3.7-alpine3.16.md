## `hylang:python3.7-alpine3.16`

```console
$ docker pull hylang@sha256:7de95bf65e4de4ce883b16a877a91287b55b443bc0c2d527ab9ad4f4f7d43553
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

### `hylang:python3.7-alpine3.16` - linux; amd64

```console
$ docker pull hylang@sha256:fc0730d87807ec627735ba261c5ffb277a667bf4b842d1174670b3312d457f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21645366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa948419f88a8a193566659f07752fedf3f9f1737261b3ad32a7b4c980aecf49`
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
# Sat, 12 Nov 2022 07:39:00 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 08 Dec 2022 04:23:45 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 04 Feb 2023 04:33:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 04 Feb 2023 04:33:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 04 Feb 2023 04:33:05 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 04 Feb 2023 04:33:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 04 Feb 2023 04:33:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 04 Feb 2023 04:33:05 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 04 Feb 2023 04:33:11 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 04 Feb 2023 04:33:11 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 02:57:35 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:57:35 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:57:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:57:53 GMT
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
	-	`sha256:70e2ca60d8d0925ee312b419a2e05ff15031548afa21c6f3c3a90ad73ecc68fb`  
		Last Modified: Sat, 04 Feb 2023 04:42:27 GMT  
		Size: 11.5 MB (11539514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11780abaf601d9944ad0877057d6fe6b31c54a1e65d1c120506a8273f85f9ce`  
		Last Modified: Sat, 04 Feb 2023 04:42:26 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca552efeeca00431340e6c19f62a03b9b00f5eec5d63b4c08844ee1f1a18032`  
		Last Modified: Sat, 04 Feb 2023 04:42:28 GMT  
		Size: 2.9 MB (2881863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691aaf835bb31fc1f542c2689739eac44e0358ebf7d2b4d822807058a30b4d0f`  
		Last Modified: Thu, 09 Feb 2023 03:09:23 GMT  
		Size: 3.8 MB (3755652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; arm variant v6

```console
$ docker pull hylang@sha256:2b185966642bada53297959ed5c0016e7b6616c7d22f3f6850155f6a40573280
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.7 MB (20667413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827384427788d142749fe211aca7470c9625dd757041effb4ae907ee1aab0432`
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
# Sat, 11 Feb 2023 05:52:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 05:52:08 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 06:01:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 06:01:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 06:01:29 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 06:01:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 06:01:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 06:01:29 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 06:01:36 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 06:01:36 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 09:46:25 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 09:46:25 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 09:46:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 09:46:47 GMT
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
	-	`sha256:d40546a141d7c419c60dacb5794638a2f8148cd2b4c1d8f785e088d2f7cd4d2a`  
		Last Modified: Sat, 11 Feb 2023 06:07:02 GMT  
		Size: 10.8 MB (10750227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e9edde398207e7b62aa72676d7590d88f62c12a768934477fb4152922cef`  
		Last Modified: Sat, 11 Feb 2023 06:07:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5069598b08ec367076ca8b0f4d0b220cead65daea8cc3091eea7d7d4fc0716f2`  
		Last Modified: Sat, 11 Feb 2023 06:07:00 GMT  
		Size: 2.9 MB (2881561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200eb5405b6b613795e82d1bb71ab821480fa49daf3385c0faf81d1cb971b0a3`  
		Last Modified: Sat, 11 Feb 2023 09:55:13 GMT  
		Size: 3.8 MB (3752396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; arm variant v7

```console
$ docker pull hylang@sha256:f4fd17499fa0e833cad6db3ce9967fc558faf034a757d854274dcb39e7c5c4de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (20012291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f955036279b0c8eff23b4f7a1e0c44a93b057dd89750029b2a83090a5ab9b8`
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
# Sat, 11 Feb 2023 05:07:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 05:07:25 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 05:16:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 05:16:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 05:16:30 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 05:16:30 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 05:16:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 05:16:31 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 05:16:38 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 05:16:39 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:33:20 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:33:20 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:33:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:33:37 GMT
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
	-	`sha256:8c75660164af4c75e4bf399dc47f79a0366210d35c28fd8b4e0eea79da4c55e0`  
		Last Modified: Sat, 11 Feb 2023 05:25:51 GMT  
		Size: 10.3 MB (10298451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac066c015084b8b68f73d974689a38929badf1a2e4ec107a95a4418db22617c1`  
		Last Modified: Sat, 11 Feb 2023 05:25:49 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f6c4d5a6b34c6d437426d1934840cab4d7351adc30c14177c58c77e7d05dff`  
		Last Modified: Sat, 11 Feb 2023 05:25:50 GMT  
		Size: 2.9 MB (2881550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0317e4f2142bb7866c05969f61be7a3ccc654242d7cc22a58a5cc455d34963`  
		Last Modified: Sat, 11 Feb 2023 12:43:51 GMT  
		Size: 3.8 MB (3752261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:6d5f1ef302d72168d47264d4da1da6d49227d21edf6a34ae9ac3c878a63a0f4c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21230573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13311453e1be3ebccea1a92b3fe039ccae1e81c21c80642052b0f2db5aee897`
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
# Sat, 11 Feb 2023 04:53:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 04:53:37 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 04:59:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:59:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:59:59 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 04:59:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 04:59:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:59:59 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 05:00:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 05:00:05 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 08:37:19 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 08:37:19 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 08:37:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 08:37:34 GMT
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
	-	`sha256:6aec9f8908d3df5fa9909feba9b6a0536bc65d460ddde5946b6ea547908f0641`  
		Last Modified: Sat, 11 Feb 2023 05:04:55 GMT  
		Size: 11.2 MB (11220420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a938269c8374114c477c51b8d5005bb5974caf0b676a8d63f77e9cdbe9d5ffd`  
		Last Modified: Sat, 11 Feb 2023 05:04:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e278e8bf5099bf5ca6658960690e496ddc5d9ea00446e9a075be8e7ade1df5`  
		Last Modified: Sat, 11 Feb 2023 05:04:54 GMT  
		Size: 2.9 MB (2881815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ed46ea59863e60e7c6156d3bd575191851b816e626366562a2d2b268d895af`  
		Last Modified: Sat, 11 Feb 2023 08:43:44 GMT  
		Size: 3.8 MB (3755482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; 386

```console
$ docker pull hylang@sha256:9c9688de385f0a6784925e9b0d2523fd89d2dec52b5bcf3b272b1cf7cc534076
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21441417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdc7cf9aaa1d81fa4f6b863ef721cb27919a37c32924e3f69703840fef12878`
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
# Sat, 11 Feb 2023 02:23:58 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 02:23:59 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 02:32:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 02:32:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 02:32:03 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 02:32:04 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 02:32:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 02:32:06 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 02:32:13 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 02:32:14 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 06:01:35 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 06:01:36 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 06:01:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 06:01:59 GMT
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
	-	`sha256:3e285d3368f04b8333a77d417b2d5538126cffe65500980b2ad03b50189e563c`  
		Last Modified: Sat, 11 Feb 2023 02:40:16 GMT  
		Size: 11.3 MB (11327384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6be80c2735dd562fa1c282fd40b4bfbd5737b542d1347b85481907ef9e0e1a`  
		Last Modified: Sat, 11 Feb 2023 02:40:14 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8632fedb9a0385ff1f5b9896791bb530f8bf8bad6a39d3570a13849d25b5e2`  
		Last Modified: Sat, 11 Feb 2023 02:40:15 GMT  
		Size: 2.9 MB (2881824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f512f00816b0d9444c95aa213baf2bb2acae24b38bbffe16c531c4021b800`  
		Last Modified: Sat, 11 Feb 2023 06:12:03 GMT  
		Size: 3.8 MB (3751696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; ppc64le

```console
$ docker pull hylang@sha256:90f1fc76abd21b8036e0e0e85bb192246455598c765fc76f29cc885710f042fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21547090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe9cefa3f0d034a6a35d918e84257905d520eb4347f8fef68c759c281b2ea36`
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
# Sat, 11 Feb 2023 04:01:11 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 04:01:11 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 04:16:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:16:06 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:16:07 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 04:16:07 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 04:16:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:16:08 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:16:20 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:16:21 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:42:26 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:42:27 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:43:19 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:43:21 GMT
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
	-	`sha256:b1cdbcf4ac56ca4e5236e30cb0c402c83cccad3604645de66f2f6716246e6b87`  
		Last Modified: Sat, 11 Feb 2023 04:24:17 GMT  
		Size: 11.4 MB (11434274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00949f8ec69a35394b76c22a5f25fd31aa1d114af0292bfaabe5c6b2eb74176b`  
		Last Modified: Sat, 11 Feb 2023 04:24:14 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d6bee92c718aa4fb6ced8fe3e0dfef69438ae73c98338172790aa84bcda7b`  
		Last Modified: Sat, 11 Feb 2023 04:24:15 GMT  
		Size: 2.9 MB (2881841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5b065886eac1394afb9eee189a355782730b51afe9d0251b47fbbfbeace227`  
		Last Modified: Sat, 11 Feb 2023 12:53:02 GMT  
		Size: 3.8 MB (3755817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7-alpine3.16` - linux; s390x

```console
$ docker pull hylang@sha256:926235900cfef2e21c0a4cb3ac8c2e2dc94a75b1f60a6f1a56a70ecd6c2ce681
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21054642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8dcf439166ad0aee1bbbc3392f8d9d364b6c7743dd29051769c69746409a7b`
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
# Sat, 11 Feb 2023 10:35:14 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 10:35:14 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 10:41:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 10:41:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 10:41:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 10:41:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 10:41:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 10:41:53 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 10:41:59 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 10:41:59 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:46:59 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:47:00 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:47:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:47:14 GMT
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
	-	`sha256:2871dbb3c153ef57c0da1445a70930c871890aeca3fb7b15d1d560c585f3ca85`  
		Last Modified: Sat, 11 Feb 2023 10:47:15 GMT  
		Size: 11.2 MB (11156859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a90c74dceeed34a01049a9c2650e2a4038f6d0d02e45707e876f84c398a18`  
		Last Modified: Sat, 11 Feb 2023 10:47:14 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022ef1c3aa4ebe13affad018d0d0f9c997a865d3ed2e2c2c39c4e5e2ed18d4ad`  
		Last Modified: Sat, 11 Feb 2023 10:47:14 GMT  
		Size: 2.9 MB (2881817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956d548575ecdd1b478a9026f2419dd8845ed68a9afc15c4a92ace2a60022991`  
		Last Modified: Sat, 11 Feb 2023 12:53:18 GMT  
		Size: 3.8 MB (3755503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
