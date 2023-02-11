## `hylang:0-python3.7-alpine`

```console
$ docker pull hylang@sha256:d78554ad2411eff1b8956ea6bfc8d7fb5f176a21bf5cbc5fc9afb3f4221bff0c
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

### `hylang:0-python3.7-alpine` - linux; amd64

```console
$ docker pull hylang@sha256:767ea2bcb9e3f9129fb754f19948e01f34141368d1a515fad82f4a8819a058e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21682485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6597b030c24ca0e552816477e0ad77cc349e31b6e4803a787d3a8b21754e408`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:05:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 20:09:04 GMT
ENV LANG=C.UTF-8
# Mon, 09 Jan 2023 20:09:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Mon, 09 Jan 2023 21:01:58 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Mon, 09 Jan 2023 21:01:58 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 04 Feb 2023 04:25:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 04 Feb 2023 04:25:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 04 Feb 2023 04:25:59 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 04 Feb 2023 04:25:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 04 Feb 2023 04:26:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 04 Feb 2023 04:26:00 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 04 Feb 2023 04:26:06 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 04 Feb 2023 04:26:06 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 02:57:11 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:57:11 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:57:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:57:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd9832a787c7d68019488dcae52ce17e79f7cc4217fb549f6ff5c3fa1e10a93`  
		Last Modified: Mon, 09 Jan 2023 21:10:29 GMT  
		Size: 622.9 KB (622912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a296d0981714e21887ea12644875f392fd823dd281e75a067193e35171ba347`  
		Last Modified: Sat, 04 Feb 2023 04:42:14 GMT  
		Size: 11.1 MB (11051261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d1aef70d00cd9c0ad7d8ffe3296bcb324bbe1369e2e6557d1fc8cb98164581`  
		Last Modified: Sat, 04 Feb 2023 04:42:13 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93f823bd88e67eaf9a3247368ce3bcafaa861231d95e96eec145de20259e911`  
		Last Modified: Sat, 04 Feb 2023 04:42:13 GMT  
		Size: 2.9 MB (2881860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869f2fe5c9ea1781dc0af42af562bd02fcdcaca6e8290f17de2f8df16bb731e9`  
		Last Modified: Thu, 09 Feb 2023 03:09:00 GMT  
		Size: 3.8 MB (3755594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; arm variant v6

```console
$ docker pull hylang@sha256:f9ad3179d87d27c1dff05770b8d062757ef232d452037163cd0de697d98f4979
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21007967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7c3c33c5ae15a34fec8d1571e7dcc2d36acd4167ec0360003e5754ffdf30bd`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:44:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 03:44:38 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 03:44:39 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 05:43:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 05:43:36 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 05:51:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 05:51:42 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 05:51:42 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 05:51:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 05:51:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 05:51:43 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 05:51:50 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 05:51:50 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 09:45:57 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 09:45:57 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 09:46:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 09:46:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bc7384407f1883772f74c693a37ca7cbea92dd7cc7982c9f24fc04f6acf89d`  
		Last Modified: Sat, 11 Feb 2023 06:03:38 GMT  
		Size: 624.9 KB (624941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b3c9bfee90379b899bde67b7522df6dfaced3e539848d802937ccd295a0a7d`  
		Last Modified: Sat, 11 Feb 2023 06:06:44 GMT  
		Size: 10.6 MB (10637828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d966810a1b6cc6ee288493a8d5655c41f77773c6a5669b8ec95a5148bdfcc18`  
		Last Modified: Sat, 11 Feb 2023 06:06:41 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc80b91889b2737cc032beee508ff22cd23cdf77787bcff9bc8843fe2eaebfe`  
		Last Modified: Sat, 11 Feb 2023 06:06:42 GMT  
		Size: 2.9 MB (2881566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5efa4df129d5262ea59624b16eac0489f439e40cd9a0fc7b7740f563052ccc`  
		Last Modified: Sat, 11 Feb 2023 09:54:39 GMT  
		Size: 3.8 MB (3752518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; arm variant v7

```console
$ docker pull hylang@sha256:d09601dc963c5c9fef8b7eda3c9ef121038a46d1f9ad5aeb579debaad1fed9d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20401752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3b7392dcde0dcabdcc29557e77fad7e0719a5fabcd3ff345e8715e425039d3`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:13:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:13:05 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:13:07 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 04:59:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 04:59:10 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 05:07:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 05:07:07 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 05:07:08 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 05:07:08 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 05:07:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 05:07:08 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 05:07:14 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 05:07:14 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:32:57 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:32:57 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:33:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:33:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b306be95143370e9c4625f9567dbd30326ff6fa0d5467a88dc79756e2da560`  
		Last Modified: Sat, 11 Feb 2023 05:21:58 GMT  
		Size: 623.9 KB (623894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23c79f630806a8a5dfcf6ae2800c06e1d0ddc74b24a07fab991a9d460c54a69`  
		Last Modified: Sat, 11 Feb 2023 05:25:32 GMT  
		Size: 10.3 MB (10275487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbb8d11559977c1429a3296881360426ffad3992c887cc726942235e8282bca`  
		Last Modified: Sat, 11 Feb 2023 05:25:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132fcd7059a65688ce690f06c3b3b295bcf020cff4efda3eae7e9e6946d753d0`  
		Last Modified: Sat, 11 Feb 2023 05:25:31 GMT  
		Size: 2.9 MB (2881392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9921d44b9c86ee6c5332eefffe3ee77dea1e19e8eba42ecbc92d5e86fd25f823`  
		Last Modified: Sat, 11 Feb 2023 12:43:20 GMT  
		Size: 3.8 MB (3752255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:12e56772c4d7684282a6830d7397126286284fc85969fc5736e83a0991eb0638
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21533303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799ea3b46a1875a52474560d5bcaa74f94f8f3e6b2c2bcbce17c00e62bf8afdb`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:21:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 03:21:17 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 03:21:18 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 04:47:43 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 04:47:43 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 04:53:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:53:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:53:15 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 04:53:15 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 04:53:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:53:15 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:53:21 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:53:21 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 08:37:00 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 08:37:00 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 08:37:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 08:37:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba2f6867522ee9d2e8dcc9b1ad3ec5bafe75da976a3e613ff26cbc98738b48`  
		Last Modified: Sat, 11 Feb 2023 05:02:08 GMT  
		Size: 624.9 KB (624860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1178b7c6752e0d2eb293ee14286ec1f75d0f868d9826bcaba24fe33affea99`  
		Last Modified: Sat, 11 Feb 2023 05:04:41 GMT  
		Size: 11.0 MB (11008807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd7dfc9c660f2a9be2e537fd8f7f3c289ea1ba335c957472bd9a51630c9b449`  
		Last Modified: Sat, 11 Feb 2023 05:04:40 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89954f3f0d60e450a18357de5b7bc7d50046ac8636803e6d9169e9351a4621b2`  
		Last Modified: Sat, 11 Feb 2023 05:04:40 GMT  
		Size: 2.9 MB (2881840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb89e69c348909a9d0f3183af086e16c8a90ba9daa675f25caaceaeb4492b31`  
		Last Modified: Sat, 11 Feb 2023 08:43:22 GMT  
		Size: 3.8 MB (3755607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; 386

```console
$ docker pull hylang@sha256:2fc44ff8c77710c8742dd668973375c0cacb8b2a168ece7082ce48879866da0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.9 MB (21949132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765429898ba8dd4add0ef939bdb891ce151d4bba7336af61771df6ff5e0f526f`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:41:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:41:17 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:41:19 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 02:16:44 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 02:16:45 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 02:23:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 02:23:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 02:23:30 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 02:23:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 02:23:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 02:23:33 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 02:23:41 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 02:23:41 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 06:01:04 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 06:01:05 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 06:01:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 06:01:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d18ebabb6f744ad06852ca1e354e05d3d1db41b0c3e06758dfb23a678e0b88c`  
		Last Modified: Sat, 11 Feb 2023 02:36:23 GMT  
		Size: 623.2 KB (623161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204dc38bc96c49598406757bf107009ec6df7146b7818849824210cf48245f69`  
		Last Modified: Sat, 11 Feb 2023 02:39:49 GMT  
		Size: 11.3 MB (11279841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535900b7e575269a6f642e8b6aae7c8bf53090a218584e292ea50f367969bcf5`  
		Last Modified: Sat, 11 Feb 2023 02:39:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528101aafe5f69b23b8b3e5460edc3027ef023a2aa41e70efb83bf2bb070f7c3`  
		Last Modified: Sat, 11 Feb 2023 02:39:48 GMT  
		Size: 2.9 MB (2881818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c60d8378bff209849719755060ca9538c2152e5df4a7abae553862bbe3b2ef`  
		Last Modified: Sat, 11 Feb 2023 06:11:34 GMT  
		Size: 3.8 MB (3751730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; ppc64le

```console
$ docker pull hylang@sha256:4e3524b33bf89e35e0d7bb69969a7be3310efd0a6db8f97953d9658b15dfa58e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.1 MB (22090410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf1642beba8c5f1364ba59dc086b3c21b2fcb9e39512f9f12202567e13a4f00`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:43:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 00:43:03 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 00:43:06 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 11 Feb 2023 03:48:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 11 Feb 2023 03:48:13 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 11 Feb 2023 04:00:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 11 Feb 2023 04:00:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 11 Feb 2023 04:00:41 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 11 Feb 2023 04:00:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 11 Feb 2023 04:00:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 11 Feb 2023 04:00:42 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 11 Feb 2023 04:00:55 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 11 Feb 2023 04:00:56 GMT
CMD ["python3"]
# Sat, 11 Feb 2023 12:41:26 GMT
ENV HY_VERSION=0.26.0
# Sat, 11 Feb 2023 12:41:27 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 11 Feb 2023 12:42:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 11 Feb 2023 12:42:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a413709dc452963685d247540895a4124799730691a6ec60fab72353e238035`  
		Last Modified: Sat, 11 Feb 2023 04:19:55 GMT  
		Size: 625.3 KB (625282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60434e271bf3f80f7aacb8ad487417b6e8248467c1eab52c9d20666504c60bcd`  
		Last Modified: Sat, 11 Feb 2023 04:23:57 GMT  
		Size: 11.4 MB (11436447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2818921a92df80e05c0293cf337573f70949bc3f414382e6063685a33b51b25`  
		Last Modified: Sat, 11 Feb 2023 04:23:54 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e530b8ae62aeeba725b29054725567324f05a9f97eb42af96f66c0950ab9eb03`  
		Last Modified: Sat, 11 Feb 2023 04:23:55 GMT  
		Size: 2.9 MB (2881878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51134e20cc3efccb56916d068491d2cdd46e6c48799e04c6f42c82b6774d2a7b`  
		Last Modified: Sat, 11 Feb 2023 12:52:27 GMT  
		Size: 3.8 MB (3755823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-alpine` - linux; s390x

```console
$ docker pull hylang@sha256:7d28ae0f06e7f26961491e01e75f991916e51083b46b13113b54897e900f9446
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21457231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64afc2280943ecab9f5d0cc70936699b6144ba68e45d76ad32588345fb6cc14`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 23:26:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 23:26:45 GMT
ENV LANG=C.UTF-8
# Mon, 09 Jan 2023 23:26:48 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 10 Jan 2023 00:44:12 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Jan 2023 00:44:13 GMT
ENV PYTHON_VERSION=3.7.16
# Sat, 04 Feb 2023 02:07:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Sat, 04 Feb 2023 02:07:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Sat, 04 Feb 2023 02:07:03 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Sat, 04 Feb 2023 02:07:03 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 04 Feb 2023 02:07:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Sat, 04 Feb 2023 02:07:03 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Sat, 04 Feb 2023 02:07:09 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 04 Feb 2023 02:07:10 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 02:25:38 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 02:25:39 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 02:25:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 02:25:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6acf5c56be5c3721cd05ad50683db0ec17f48fc7ada071d7007f6c109b5bb1`  
		Last Modified: Tue, 10 Jan 2023 00:56:26 GMT  
		Size: 623.2 KB (623214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1934bb2fd350883215133325a7de3908195f624f4f0da9e7698687af1fd7f02e`  
		Last Modified: Sat, 04 Feb 2023 02:21:38 GMT  
		Size: 11.0 MB (11025419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded192475747eed6f936b93349265f06ec668a47dc2e7cee8bcb878d857f90c0`  
		Last Modified: Sat, 04 Feb 2023 02:21:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777ebbfaaa4eed123dd493de8816f5ef6eb82e7d2fa73ed7abb4c757f69c7f68`  
		Last Modified: Sat, 04 Feb 2023 02:21:37 GMT  
		Size: 2.9 MB (2881824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c123c96658fd458ba19095a2c324ee1d2bcd038846653eea9b587bdac83cdde6`  
		Last Modified: Thu, 09 Feb 2023 02:34:08 GMT  
		Size: 3.8 MB (3755799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
