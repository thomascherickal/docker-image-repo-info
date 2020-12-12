## `hylang:0-python3.7-stretch`

```console
$ docker pull hylang@sha256:57750429b96e21d21289ba88c420cf8ee00f6d62c0db15fa35ee6af58ab48a21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-python3.7-stretch` - linux; amd64

```console
$ docker pull hylang@sha256:97e3b581c6a37af230fd126d2c562f3b19c55ca1da1c09222ece9a6108bbbbca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40260135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdf75327db4fa8bbeca845b17457e0beaebfa81285302107cf2ad8ad11086bd`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:55:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:55:21 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:55:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:55:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 11 Dec 2020 14:55:29 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 11 Dec 2020 15:02:41 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 11 Dec 2020 15:02:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 15:02:43 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 15:02:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 15:02:43 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 15:02:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 15:02:57 GMT
CMD ["python3"]
# Sat, 12 Dec 2020 02:25:02 GMT
ENV HY_VERSION=0.19.0
# Sat, 12 Dec 2020 02:25:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Sat, 12 Dec 2020 02:25:08 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f38db61859bae698a1c0d931ac793156793ff0d6423c9c41f97325d4ae0125d`  
		Last Modified: Fri, 11 Dec 2020 15:34:43 GMT  
		Size: 2.5 MB (2485528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4627deec4d105c343b54ed0b7a9f0a763ce6fe847b1ddf3871b750b7f719d9bf`  
		Last Modified: Fri, 11 Dec 2020 15:34:44 GMT  
		Size: 10.0 MB (10003974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77329f47fc47e3dcf9728629907da36d0b9c03896d6b5dc6f5ea20e80910e773`  
		Last Modified: Fri, 11 Dec 2020 15:34:42 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5854986189cd0382510a69d5fb3410782ce99e1c547d47f47d3cefd228deec54`  
		Last Modified: Fri, 11 Dec 2020 15:34:43 GMT  
		Size: 2.4 MB (2419934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e846b8a70ddb5a901f3b16d6b3003a7852522a3bff2a38debe13906a6a023d50`  
		Last Modified: Sat, 12 Dec 2020 02:29:57 GMT  
		Size: 2.8 MB (2822600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm variant v5

```console
$ docker pull hylang@sha256:7e21138901c1411686a4bddd782fe628c1cea062cc251cfc90aa6bcf9791db59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38011002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4631f82acf378b73528a593103627768b7218af4caccf5915e410c0fc457759f`
-	Default Command: `["hy"]`

```dockerfile
# Fri, 11 Dec 2020 02:10:01 GMT
ADD file:aeadef1b764688b17f4ecd9d601a8f8f0fbcd69b5e2914c0dfa858244ca47082 in / 
# Fri, 11 Dec 2020 02:10:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 11:27:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 11:27:43 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 11:28:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 11:28:01 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Fri, 11 Dec 2020 11:28:02 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 11 Dec 2020 11:38:24 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Fri, 11 Dec 2020 11:38:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 11:38:28 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 11:38:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 11:38:29 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 11:39:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 11:39:04 GMT
CMD ["python3"]
# Fri, 11 Dec 2020 19:49:12 GMT
ENV HY_VERSION=0.19.0
# Fri, 11 Dec 2020 19:49:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Fri, 11 Dec 2020 19:49:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5079989477ba4f2a9ed6ef3b2c1d651c8ebc1291cd699d4c7c4bee28f5d09810`  
		Last Modified: Fri, 11 Dec 2020 02:19:04 GMT  
		Size: 21.2 MB (21202023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06b55d425d2a164ec177348926138ac5f129c80095ac1f2f88d2a7902eff328`  
		Last Modified: Fri, 11 Dec 2020 12:15:36 GMT  
		Size: 2.2 MB (2216227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1283bc1d87943609a292ef188c6a0b5d09f4c2e2f6976b80bd3cf904e080adeb`  
		Last Modified: Fri, 11 Dec 2020 12:15:38 GMT  
		Size: 9.3 MB (9349478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589d0aa2fb345befbc5df12b6a79b28e062ac72e784d6686215037390058efc7`  
		Last Modified: Fri, 11 Dec 2020 12:15:35 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e6b154bdcfee1a54acd5ffab5f95fd0b14fff81a55025ab4b85796785ef901`  
		Last Modified: Fri, 11 Dec 2020 12:15:36 GMT  
		Size: 2.4 MB (2419926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a1e189538841026ae57a64758bcb7f38d56fda61cdb4a8f4ab2957aef676ae`  
		Last Modified: Fri, 11 Dec 2020 19:51:39 GMT  
		Size: 2.8 MB (2823105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm variant v7

```console
$ docker pull hylang@sha256:b2d8f0020ce54ab8d02540798c3e8a886cda6e6fd8d8750922b74cf2f5f01a5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (35988692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762dbdb0003f835ef5ceb6fe5d84d198a0dcb455f354bcad6dc0714a9363fae8`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:23 GMT
ADD file:de081793a94d15fb89877812e1c838c9e3836070e36a6fb7f01b858a884b6680 in / 
# Tue, 17 Nov 2020 20:27:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:05:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 06:05:56 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 04:53:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 04:53:47 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 25 Nov 2020 04:53:48 GMT
ENV PYTHON_VERSION=3.7.9
# Wed, 25 Nov 2020 05:07:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 25 Nov 2020 05:07:13 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 03 Dec 2020 22:09:14 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Thu, 03 Dec 2020 22:09:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Thu, 03 Dec 2020 22:09:16 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Thu, 03 Dec 2020 22:09:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 03 Dec 2020 22:09:47 GMT
CMD ["python3"]
# Thu, 03 Dec 2020 22:35:25 GMT
ENV HY_VERSION=0.19.0
# Thu, 03 Dec 2020 22:35:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 03 Dec 2020 22:35:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a97dc136886474245bdc5c70c58e70e18fc55d193dae8225f0543e0b500b484a`  
		Last Modified: Tue, 17 Nov 2020 20:35:46 GMT  
		Size: 19.3 MB (19313228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f28fa623dfd2a6e8356a0f3f8e61dbda0dd0126be4813ee32cf2c77db86a251`  
		Last Modified: Wed, 25 Nov 2020 06:02:19 GMT  
		Size: 2.1 MB (2137495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb70d3bb8ec130b025ccb266decd782725ebf480555250e39081b0c4b197348a`  
		Last Modified: Wed, 25 Nov 2020 06:02:22 GMT  
		Size: 9.3 MB (9294785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19bd3d747902ec47c432634de09526401d9f7d91a7af64c3fdd89d5e487fb1d`  
		Last Modified: Wed, 25 Nov 2020 06:02:19 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6d81cec3bf4b74c1fbf4686df5ddf291ee802bc6a78441c406aea04e8d0b50`  
		Last Modified: Thu, 03 Dec 2020 22:16:55 GMT  
		Size: 2.4 MB (2420059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f69c7eeb4d266fbba51b1fc2442921ae14cc5ca8a5719ab5caf07970393c4`  
		Last Modified: Thu, 03 Dec 2020 22:39:32 GMT  
		Size: 2.8 MB (2822886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:2df31e71a79cd731d79e5a19d585e1237717af7e90d22d74b1458ddfabd33bc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37553826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20fda5612c358c43ee4131b38401c3469b5f6433aa7ea6bb32553ed3cf5c56b4`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Nov 2020 20:28:08 GMT
ADD file:b5b22f625d299254bffe6243b53eb5867cecdaab5c226e41411fa55763587755 in / 
# Tue, 17 Nov 2020 20:28:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 08:08:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 08:08:46 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 05:07:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 05:07:59 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 25 Nov 2020 05:08:00 GMT
ENV PYTHON_VERSION=3.7.9
# Wed, 25 Nov 2020 05:20:04 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 25 Nov 2020 05:20:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 03 Dec 2020 23:06:23 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Thu, 03 Dec 2020 23:06:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Thu, 03 Dec 2020 23:06:24 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Thu, 03 Dec 2020 23:06:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 03 Dec 2020 23:06:54 GMT
CMD ["python3"]
# Thu, 03 Dec 2020 23:26:08 GMT
ENV HY_VERSION=0.19.0
# Thu, 03 Dec 2020 23:26:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 03 Dec 2020 23:26:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f37c1cd284d6b059670ae5ae080ea2b30b095b4328a6580f4f0d90ef0da06b9a`  
		Last Modified: Tue, 17 Nov 2020 20:34:38 GMT  
		Size: 20.4 MB (20387780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fc7698caaf8f46094995e38c587dc46097d7fea1af3e51de4a22a384c2e8c4`  
		Last Modified: Wed, 25 Nov 2020 06:29:18 GMT  
		Size: 2.2 MB (2199094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9d3b143f7e75cd480e0464631cf89f66a43deb22ddf7e2039afc50e8761a77`  
		Last Modified: Wed, 25 Nov 2020 06:29:20 GMT  
		Size: 9.7 MB (9724159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd503f1f3e208614422f36a0ccf6dc1a17c8157fc49e534200dc976e09ffe0`  
		Last Modified: Wed, 25 Nov 2020 06:29:18 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca05c649b8a3414e6ef97ea9b27102af4cb2cd71e4b16bb04870210d14bf9c6`  
		Last Modified: Thu, 03 Dec 2020 23:13:51 GMT  
		Size: 2.4 MB (2419743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94584f1cefd2b63b4df0faf1cee60c11abe10071e9fff44b51eb6f6555501b5`  
		Last Modified: Thu, 03 Dec 2020 23:31:15 GMT  
		Size: 2.8 MB (2822808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.7-stretch` - linux; 386

```console
$ docker pull hylang@sha256:35f4b8bb930e2210b0411801859bd419f01007c7cb0f23e805ee5ee1be2804ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40978949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9d63828597f14d6c96839648704701231bc901cf55c7510aa09c4bf401dd31`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:25 GMT
ADD file:6d0d227a50cb77b9603ef598794fe0f583312a776daf61e7cd7e5493260354c9 in / 
# Tue, 17 Nov 2020 20:23:25 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 14:45:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 14:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 25 Nov 2020 03:54:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 03:54:15 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 25 Nov 2020 03:54:15 GMT
ENV PYTHON_VERSION=3.7.9
# Wed, 25 Nov 2020 04:04:56 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 25 Nov 2020 04:04:57 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 03 Dec 2020 22:54:41 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Thu, 03 Dec 2020 22:54:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Thu, 03 Dec 2020 22:54:42 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Thu, 03 Dec 2020 22:54:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 03 Dec 2020 22:54:58 GMT
CMD ["python3"]
# Thu, 03 Dec 2020 23:06:44 GMT
ENV HY_VERSION=0.19.0
# Thu, 03 Dec 2020 23:06:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 03 Dec 2020 23:06:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:657537e4548aa71eaa79344d36c62360306a66e11486f3d90ce21ecef49a62cb`  
		Last Modified: Tue, 17 Nov 2020 20:30:22 GMT  
		Size: 23.2 MB (23154739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295f99f03e3a70f4f97c169178779462aa052afe1a602a4d7b08cecd8e4413f0`  
		Last Modified: Wed, 25 Nov 2020 05:09:32 GMT  
		Size: 2.5 MB (2490127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a131aba37c670df78386727194eb11345e46adde39257e349085321805a3548c`  
		Last Modified: Wed, 25 Nov 2020 05:09:34 GMT  
		Size: 10.1 MB (10091784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7f8e5b1a0c65169b54517f3059623441db24853587c9c3ce4b5b260ab7656`  
		Last Modified: Wed, 25 Nov 2020 05:09:31 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84481fcae265aa8085467b2d7d8fd83a8910941737f5e9bffa9b66b3cb610`  
		Last Modified: Thu, 03 Dec 2020 22:59:30 GMT  
		Size: 2.4 MB (2419671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f80b21df42282c72eaa08061063165826cacec3742ef30ae931b7583bd57fb7`  
		Last Modified: Thu, 03 Dec 2020 23:10:15 GMT  
		Size: 2.8 MB (2822389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
