## `hylang:0-python3.7-buster`

```console
$ docker pull hylang@sha256:f7ac592ecf38422686f252453c27e2b7ca4168ad836442e061917ff6799374d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-python3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:81fe30fab402ac0219c9190744c3a6c49ab2e85ecb2a5f9e795ccde7d47b8950
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47537442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23b846324a5fc40dd4446dbe128b7e8c3937c70d0cfe5611cbf6dbf3d702f66`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:29:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 14:29:22 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 14:29:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:23:49 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 01 Mar 2023 16:23:49 GMT
ENV PYTHON_VERSION=3.7.16
# Wed, 01 Mar 2023 16:30:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 01 Mar 2023 16:30:56 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 01 Mar 2023 16:30:56 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 01 Mar 2023 16:30:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 01 Mar 2023 16:30:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 01 Mar 2023 16:30:56 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 01 Mar 2023 16:31:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 01 Mar 2023 16:31:09 GMT
CMD ["python3"]
# Thu, 02 Mar 2023 02:03:20 GMT
ENV HY_VERSION=0.26.0
# Thu, 02 Mar 2023 02:03:20 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 02 Mar 2023 02:03:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 02 Mar 2023 02:03:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53683fb464bd118081a539c199f8918d31828d851085907fa5a1c5ee324efb3`  
		Last Modified: Wed, 01 Mar 2023 16:33:45 GMT  
		Size: 2.8 MB (2782116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ffe2370788c5d0730d7641dbd0e37e47daf9325151b28bac17827ada608389`  
		Last Modified: Wed, 01 Mar 2023 16:38:12 GMT  
		Size: 10.7 MB (10688211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1996a685ed2781bc4b0d8140ffae35c5fcc9647da1d9ffeb7d674df0126c493f`  
		Last Modified: Wed, 01 Mar 2023 16:38:10 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efa6ee89c3ce1458f1b33d21e53585e4cc7fe3168997eb5817667c597aa880`  
		Last Modified: Wed, 01 Mar 2023 16:38:11 GMT  
		Size: 3.2 MB (3171518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707ddec095e2b0e6a592e568a4b1a3c01ce8e9da1ff51e91d114791a22ca66d4`  
		Last Modified: Thu, 02 Mar 2023 02:11:32 GMT  
		Size: 3.8 MB (3755481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:fa375b970a1044d6b59d6321161164abf04a8e08b29dff80914d08a9d19879dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41981987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b76871c9999f05353cc7fc863df45a5dc0c1fc3e2b3e08439ba47b746c9f2f7`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:13 GMT
ADD file:421c3f57223e760f56f68a9d1c272feaf8239dd72494fc3ef8e9896758e503c8 in / 
# Wed, 01 Mar 2023 01:58:13 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 13:00:48 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 13:00:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 15:33:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 01 Mar 2023 15:33:31 GMT
ENV PYTHON_VERSION=3.7.16
# Wed, 01 Mar 2023 15:41:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 01 Mar 2023 15:41:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 01 Mar 2023 15:41:24 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 01 Mar 2023 15:41:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 01 Mar 2023 15:41:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 01 Mar 2023 15:41:25 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 01 Mar 2023 15:41:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 01 Mar 2023 15:41:43 GMT
CMD ["python3"]
# Thu, 02 Mar 2023 05:34:06 GMT
ENV HY_VERSION=0.26.0
# Thu, 02 Mar 2023 05:34:06 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 02 Mar 2023 05:34:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 02 Mar 2023 05:34:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7138f15de53476a9a56af46eac63ea2f39c78b20aa9ad61ce3018e0eddb748f8`  
		Last Modified: Wed, 01 Mar 2023 02:03:50 GMT  
		Size: 22.7 MB (22748560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263bcfdfa8cf12a4cdb3701ea31c7cc9e9b61291cbf7f31c3412cb6a1ea737e`  
		Last Modified: Wed, 01 Mar 2023 15:47:12 GMT  
		Size: 2.4 MB (2369991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b5c6b64ab0ed035c0987a251a6d38323d690c5e4274e2119571b0e5b37e5c2`  
		Last Modified: Wed, 01 Mar 2023 15:52:53 GMT  
		Size: 9.9 MB (9936845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d2c344d76fe01840de1b2edea634e156bc75d9707538b19777e854094807c`  
		Last Modified: Wed, 01 Mar 2023 15:52:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5dc59ba0768b1d984b3f54e853545c79c854c7c7834e1205522a218a08a9e`  
		Last Modified: Wed, 01 Mar 2023 15:52:52 GMT  
		Size: 3.2 MB (3170887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0919093c75aa4fdad320ff66a3890e8a52f8b5eae31deba79a313eab24012856`  
		Last Modified: Thu, 02 Mar 2023 05:43:13 GMT  
		Size: 3.8 MB (3755470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:db7b5c12a6dce54e12ce8bfcba5cd6917fa0cd19f68e5618b98b308620186d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46228291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d157e596c172d46966821b7c9a5fc6e9b8a2313879949b78213a7a35db0b97e`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 10:23:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 10:23:00 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 10:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:13:52 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 01 Mar 2023 12:13:53 GMT
ENV PYTHON_VERSION=3.7.16
# Wed, 01 Mar 2023 12:20:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 01 Mar 2023 12:20:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 01 Mar 2023 12:20:05 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 01 Mar 2023 12:20:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 01 Mar 2023 12:20:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 01 Mar 2023 12:20:06 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 01 Mar 2023 12:20:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 01 Mar 2023 12:20:16 GMT
CMD ["python3"]
# Wed, 01 Mar 2023 20:28:17 GMT
ENV HY_VERSION=0.26.0
# Wed, 01 Mar 2023 20:28:18 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 01 Mar 2023 20:28:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Mar 2023 20:28:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb47e609cb80ec3793eae0425f40328f8a21fa27e2c385fa3bf3d506009ecfb`  
		Last Modified: Wed, 01 Mar 2023 12:23:01 GMT  
		Size: 2.6 MB (2648670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bd475609cc03b51f0b0b401b5dd302f30aaa39434a90670d039854ca44d07`  
		Last Modified: Wed, 01 Mar 2023 12:27:23 GMT  
		Size: 10.7 MB (10730146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f0e76aa50a1e9b8570d8d78d0013fced21a9c5d439f07a41468b24f2e20f6`  
		Last Modified: Wed, 01 Mar 2023 12:27:22 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7739c6de89a77aa8cf21b157b4fe395b063611b211a78271007f7791c6ab96`  
		Last Modified: Wed, 01 Mar 2023 12:27:23 GMT  
		Size: 3.2 MB (3171103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207cfc1339066d761d5bb223a3e5fd55740e82cdf3c2b94ee505278811a4631f`  
		Last Modified: Wed, 01 Mar 2023 20:36:37 GMT  
		Size: 3.8 MB (3755440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:cc6e215b877467eb86c30e06c4d7a80339d4038bb9b2555a64b73f52335426fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48302472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a9a11b7c28ed32ee61decd9846ea6542ff9ffea380028ab849ef99e46f06e17`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:35 GMT
ADD file:d90e1c78fceb91ea00c9b00cdf477b7254e3d4d37b561698e90b75c62d84320c in / 
# Wed, 01 Mar 2023 01:39:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:03:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 04:03:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 04:03:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:28:56 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 01 Mar 2023 07:28:56 GMT
ENV PYTHON_VERSION=3.7.16
# Wed, 01 Mar 2023 07:39:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	LDFLAGS="-Wl,--strip-all"; 	PROFILE_TASK='-m test.regrtest --pgo 		test_array 		test_base64 		test_binascii 		test_binhex 		test_binop 		test_bytes 		test_c_locale_coercion 		test_class 		test_cmath 		test_codecs 		test_compile 		test_complex 		test_csv 		test_decimal 		test_dict 		test_float 		test_fstring 		test_hashlib 		test_io 		test_iter 		test_json 		test_long 		test_math 		test_memoryview 		test_pickle 		test_re 		test_set 		test_slice 		test_struct 		test_threading 		test_time 		test_traceback 		test_unicode 	'; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 01 Mar 2023 07:39:06 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 01 Mar 2023 07:39:07 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 01 Mar 2023 07:39:07 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 01 Mar 2023 07:39:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 01 Mar 2023 07:39:07 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 01 Mar 2023 07:39:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 01 Mar 2023 07:39:20 GMT
CMD ["python3"]
# Thu, 02 Mar 2023 05:09:17 GMT
ENV HY_VERSION=0.26.0
# Thu, 02 Mar 2023 05:09:17 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 02 Mar 2023 05:09:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 02 Mar 2023 05:09:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5dd0dee7d259a761fe8021e1fd6a2a9a8590880098b27d4f97cfbda4e50bc631`  
		Last Modified: Wed, 01 Mar 2023 01:45:36 GMT  
		Size: 27.8 MB (27798766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a978f2d70c03ae2b43d6ea17659a095336d76126c4de2176f6a4db9f0c68ef7`  
		Last Modified: Wed, 01 Mar 2023 07:44:22 GMT  
		Size: 2.8 MB (2790284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46dbc1a03c2c6a1c21f285f3a024771496a5912bd7332c89079003ae15c3c5b3`  
		Last Modified: Wed, 01 Mar 2023 07:50:04 GMT  
		Size: 10.8 MB (10786533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014d30dddd697342ba187d94252305668d9a28a96d1957cbadfe1c172d9c1cd4`  
		Last Modified: Wed, 01 Mar 2023 07:50:02 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72867f0519793fbdd7fd0836827669f9de2a45871c39c1c519ee07ecb49f2145`  
		Last Modified: Wed, 01 Mar 2023 07:50:03 GMT  
		Size: 3.2 MB (3171216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65221a282a4c76350426081e0e4f9ef1f67b99ab2ed45fb78722284d94c0e8f`  
		Last Modified: Thu, 02 Mar 2023 05:21:52 GMT  
		Size: 3.8 MB (3755440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
