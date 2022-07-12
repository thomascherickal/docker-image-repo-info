## `hylang:0-python3.7-buster`

```console
$ docker pull hylang@sha256:6c855d8e677460a3580aeb4c11f9931cb640c65b8a91837226219d02c3d81169
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `hylang:0-python3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:a3ab09c2fd4edcaa933e137f31d33ff3f3cd85f84ecb7f0b631c0e24065f546a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47469031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6411cbc9f34d5cc89d94a4b857e3f536928ac54dc6ed49065b826842b4735133`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 10:20:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 10:20:34 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 10:20:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:14:02 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Jun 2022 12:14:02 GMT
ENV PYTHON_VERSION=3.7.13
# Thu, 23 Jun 2022 12:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 23 Jun 2022 12:20:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 23 Jun 2022 12:20:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 23 Jun 2022 12:20:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 23 Jun 2022 12:20:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Thu, 23 Jun 2022 12:20:52 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Thu, 23 Jun 2022 12:21:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 23 Jun 2022 12:21:04 GMT
CMD ["python3"]
# Fri, 24 Jun 2022 02:20:56 GMT
ENV HY_VERSION=0.24.0
# Fri, 24 Jun 2022 02:20:56 GMT
ENV HYRULE_VERSION=0.2
# Fri, 24 Jun 2022 02:21:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 24 Jun 2022 02:21:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bff26542d3686b2ab27a0717c161d81eaf10369688d0e880f1c646c3dd7163`  
		Last Modified: Thu, 23 Jun 2022 12:23:23 GMT  
		Size: 2.8 MB (2779284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb8324458c0947bed9733f1e5318074bb5e0ba1e31f5c8453444a77648cfa6d`  
		Last Modified: Thu, 23 Jun 2022 12:26:58 GMT  
		Size: 10.7 MB (10684519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67240a9fcf602616a90b7415c8a3a6c70bf134b97762d8814e5dd01342e7b03`  
		Last Modified: Thu, 23 Jun 2022 12:26:56 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa80be33dc0b7a38576e6c637750df396ca991b1d709c11689254a4eb34c9c85`  
		Last Modified: Thu, 23 Jun 2022 12:26:57 GMT  
		Size: 3.2 MB (3166341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc095a16bc084ea1ec7c9aaee03443bf335b277cbb1b763c6265fb6ee2c44f4`  
		Last Modified: Fri, 24 Jun 2022 02:31:57 GMT  
		Size: 3.7 MB (3698611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:e0e1fc0b7416bdb88adad0b0e8fbe5576ec905f7763bba874494f52f0c901549
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44583981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586bc270c4143dde723c5fadf14b2093ba55b1fdc4792e059ffbc66149fdb8d0`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 00:51:39 GMT
ADD file:b1e035d48236f9259b8573f7b0ac432e69c0d8d42292d24b41d94cba3b942eab in / 
# Thu, 23 Jun 2022 00:51:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:30:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 15:30:37 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 15:30:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:11:00 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Jun 2022 21:11:01 GMT
ENV PYTHON_VERSION=3.7.13
# Thu, 23 Jun 2022 21:30:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 23 Jun 2022 21:30:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 23 Jun 2022 21:30:13 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 23 Jun 2022 21:30:13 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 23 Jun 2022 21:30:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Thu, 23 Jun 2022 21:30:14 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Thu, 23 Jun 2022 21:30:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 23 Jun 2022 21:30:49 GMT
CMD ["python3"]
# Fri, 24 Jun 2022 11:48:38 GMT
ENV HY_VERSION=0.24.0
# Fri, 24 Jun 2022 11:48:39 GMT
ENV HYRULE_VERSION=0.2
# Fri, 24 Jun 2022 11:49:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 24 Jun 2022 11:49:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e6235ec1c9144fd72693df78eccd13b2e35d15fb254f6e0e7dd5ff17a944f0e7`  
		Last Modified: Thu, 23 Jun 2022 01:07:10 GMT  
		Size: 24.9 MB (24889983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca7bf849a23162f9e0320d83ac94aea386673915854b4a6461be68aa6c4b434`  
		Last Modified: Thu, 23 Jun 2022 21:37:10 GMT  
		Size: 2.5 MB (2466059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04e40401ad32aee45cf45a8a659f49e6a8214765ac069f21ed0deb7f1dd7412`  
		Last Modified: Thu, 23 Jun 2022 21:43:53 GMT  
		Size: 10.4 MB (10362532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d460a2301ac0eaadfcf369356165ef10044d7499d0126c9f2c266b7215660d5e`  
		Last Modified: Thu, 23 Jun 2022 21:43:49 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad977d66c4d3e737a533ea899c198b3b2f70070aa0ef2a844c78aa8419a4a1d`  
		Last Modified: Thu, 23 Jun 2022 21:43:51 GMT  
		Size: 3.2 MB (3165961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d21b5292364977a348a1f8460099591509ae6f99907c09c164505c94dab9a`  
		Last Modified: Fri, 24 Jun 2022 11:56:30 GMT  
		Size: 3.7 MB (3699213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:01909ba94121238321dd96b7875de213c124de7ea9fb9a5c44035f6bc535623b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41914617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:602584698dd03bba380e3e1909cd7ebfc0dda384dc327ec8470f96d555eec2ee`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 01:00:49 GMT
ADD file:029ce6b1d94ffab93115ec72e29b81dc578e1e506b9f17808517198fa9a93144 in / 
# Thu, 23 Jun 2022 01:00:50 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 04:04:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 04:04:23 GMT
ENV LANG=C.UTF-8
# Fri, 24 Jun 2022 04:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 11:14:43 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Jun 2022 11:14:43 GMT
ENV PYTHON_VERSION=3.7.13
# Fri, 24 Jun 2022 11:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 24 Jun 2022 11:36:06 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 24 Jun 2022 11:36:07 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 24 Jun 2022 11:36:07 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Jun 2022 11:36:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Fri, 24 Jun 2022 11:36:08 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Fri, 24 Jun 2022 11:36:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Jun 2022 11:36:37 GMT
CMD ["python3"]
# Sat, 25 Jun 2022 06:29:50 GMT
ENV HY_VERSION=0.24.0
# Sat, 25 Jun 2022 06:29:51 GMT
ENV HYRULE_VERSION=0.2
# Sat, 25 Jun 2022 06:30:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Jun 2022 06:30:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4a43dd1ec497b763b016923ec92796419a4f550a0b2c64b17a79c4f7f575643e`  
		Last Modified: Thu, 23 Jun 2022 01:16:47 GMT  
		Size: 22.7 MB (22748000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d04eaa03448f89cc3940e5cbb40d0006ae57c55cfb80e12b1cd2cbf170fa83`  
		Last Modified: Fri, 24 Jun 2022 11:45:27 GMT  
		Size: 2.4 MB (2366955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40054972106c23438820cbf72073c6a959717d68e45437002a3079489dba45fb`  
		Last Modified: Fri, 24 Jun 2022 11:52:48 GMT  
		Size: 9.9 MB (9934397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcb6f6d85380330519b8e51990efd76ad36bf60f89d0f12970ecde297b2c1c7`  
		Last Modified: Fri, 24 Jun 2022 11:52:41 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60b27378af35fa8974dbfb0d100e3023ddecfb7725855d4689fdc8354c319c9`  
		Last Modified: Fri, 24 Jun 2022 11:52:44 GMT  
		Size: 3.2 MB (3165700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c283245dbecaa5fe770a446b2a50adc3d5881aa3d93f4cecd3a79d5b46bb63`  
		Last Modified: Sat, 25 Jun 2022 06:43:42 GMT  
		Size: 3.7 MB (3699331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:7e81993ca09e864519bd78923abb457771e02fad2cac120aa7e4168d9692abf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45925377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d134fb3f40fa2704ee32eb1b1a766400e320ac62e563afb1db45ff37ccaabd`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:08 GMT
ADD file:e491c8ce913289e0c673bd14014c5506cca7b78575aa5c8303ec856525209505 in / 
# Thu, 23 Jun 2022 00:41:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 10:54:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 10:54:59 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 10:55:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:56:24 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Jun 2022 12:56:25 GMT
ENV PYTHON_VERSION=3.7.13
# Thu, 23 Jun 2022 13:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 23 Jun 2022 13:03:13 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 23 Jun 2022 13:03:14 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 23 Jun 2022 13:03:15 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 23 Jun 2022 13:03:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Thu, 23 Jun 2022 13:03:17 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Thu, 23 Jun 2022 13:03:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 23 Jun 2022 13:03:35 GMT
CMD ["python3"]
# Thu, 23 Jun 2022 23:49:30 GMT
ENV HY_VERSION=0.24.0
# Thu, 23 Jun 2022 23:49:31 GMT
ENV HYRULE_VERSION=0.2
# Thu, 23 Jun 2022 23:49:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Jun 2022 23:49:48 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d8b55b2b6839f70c2ed0662b18f4d9724108500136dfd03e999a5f91c815984b`  
		Last Modified: Thu, 23 Jun 2022 00:48:15 GMT  
		Size: 25.9 MB (25914029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711167e5dcf37098a7fd3b366ab784d4e56005d1ddf8506006975e8f70218213`  
		Last Modified: Thu, 23 Jun 2022 13:07:55 GMT  
		Size: 2.6 MB (2643217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb459b97bb8ad6d8b73eaadd297ae523823c0846d87b819ef10884e14f47fd6c`  
		Last Modified: Thu, 23 Jun 2022 13:12:49 GMT  
		Size: 10.7 MB (10723621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985345f891608377da222d3449cf16e96b9359cc079264895f2c8d765e631052`  
		Last Modified: Thu, 23 Jun 2022 13:12:47 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca26710eb7af9584a9238f17de0569fae6b9ed35256026523dadef81d501ec3`  
		Last Modified: Thu, 23 Jun 2022 13:12:48 GMT  
		Size: 2.9 MB (2949545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918aed1dcc32567e7305f5dd223a0b48f28bc239a147c8c44fb4738b28fea5d5`  
		Last Modified: Fri, 24 Jun 2022 00:04:15 GMT  
		Size: 3.7 MB (3694732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:b4f600c5c50d91884aa051334c9cec2954c9097e300fd6fc3feccb0bb731a8b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48011079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370ec74154469222b9e65443ba7f20cb110b0441df7624169b5fef842e4b26ab`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:54 GMT
ADD file:127048950e335136312b4abd45e2f6dbcdbf1641675573278ae97951686fc50a in / 
# Tue, 12 Jul 2022 00:39:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 12:05:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 12:05:23 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 12:05:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:36:05 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 12 Jul 2022 14:36:06 GMT
ENV PYTHON_VERSION=3.7.13
# Tue, 12 Jul 2022 14:43:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 12 Jul 2022 14:43:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 12 Jul 2022 14:43:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 12 Jul 2022 14:43:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 12 Jul 2022 14:43:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Tue, 12 Jul 2022 14:43:49 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Tue, 12 Jul 2022 14:44:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 12 Jul 2022 14:44:03 GMT
CMD ["python3"]
# Tue, 12 Jul 2022 21:42:03 GMT
ENV HY_VERSION=0.24.0
# Tue, 12 Jul 2022 21:42:03 GMT
ENV HYRULE_VERSION=0.2
# Tue, 12 Jul 2022 21:42:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 12 Jul 2022 21:42:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3f7bc4b396f6bcb2720b727a14ac5d6a9809a1d7c1a3363baea1fe8d8c6249ff`  
		Last Modified: Tue, 12 Jul 2022 00:46:09 GMT  
		Size: 27.8 MB (27799525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1b41a4a80c15591c06707a9e25994b3017079e407ff919dfadc141aeff2e2`  
		Last Modified: Tue, 12 Jul 2022 14:48:33 GMT  
		Size: 2.8 MB (2787357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1dd0848eeafbf2c22a3b9daeffd27730bca1c8c49f7f52ca6c186d69b123bc`  
		Last Modified: Tue, 12 Jul 2022 14:53:32 GMT  
		Size: 10.8 MB (10779404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf40d8bfec6342e87efcd934f9ea426899fb2fc4793a194fdc9c9f73357bb044`  
		Last Modified: Tue, 12 Jul 2022 14:53:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924a091b7a5ea12841870373b0fbb4a5e9d9ecc09003b9806b6cafa343570350`  
		Last Modified: Tue, 12 Jul 2022 14:53:31 GMT  
		Size: 2.9 MB (2949559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f524398afd8cba24b425ff27982e577d2336abd379f5adba173d937bc9a06a58`  
		Last Modified: Tue, 12 Jul 2022 21:55:01 GMT  
		Size: 3.7 MB (3695001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:f8164e7cdad1e33ebff1d05c7645bcc1e858697dcef79caafc965996994faeb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45424088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d81d5408cd292fc6a51939de0b7b1f3dda00362a78bc4dcebc3ccd5cde30eb`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 01:11:27 GMT
ADD file:ef55fe42f292a3671fe1772cf96e3559101dea308e79974d1ca92103cb6c7b9c in / 
# Thu, 23 Jun 2022 01:11:31 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 16:51:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 16:51:50 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 16:52:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 02:54:24 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Jun 2022 02:54:27 GMT
ENV PYTHON_VERSION=3.7.13
# Fri, 24 Jun 2022 03:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 24 Jun 2022 03:38:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 24 Jun 2022 03:38:27 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 24 Jun 2022 03:38:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Jun 2022 03:38:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Fri, 24 Jun 2022 03:38:35 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Fri, 24 Jun 2022 03:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Jun 2022 03:39:29 GMT
CMD ["python3"]
# Sat, 25 Jun 2022 02:29:48 GMT
ENV HY_VERSION=0.24.0
# Sat, 25 Jun 2022 02:29:51 GMT
ENV HYRULE_VERSION=0.2
# Sat, 25 Jun 2022 02:31:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Jun 2022 02:31:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4490dc714fa293f64fe0693aa619f1baee9db64f30c00558cfbe5bc798ba1a30`  
		Last Modified: Thu, 23 Jun 2022 01:21:44 GMT  
		Size: 25.8 MB (25814612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab24afb2967203529eb905580f2877ae91275b9bde4222b68bc3faf1388510b`  
		Last Modified: Fri, 24 Jun 2022 03:42:04 GMT  
		Size: 2.3 MB (2327164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ceb98b62dc0e4ad7f0365905bf4e9b6c328d250d2e87c7fea8ddea903e70ed`  
		Last Modified: Fri, 24 Jun 2022 03:46:36 GMT  
		Size: 10.6 MB (10636057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9b3fc605df74a6f996c5bed990f7ac656c71b958c13e77feb047cf6aa3a382`  
		Last Modified: Fri, 24 Jun 2022 03:46:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d7bc8bff37df62602a2a3d170974bd332040b23e209b8be0b19b540b8c4c31`  
		Last Modified: Fri, 24 Jun 2022 03:46:32 GMT  
		Size: 3.0 MB (2950267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc452693c2bf68fb394ecda3a1eb58902f765129c6904c391126b998a4735913`  
		Last Modified: Sat, 25 Jun 2022 02:34:30 GMT  
		Size: 3.7 MB (3695754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:f922dbcdcfccc2bc8b27f5510c0f506e940e52f5f8d5ab2a472754df558b2b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51800301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b6b3339cdf1481f782dfbf6e6824c782e60e0aa03548b79e0d37331e12285db`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 02:03:29 GMT
ADD file:72c3739ee19c484811115caacd1b2bf903a764246b77af65c098817e5a13f8ca in / 
# Thu, 23 Jun 2022 02:03:32 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 19:59:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 19:59:56 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 20:00:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 00:21:09 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 24 Jun 2022 00:21:12 GMT
ENV PYTHON_VERSION=3.7.13
# Fri, 24 Jun 2022 00:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 24 Jun 2022 00:40:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 24 Jun 2022 00:40:33 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 24 Jun 2022 00:40:35 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Jun 2022 00:40:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Fri, 24 Jun 2022 00:40:41 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Fri, 24 Jun 2022 00:41:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Jun 2022 00:41:31 GMT
CMD ["python3"]
# Fri, 24 Jun 2022 19:16:41 GMT
ENV HY_VERSION=0.24.0
# Fri, 24 Jun 2022 19:16:43 GMT
ENV HYRULE_VERSION=0.2
# Fri, 24 Jun 2022 19:17:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 24 Jun 2022 19:17:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:18188ef7804b6b81fced393814287e8c6e18656751108acdbbd364d57775a243`  
		Last Modified: Thu, 23 Jun 2022 02:17:52 GMT  
		Size: 30.6 MB (30560321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a402da4b7f89c9fe20e7f592a804aa7387a2b1c1519fbe91f900584b7c33d3`  
		Last Modified: Fri, 24 Jun 2022 00:46:15 GMT  
		Size: 2.9 MB (2892954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0bbba76432605975f2c9196a0f821018d364bd675033c5ae31c9e5221ce65b`  
		Last Modified: Fri, 24 Jun 2022 00:51:24 GMT  
		Size: 11.5 MB (11479079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344ad3eeccedb41c141a7343770e1d8b0e098b775f63e03d506235110abc2b1e`  
		Last Modified: Fri, 24 Jun 2022 00:51:22 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34e8e401078af204c4a41aebbb68d856932fc7fa8d9c576e377d50c5feeef6`  
		Last Modified: Fri, 24 Jun 2022 00:51:23 GMT  
		Size: 3.2 MB (3167875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63a147cf13fba544e657a40f7cf38c0bfd6d13bd7ce95af5d25ead9384d7274`  
		Last Modified: Fri, 24 Jun 2022 19:28:06 GMT  
		Size: 3.7 MB (3699838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; s390x

```console
$ docker pull hylang@sha256:6fcc44fa9e5d6e4fda42442ba4ee122d8ee66c0ec95cba085f4a97829494051b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45668867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746cede041003ad6d3020a89dfcb5438181a3a06d12ab44c9198fbe7f0895d32`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Jun 2022 00:44:04 GMT
ADD file:b5735387132c5d35278da27339d76ef4a166c7ea012cfe13bd542fd5f0055fb4 in / 
# Thu, 23 Jun 2022 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 10:30:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 10:30:00 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 10:30:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:40:18 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 23 Jun 2022 12:40:18 GMT
ENV PYTHON_VERSION=3.7.13
# Thu, 23 Jun 2022 12:45:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 23 Jun 2022 12:45:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 23 Jun 2022 12:45:25 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 23 Jun 2022 12:45:25 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 23 Jun 2022 12:45:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Thu, 23 Jun 2022 12:45:25 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Thu, 23 Jun 2022 12:45:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 23 Jun 2022 12:45:35 GMT
CMD ["python3"]
# Thu, 23 Jun 2022 22:02:03 GMT
ENV HY_VERSION=0.24.0
# Thu, 23 Jun 2022 22:02:03 GMT
ENV HYRULE_VERSION=0.2
# Thu, 23 Jun 2022 22:02:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Jun 2022 22:02:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:34b063f6640cedaaed5292721bedcce5039c2e2c11d3168badb2d90259505d49`  
		Last Modified: Thu, 23 Jun 2022 00:52:35 GMT  
		Size: 25.8 MB (25758710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c02149d52a7380d40fc006a76ed033091d88cc92a670a80751b3b1444d0cbd`  
		Last Modified: Thu, 23 Jun 2022 12:49:37 GMT  
		Size: 2.5 MB (2466877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363b6018d9b9112112523683c69cbc15f72cb60b7724fa2d910cda829ac8247d`  
		Last Modified: Thu, 23 Jun 2022 12:52:56 GMT  
		Size: 10.6 MB (10578543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384628600641115ef53477d333593ed4a3ef90a6e1913cb47d95d229a43e9026`  
		Last Modified: Thu, 23 Jun 2022 12:52:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9115f10634d606e10b14a30e20ae0fe4bcacd2b014e5b1fbbf07883ca6cce6a`  
		Last Modified: Thu, 23 Jun 2022 12:52:55 GMT  
		Size: 3.2 MB (3165675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72e583c0d0e41d203a3417064d2b8d204c2d2b22e0a601dc3a4b8184025b680`  
		Last Modified: Thu, 23 Jun 2022 22:11:58 GMT  
		Size: 3.7 MB (3698829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
