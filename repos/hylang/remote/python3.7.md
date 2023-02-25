## `hylang:python3.7`

```console
$ docker pull hylang@sha256:076e0c40fb2ce9620a2029357274c30d870f74f579fcc4fd9df555a1a064fb5f
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

### `hylang:python3.7` - linux; amd64

```console
$ docker pull hylang@sha256:bd83122131a0bb75d25ecf3959147ebff145adbd32710408b27fbeca43cfb7ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50146204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6d89646bf2cae77d8bc0abedf5117ed6bffe26b18cb4ce4ce2e9652d4b943c`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:45:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 04:45:53 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 04:45:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:48:57 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 05:48:57 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 05:55:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 05:55:53 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 05:55:53 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 05:55:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Feb 2023 23:28:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 24 Feb 2023 23:28:20 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 24 Feb 2023 23:28:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Feb 2023 23:28:31 GMT
CMD ["python3"]
# Fri, 24 Feb 2023 23:57:56 GMT
ENV HY_VERSION=0.26.0
# Fri, 24 Feb 2023 23:57:56 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 24 Feb 2023 23:58:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 24 Feb 2023 23:58:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43900b2bbd7f3a41cc0b3afe622d03b882980d3997c006ab4309a4b2f2126ad4`  
		Last Modified: Thu, 09 Feb 2023 06:05:32 GMT  
		Size: 1.1 MB (1076306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bcbd81e42519cc20c3b114224f38bbff2953b17c16eb228f8ab4d46e78d53a`  
		Last Modified: Thu, 09 Feb 2023 06:08:08 GMT  
		Size: 10.7 MB (10728463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e9748993b80947c4417213772f270f2021d3ec9a875e4fe1f2fbfa421f8f18`  
		Last Modified: Thu, 09 Feb 2023 06:08:06 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f874f05c3fed9ac89615da0e7df68c8390afc188242aa0784665a40b4f19b857`  
		Last Modified: Fri, 24 Feb 2023 23:36:34 GMT  
		Size: 3.2 MB (3173786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12e79881d7b67b8c86a2baa2d699989d42663d043d247b93a08278e335805f5`  
		Last Modified: Sat, 25 Feb 2023 00:06:27 GMT  
		Size: 3.8 MB (3755606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm variant v5

```console
$ docker pull hylang@sha256:73339b2f49e3ca61e972db52f28dc57f0cc5eb58b86e3145d022d634697536dd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47224006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d8b25f2708b87a025692d90fcc70c243d9900ea2c05ab8cb4fb4066d6a0ca7`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:53:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 05:53:19 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 05:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:27:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 07:27:07 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 07:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 07:35:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 07:35:28 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 07:35:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 09 Feb 2023 07:35:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 07:35:28 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 07:35:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 07:35:47 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 13:04:58 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 13:04:58 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 13:05:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 13:05:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c484fa5df5b5ae3f687aebb0b9d10cf4d895e9753d03aa92d99140c234f58f`  
		Last Modified: Thu, 09 Feb 2023 07:38:43 GMT  
		Size: 1.1 MB (1059618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4fcb89509bbaae21db25434046f65e7ce3ff284882bfd843ae8c9aea7fec9`  
		Last Modified: Thu, 09 Feb 2023 07:41:47 GMT  
		Size: 10.3 MB (10322604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9451bd6412a46aac144a41695c096f1f4c3715fd603528280bd141304611378f`  
		Last Modified: Thu, 09 Feb 2023 07:41:45 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e1404ff4443fa523ae9be72e942aef61438a00aee882d9d96985266f5c176`  
		Last Modified: Thu, 09 Feb 2023 07:41:46 GMT  
		Size: 3.2 MB (3172989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2db6b6143ebe428cab26986a9ccc7e927628f84b95d2c90408457fbb602458`  
		Last Modified: Thu, 09 Feb 2023 13:08:38 GMT  
		Size: 3.8 MB (3752272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm variant v7

```console
$ docker pull hylang@sha256:2a69184a810dc4ae158a4e34cae08b47a33269789ce0c80d006e704a0d11bbbe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44460039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbdaaa0e15b9d1f83be83cab59f05111e94838b82adb090d8f2d4ce6198bb2`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:33:03 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:23:39 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 12:23:39 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 12:32:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 12:32:31 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 12:32:31 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 12:32:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 09 Feb 2023 12:32:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 12:32:31 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 12:32:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 12:32:44 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 21:38:04 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 21:38:04 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 21:38:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 21:38:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e6e3de19fb290e2eecfcbb2c34a2bc0078d282ae6f2f24e710a84231a771e4`  
		Last Modified: Thu, 09 Feb 2023 12:47:38 GMT  
		Size: 1.0 MB (1041591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5227c2f26016f16f19141a9c685cd4a80c4f8c484cacd7df902600bda7ee4af`  
		Last Modified: Thu, 09 Feb 2023 12:51:30 GMT  
		Size: 9.9 MB (9915042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b104592a7bd661cfd259e0e70d0e3e9b093b7d5381fbb2bf2fe1fbda8a31460`  
		Last Modified: Thu, 09 Feb 2023 12:51:28 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d564ce71f373a1f42c55986e9aef39aee9595af692750a824b94c47e8d889e8`  
		Last Modified: Thu, 09 Feb 2023 12:51:29 GMT  
		Size: 3.2 MB (3173078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130bd2dc0a41d5eb98cabc3da8dcbcb01b52eabf207918597045e9379ab280a6`  
		Last Modified: Thu, 09 Feb 2023 21:48:28 GMT  
		Size: 3.8 MB (3752429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:021464486266ff2e24cc137cbb88ba39e4dfca7be294807aced06e22fa479c60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48813502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3097d4ffa878670cd81433470529407717425f603280fcd13812c4214fdedad9`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:51:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 06:51:25 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 06:51:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:54:50 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 07:54:50 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 08:00:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 08:00:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 08:00:55 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 08:00:55 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Feb 2023 23:50:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 24 Feb 2023 23:50:18 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 24 Feb 2023 23:50:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Feb 2023 23:50:27 GMT
CMD ["python3"]
# Sat, 25 Feb 2023 00:55:52 GMT
ENV HY_VERSION=0.26.0
# Sat, 25 Feb 2023 00:55:52 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 25 Feb 2023 00:56:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Feb 2023 00:56:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e56a568739f5da3e0f40727ca225a6d93a75b92df42ac07ed19c0ea7984dc12`  
		Last Modified: Thu, 09 Feb 2023 08:09:33 GMT  
		Size: 1.1 MB (1064151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5510fa1295e805e9eb2a111da50ee87ff037b8e7f084d47e2f8c711c061a0c03`  
		Last Modified: Thu, 09 Feb 2023 08:12:11 GMT  
		Size: 10.8 MB (10757649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25104a9100689ab735ef37cd7fc63d90630110ef50ed85878830ef95610ca25`  
		Last Modified: Thu, 09 Feb 2023 08:12:09 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a43f0838aca5e69df3def02335dc7b22c8e730b6c32bd100d6715dd525ca9f`  
		Last Modified: Fri, 24 Feb 2023 23:58:32 GMT  
		Size: 3.2 MB (3173463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce9df72989c10ae36c074644852184bfa22d590c6445f8882e9f14a5320d885`  
		Last Modified: Sat, 25 Feb 2023 01:04:37 GMT  
		Size: 3.8 MB (3755496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; 386

```console
$ docker pull hylang@sha256:057de52fccf18845065725b59849d9973f2ce11a15d863ab05eba8a39d86a0a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50823178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a448b2f4291b022f3276aa9428479fd9cc1b6bffc274269298c2980201a4e7`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:09:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 08:09:59 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 08:10:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:43 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 09:44:44 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 09:52:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 09:52:20 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 09:52:20 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 09:52:21 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 09 Feb 2023 09:52:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1a96dc5acd0303c4700e02655aefd3bc68c78958/public/get-pip.py
# Thu, 09 Feb 2023 09:52:23 GMT
ENV PYTHON_GET_PIP_SHA256=d1d09b0f9e745610657a528689ba3ea44a73bd19c60f4c954271b790c71c2653
# Thu, 09 Feb 2023 09:52:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 09 Feb 2023 09:52:37 GMT
CMD ["python3"]
# Thu, 09 Feb 2023 20:23:14 GMT
ENV HY_VERSION=0.26.0
# Thu, 09 Feb 2023 20:23:15 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 09 Feb 2023 20:23:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 09 Feb 2023 20:23:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184a06b5a11e3ed0c831f3a07ef485a3f12d06a86f36807a0eb96cbbbc001d5`  
		Last Modified: Thu, 09 Feb 2023 10:04:50 GMT  
		Size: 883.7 KB (883730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f96228d2b1695ce4544d71b8033d8890be9f8634921c2432145d3d6b8ef9`  
		Last Modified: Thu, 09 Feb 2023 10:08:06 GMT  
		Size: 10.8 MB (10832443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abab5c36c7e13c3038036411dd1414b9a6965269f2f484141280bb5e87391df5`  
		Last Modified: Thu, 09 Feb 2023 10:08:05 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a97788c63255f62f23fbeb8ee6a9caf1205d2c9ec42fcce7df91f97c134bb`  
		Last Modified: Thu, 09 Feb 2023 10:08:42 GMT  
		Size: 3.0 MB (2958129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b246008f9d8864243b613e54cd23b31764e2deb11e01d6449de5345f1fe87f`  
		Last Modified: Thu, 09 Feb 2023 20:36:25 GMT  
		Size: 3.8 MB (3751769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; mips64le

```console
$ docker pull hylang@sha256:cc24741250ec776fecefd5605ccc0ce69a7cb73fbcbd02ca3ebcf5116fbeea6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47842224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997ea5dfb953174a977dd18e53d955787f3fd04493b4bbdac7bb52dc4b63c34e`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:57:28 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 03:57:31 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 03:57:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:22:55 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 05:22:58 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 06:09:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 06:09:08 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 06:09:10 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 06:09:13 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 25 Feb 2023 00:39:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Sat, 25 Feb 2023 00:39:26 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Sat, 25 Feb 2023 00:40:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 25 Feb 2023 00:40:20 GMT
CMD ["python3"]
# Sat, 25 Feb 2023 01:00:43 GMT
ENV HY_VERSION=0.26.0
# Sat, 25 Feb 2023 01:00:46 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 25 Feb 2023 01:01:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Feb 2023 01:02:01 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9017d112f64807246351474c93979ce232a9a75cf39e2e1190e5e8b1ff01a6c`  
		Last Modified: Thu, 09 Feb 2023 06:10:37 GMT  
		Size: 844.8 KB (844811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fb3ec502ad120b6d67ffad635327f9bca019e5d382bb72966898e5d7c60c1a`  
		Last Modified: Thu, 09 Feb 2023 06:11:25 GMT  
		Size: 10.7 MB (10651239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c116415a18d97e9a0568c7be5f10dbe64c92269a6cc4d10d39e2ade70f66a056`  
		Last Modified: Thu, 09 Feb 2023 06:11:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea995b2da48aaa3b33397949ebe4e335a8be229148a207a42c565b396a4b6f80`  
		Last Modified: Sat, 25 Feb 2023 00:41:55 GMT  
		Size: 3.0 MB (2959142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15bd2bbba411313915ca13595606f13a2fffa1907bcf481936967e9fae81631`  
		Last Modified: Sat, 25 Feb 2023 01:03:06 GMT  
		Size: 3.8 MB (3752352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; ppc64le

```console
$ docker pull hylang@sha256:19784ab8b7943b0859f7570e001405d6f52eb306a9cf45c34b260a85a9acaf54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54391952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da299de4a079568878cb5bd7a837b8ce75156ebc3f261fa895a5aed311a64a2`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:09:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 08:09:40 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 08:09:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:30:32 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 09:30:33 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 09:52:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 09:52:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 09:52:31 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 09:52:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Feb 2023 23:25:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 24 Feb 2023 23:25:53 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 24 Feb 2023 23:26:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Feb 2023 23:26:17 GMT
CMD ["python3"]
# Sat, 25 Feb 2023 00:00:46 GMT
ENV HY_VERSION=0.26.0
# Sat, 25 Feb 2023 00:00:46 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 25 Feb 2023 00:01:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Feb 2023 00:01:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c969b6572e038316bc81f0fad08b05fce4d8f55eac98e746dd085c93bbcb3`  
		Last Modified: Thu, 09 Feb 2023 09:56:17 GMT  
		Size: 1.1 MB (1094719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5042f04dbf4437a9d6cdc5a366c7b9eec6f001531772fe589ba67dd1ee2bba`  
		Last Modified: Thu, 09 Feb 2023 09:58:06 GMT  
		Size: 11.1 MB (11077800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cb9718f95f2d3876d688acdba8b6088c4676bd5a0d3e5ebed5e889feecaae5`  
		Last Modified: Thu, 09 Feb 2023 09:58:03 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ad9f1f977b364a7d85f5423d7e1892c26adadb775d96a3f0edc78a3c8a215`  
		Last Modified: Fri, 24 Feb 2023 23:35:35 GMT  
		Size: 3.2 MB (3174133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77491ac1220a2cf2f9420df803849e56a49c5fd3db7d15cd06fee2d9f41f5c79`  
		Last Modified: Sat, 25 Feb 2023 00:12:01 GMT  
		Size: 3.8 MB (3755815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.7` - linux; s390x

```console
$ docker pull hylang@sha256:784b8fd4ab2d99156ac5cd0e608161f291ae96d6cf522693b36fb8a03fd45abb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48246038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0464d8e0fbf3eb509b5861c03e3e5299f5a02b70720b2e14c9fc36821041de`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:19:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 06:19:15 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 06:19:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:02:54 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 09 Feb 2023 07:02:54 GMT
ENV PYTHON_VERSION=3.7.16
# Thu, 09 Feb 2023 07:09:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 09 Feb 2023 07:09:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 09 Feb 2023 07:09:30 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 09 Feb 2023 07:09:30 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Fri, 24 Feb 2023 23:48:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 24 Feb 2023 23:48:23 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 24 Feb 2023 23:48:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 24 Feb 2023 23:48:33 GMT
CMD ["python3"]
# Sat, 25 Feb 2023 00:29:54 GMT
ENV HY_VERSION=0.26.0
# Sat, 25 Feb 2023 00:29:54 GMT
ENV HYRULE_VERSION=0.3.0
# Sat, 25 Feb 2023 00:30:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 25 Feb 2023 00:30:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26afbabb71171c124d735797e21a2b4d7efb579558b9d26534097ef8057dc0e`  
		Last Modified: Thu, 09 Feb 2023 07:13:12 GMT  
		Size: 1.1 MB (1075814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ec2c054ca65a7c17214280fff00dff5054a2b36ab41d83796a52ac3557922`  
		Last Modified: Thu, 09 Feb 2023 07:14:59 GMT  
		Size: 10.6 MB (10593247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0cddea57dedea8294cb80883f515a5468537d16ffd4b1a54e50e46e86c8179`  
		Last Modified: Thu, 09 Feb 2023 07:14:57 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbcd7ab3c17ffe5a522d9e76db4adcd9146bb81ca5b403427f4d475519b1e94`  
		Last Modified: Sat, 25 Feb 2023 00:01:26 GMT  
		Size: 3.2 MB (3173616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98da808b42dbf0c9316dbd58edef2bcbc556be2eb01e1e646b7d152851ffcf43`  
		Last Modified: Sat, 25 Feb 2023 00:37:48 GMT  
		Size: 3.8 MB (3755616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
