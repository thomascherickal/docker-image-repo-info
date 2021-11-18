## `hylang:python3.8-buster`

```console
$ docker pull hylang@sha256:cccf6dabd313e9d064aeb4bafe30c72a3b9683ce035bbbcb1902f9bbcd3ff123
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

### `hylang:python3.8-buster` - linux; amd64

```console
$ docker pull hylang@sha256:59ab61763e651939d6f02dfa7479b66779c8ce617cfed784e825ce3154b04fc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46391195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f800e5b04802273ae85682aaa668051c789335f336b2f76312e632db7509c92`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:27:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:27:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:06:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 03:06:59 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 03:17:13 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 03:17:14 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 03:17:14 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 03:17:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 26 Oct 2021 23:50:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 26 Oct 2021 23:50:17 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 26 Oct 2021 23:50:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 23:50:29 GMT
CMD ["python3"]
# Wed, 27 Oct 2021 00:40:58 GMT
ENV HY_VERSION=1.0a3
# Wed, 27 Oct 2021 00:41:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 27 Oct 2021 00:41:03 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c44d634db0b14bf8679c170f6add62868c6df5e69e0b63c8fc3a247859d20c`  
		Last Modified: Tue, 12 Oct 2021 04:00:37 GMT  
		Size: 2.8 MB (2770140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9667f949f66d2ac5ec4830972842cd04eebbb378cc8521bafdb3961c7a2cda8d`  
		Last Modified: Tue, 12 Oct 2021 04:00:39 GMT  
		Size: 10.7 MB (10725735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f5c1d871efc0d134593e1022481d0f9c14d9d6c14102b7fa821c72781d4dc`  
		Last Modified: Tue, 12 Oct 2021 04:00:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181e9f84c7445a49dc8e0bfe46d33c7a3e942e773f3aa2fa856e69ea53a3e49`  
		Last Modified: Tue, 26 Oct 2021 23:59:59 GMT  
		Size: 2.6 MB (2637204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3aa980db5945a57c6d0ded8f74d42981124c18db04d630c882e8b3c6454ba0`  
		Last Modified: Wed, 27 Oct 2021 00:47:07 GMT  
		Size: 3.1 MB (3118373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:4080a760ff35a8bd3ceb99e3e617726775ce7e1f28bca18ce36b403382334ad0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43497142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0639d5c679ae65e9b7e120ba49aad9e8d30fdd86fb43384728da349764a76ca3`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:51:39 GMT
ADD file:e580d4d2066301375327ea51dd8db3af956e5a465495bf09d69d6deec9b0bfae in / 
# Wed, 17 Nov 2021 02:51:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 16:31:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 16:31:21 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 17:49:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 17:49:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 17 Nov 2021 17:49:53 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 17 Nov 2021 18:04:46 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 18:04:48 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 18:04:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 18:04:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 18:04:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 18:04:50 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 18:05:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 18:05:23 GMT
CMD ["python3"]
# Thu, 18 Nov 2021 02:20:16 GMT
ENV HY_VERSION=1.0a3
# Thu, 18 Nov 2021 02:20:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 18 Nov 2021 02:20:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dba255a4b166bb02562ca152d0da236ba8f211de5bf9d79e35ee023b1fce203e`  
		Last Modified: Wed, 17 Nov 2021 03:07:41 GMT  
		Size: 24.9 MB (24886310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce1603d3a96f1bba29f7e8f3c5f3e448e92001e18f589d62752052de948e393`  
		Last Modified: Wed, 17 Nov 2021 19:20:02 GMT  
		Size: 2.5 MB (2460703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa60943ac017f4c0cc1491e2a05f0c66430dd7510d412f07f3231ba919aa78`  
		Last Modified: Wed, 17 Nov 2021 19:20:07 GMT  
		Size: 10.4 MB (10394364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08940a43dcb9345d1ba9acac04609339793eeba113c619bd1ab4c27ed4f7b9c`  
		Last Modified: Wed, 17 Nov 2021 19:20:00 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae1e75462957820ead0655c26004292a9b3d20ef08a9467e35805b81f0d2b1c`  
		Last Modified: Wed, 17 Nov 2021 19:20:03 GMT  
		Size: 2.6 MB (2636841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67b2fbfaa26da2cea806abb6207830948fc0df6df95d3720303d1315291bf79`  
		Last Modified: Thu, 18 Nov 2021 02:26:16 GMT  
		Size: 3.1 MB (3118692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:f8af12d12feecd5adbb8a3eb4558d1c6226171a6933217892ccfec5b8ab2cc37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40791050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b3e5215e73d8ef7c9fd0c64c0666b45cdf62d32702f4ada50e57ab50fb916e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 14:38:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 14:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:07:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:07:20 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 16:07:20 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 16:26:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 16:26:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 16:26:05 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 16:26:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 03:41:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 03:41:01 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 03:41:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 03:41:29 GMT
CMD ["python3"]
# Thu, 28 Oct 2021 03:01:36 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 03:01:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 03:01:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f53a94afb1693ce51bceab3ba81983eb0311e1b230c67c857422abe1559baf0`  
		Last Modified: Tue, 12 Oct 2021 17:59:30 GMT  
		Size: 2.4 MB (2359017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed77bce9f0a80a2745deb1b7a27049a9a2c1800664ad16116b6df7bcb3d8da`  
		Last Modified: Tue, 12 Oct 2021 17:59:35 GMT  
		Size: 9.9 MB (9936645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9348c5224e266562cb4f5068038daa76f48fa0db93b4ca4f0bd06cc85781b125`  
		Last Modified: Tue, 12 Oct 2021 17:59:29 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7b88606e8c10812729ff4426b5ca6754f9b56ca2523e60db3cde6ac77ddd2d`  
		Last Modified: Wed, 27 Oct 2021 04:04:26 GMT  
		Size: 2.6 MB (2636788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b026a31495469b45ac0aebdeb321e1eb7d216a05d2f9886c9f6e4915f8b0c993`  
		Last Modified: Thu, 28 Oct 2021 03:14:04 GMT  
		Size: 3.1 MB (3118669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:b397c79843ad453d3d8807cc248634d7279a335f926006ef9ae2e27396da7001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44836210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cab2ee882ad7c58b9f1c558dec319ab2b6ba0d94dfe62d25541af7193c7419`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:08:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 12:08:48 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 12:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 12:39:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 17 Nov 2021 12:39:15 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 17 Nov 2021 12:44:39 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 12:44:40 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 12:44:41 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 12:44:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 12:44:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 12:44:44 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 12:44:59 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 12:45:00 GMT
CMD ["python3"]
# Wed, 17 Nov 2021 19:36:19 GMT
ENV HY_VERSION=1.0a3
# Wed, 17 Nov 2021 19:36:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 17 Nov 2021 19:36:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9944de13a6de6bc0bf97ba25f6fc4a8ac6db06ba872c81cb8f6db42f0dc7bc`  
		Last Modified: Wed, 17 Nov 2021 13:18:22 GMT  
		Size: 2.6 MB (2636100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e571701bc115cd2687e845662e43e8e48f36f3a680344acecc004bd847e90bf9`  
		Last Modified: Wed, 17 Nov 2021 13:18:24 GMT  
		Size: 10.7 MB (10732046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d91f36ecd9c17caf445647a1abdcc76558a0428e5341f17e4d21152daf0eff`  
		Last Modified: Wed, 17 Nov 2021 13:18:21 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f0f9af80a7d5116b240008f3993d86477bf182d0eb25ba16e97d5eae36d1fe`  
		Last Modified: Wed, 17 Nov 2021 13:18:22 GMT  
		Size: 2.4 MB (2426963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802396de30bd37089925a10f750ce75374b2f711da3a1ce35dd2d9e5d14c5ab`  
		Last Modified: Wed, 17 Nov 2021 19:43:11 GMT  
		Size: 3.1 MB (3117751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; 386

```console
$ docker pull hylang@sha256:969561a23d565d6417fed376ed2abefda2e0f210ff7ab0981c2328a43cfb09c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47182402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0978c324c4511b0b51388ece8f4f336ff46b73ae7c408c0a1986a3e248854f`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:22 GMT
ADD file:2adea3474b7ebda2bf77361304ee3e6966a9118aafd8220b81c4027be1f4d583 in / 
# Wed, 17 Nov 2021 02:40:22 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 16:14:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 16:15:00 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 17:17:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 17:17:55 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 17 Nov 2021 17:17:55 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 17 Nov 2021 17:30:22 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 17:30:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 17:30:24 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 17:30:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 17:30:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 17:30:24 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 17:30:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 17:30:39 GMT
CMD ["python3"]
# Thu, 18 Nov 2021 00:25:32 GMT
ENV HY_VERSION=1.0a3
# Thu, 18 Nov 2021 00:25:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 18 Nov 2021 00:25:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7af5c9e671306e395c50a515c7bbe33d6f418ea08535b01c884457f78114eb08`  
		Last Modified: Wed, 17 Nov 2021 02:48:49 GMT  
		Size: 27.8 MB (27804550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64405a9ae5f1f487f19f2d80e476d2f651d46c52c86e0c0ca7bb5a48b70afc61`  
		Last Modified: Wed, 17 Nov 2021 18:23:17 GMT  
		Size: 2.8 MB (2781503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf2cb712460a6a7a107c36a79acc1fdbbc2afed4d63aa4e7b8733b309b508bf`  
		Last Modified: Wed, 17 Nov 2021 18:23:16 GMT  
		Size: 10.8 MB (10840925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe69322546f21056b6116d006b22a4df50a50b429fe64f27023cd75e00030c`  
		Last Modified: Wed, 17 Nov 2021 18:23:14 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f576cbade45f5478371b8e76f548b29d2314c679831a994356c06ee1d9171021`  
		Last Modified: Wed, 17 Nov 2021 18:23:15 GMT  
		Size: 2.6 MB (2636715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d42dba33d1959cb8a977f2a2a11f251a3fc9f103e52783ecb07ea09094758`  
		Last Modified: Thu, 18 Nov 2021 00:32:57 GMT  
		Size: 3.1 MB (3118475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:482d359f26e0eff4b73438e47896afda045f9f9a6a1bdc0fbdbf3bd5e136dd6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44502551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d177cbb7615326e96707b4287ff25487444fca6e1397c23d7d1f9d3a4fa301`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:12:07 GMT
ADD file:a467fbf2015350da455cad98b5f5f247d88749cf317062ca09c466c27d53f87b in / 
# Tue, 12 Oct 2021 01:12:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:09:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 06:09:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:04:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:04:32 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 12 Oct 2021 12:04:33 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 12 Oct 2021 12:44:44 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 12 Oct 2021 12:44:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 12 Oct 2021 12:44:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 04:45:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 04:45:19 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 04:46:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 04:46:00 GMT
CMD ["python3"]
# Thu, 28 Oct 2021 00:16:23 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 00:16:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 00:16:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4d8cdee9d607e77b6f8c2203cc9cc02b38004def2b7fe162538c1538da10c870`  
		Last Modified: Tue, 12 Oct 2021 01:21:36 GMT  
		Size: 25.8 MB (25806535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b3f0a0c95842077ac80397ca7ffcb063c0b0846dde4d6f43daf33ea110bacd`  
		Last Modified: Tue, 12 Oct 2021 17:45:19 GMT  
		Size: 2.3 MB (2321420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce905852c6e37194cc90d84c3f4eb4a434b03d27e520b4b9a4175e47328dec69`  
		Last Modified: Tue, 12 Oct 2021 17:45:25 GMT  
		Size: 10.6 MB (10619362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e34f06620c2c70873163463dd8bc04a917373393680ab59da7c9a40340574`  
		Last Modified: Tue, 12 Oct 2021 17:45:18 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f175789834f4fa8bbd27f6a0aba6e0893cec4369da09e0d4c56594251b551d`  
		Last Modified: Wed, 27 Oct 2021 04:56:53 GMT  
		Size: 2.6 MB (2636490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319f2fb976a796b3483f4493f67833f3192d68b204c514b424f2f2b67f22b99`  
		Last Modified: Thu, 28 Oct 2021 00:19:57 GMT  
		Size: 3.1 MB (3118511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:68e3b8d962ebd1fe8efeba95e93c5cfcd7584a057ef9d7681a8d0b92d9088854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50724432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da74a7b28976e42145af3a02135546cd471548d71011b1957e88193f55b9187`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 03:30:22 GMT
ADD file:c0f8b5d4d419bef7a494df5330ecf7bbea3cbb6462308ca0b2f26771f125dea0 in / 
# Wed, 17 Nov 2021 03:30:29 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 16:49:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 16:49:24 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 18:54:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 18:54:56 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 17 Nov 2021 18:54:58 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 17 Nov 2021 19:13:09 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 19:13:15 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 19:13:18 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 19:13:21 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 19:13:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 19:13:30 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 19:14:06 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 19:14:08 GMT
CMD ["python3"]
# Thu, 18 Nov 2021 13:11:03 GMT
ENV HY_VERSION=1.0a3
# Thu, 18 Nov 2021 13:11:26 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 18 Nov 2021 13:11:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:459de0a111d5c931674a5150ef4ae6bb1ffb1685380f4aafdba04a37d556c5de`  
		Last Modified: Wed, 17 Nov 2021 03:58:14 GMT  
		Size: 30.6 MB (30562278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36e2af59f8575ccecd011f11536966b2c5abf77dd4c4aae2f0f00aa49399e24`  
		Last Modified: Wed, 17 Nov 2021 21:18:38 GMT  
		Size: 2.9 MB (2887555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae799b9a8db2fc45e4a78499fc09781481a62cc2173625791610ebc72b0ba9ee`  
		Last Modified: Wed, 17 Nov 2021 21:18:40 GMT  
		Size: 11.5 MB (11516849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49af0f775fd629dbb874c88b5f123af50afe8d21d448b228b15be5aa024bd94`  
		Last Modified: Wed, 17 Nov 2021 21:18:37 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50993f1b45cc6d25ad5a8b03b7abb9705ef87b4567ca0ef66832ddc090994282`  
		Last Modified: Wed, 17 Nov 2021 21:18:38 GMT  
		Size: 2.6 MB (2638427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcbe5f5f2ce114b47872ae4b9154fb1b4667e32da6cda046612d08a77bc35ab`  
		Last Modified: Thu, 18 Nov 2021 13:18:08 GMT  
		Size: 3.1 MB (3119090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; s390x

```console
$ docker pull hylang@sha256:808e28233fe5e1c5122c6d3fe73a35387834d527fe2e9f5c2bf1deaa08d72a34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44563373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311583296406aa5da9bbb082abd19b9a743e211ed309a4cd9dca9cbc70a2d4b`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:3ff5fbc9c53cf76aad0fe0e1a525cb0bc0d70e8f2a3d5741dfb8b3b8a9448ffd in / 
# Wed, 17 Nov 2021 02:43:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:28:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 07:28:30 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:12:12 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 17 Nov 2021 08:12:12 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 17 Nov 2021 08:17:01 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 08:17:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 08:17:03 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 08:17:03 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 08:17:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 08:17:04 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 08:17:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 08:17:14 GMT
CMD ["python3"]
# Wed, 17 Nov 2021 20:18:19 GMT
ENV HY_VERSION=1.0a3
# Wed, 17 Nov 2021 20:18:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 17 Nov 2021 20:18:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b8b917e61b3be882db10e68210f73caf5cc788bfb07aec0a659e30f4796b476b`  
		Last Modified: Wed, 17 Nov 2021 02:49:01 GMT  
		Size: 25.8 MB (25769063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67af14b94a5960bd0fd11a2afe4d97c0d5c8e7ac001f557f316fe3380b430a5f`  
		Last Modified: Wed, 17 Nov 2021 09:03:45 GMT  
		Size: 2.5 MB (2459485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219172cda15547e03584e6fbd55a3cd0f31d24e76611cc476b645456b64f2413`  
		Last Modified: Wed, 17 Nov 2021 09:03:46 GMT  
		Size: 10.6 MB (10579774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a835f0614878f35a30293d05995f3affbf2fca84e1105bfbba18d00e3942287`  
		Last Modified: Wed, 17 Nov 2021 09:03:44 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08c67e8f973ca6cb14a66910921cbc16c2dc2c251d243bd450b5d24653826e3`  
		Last Modified: Wed, 17 Nov 2021 09:03:45 GMT  
		Size: 2.6 MB (2636487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4262cac880de20f3466c8649b3d569a0d70d3123b120e38b8a70a166965ee6`  
		Last Modified: Wed, 17 Nov 2021 20:23:56 GMT  
		Size: 3.1 MB (3118330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
