## `hylang:python3.9`

```console
$ docker pull hylang@sha256:bd334243b63dc05455bcf16cf64274d951818a3b1bb2dc1ec328cb76f3de7d49
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

### `hylang:python3.9` - linux; amd64

```console
$ docker pull hylang@sha256:8e708abb4345f3a0791dfdd184a86ae3c5dc312ebba227e373d18c0015f34b1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50976820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e55d6edea89e0afb98b3a74cc2d6cc34d98b84e2eaf84462873f1f83a7bc79bf`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 18:54:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 18:54:42 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 18:54:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 21:38:09 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Nov 2022 21:38:09 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 15 Nov 2022 21:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 15 Nov 2022 21:45:20 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 15 Nov 2022 21:45:20 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 15 Nov 2022 21:45:20 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 16 Nov 2022 06:57:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Wed, 16 Nov 2022 06:57:41 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Wed, 16 Nov 2022 06:57:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 16 Nov 2022 06:57:52 GMT
CMD ["python3"]
# Wed, 16 Nov 2022 07:35:29 GMT
ENV HY_VERSION=0.25.0
# Wed, 16 Nov 2022 07:35:29 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 16 Nov 2022 07:35:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Nov 2022 07:35:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00aaacf759c581712fa578a6b4e8e0b9fc780919a5d835a168457b754755644`  
		Last Modified: Tue, 15 Nov 2022 22:58:09 GMT  
		Size: 1.1 MB (1077982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50f75309cbe5622982b1b3b296361cb00825e87f028f0edef33b71c77e87f6a`  
		Last Modified: Tue, 15 Nov 2022 23:01:27 GMT  
		Size: 11.6 MB (11588493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea95839e7aaa8aa538343716153a70d50b051f9a258beac8bd6b9b4b8704f5a`  
		Last Modified: Tue, 15 Nov 2022 23:01:25 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bc4d5c5fdacbf12570ee2972996b9be8c89325fa61d77b1be803b441e58a7`  
		Last Modified: Wed, 16 Nov 2022 07:07:44 GMT  
		Size: 3.2 MB (3176567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e38eb5b618cd7193ab6716f35fb4b8771276a8ec198c612c2464d59bd3851`  
		Last Modified: Wed, 16 Nov 2022 07:45:43 GMT  
		Size: 3.7 MB (3720915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; arm variant v5

```console
$ docker pull hylang@sha256:ae57bf483feaba45d81dfff710b361484ef1d8bd97b504f50ff7bfc94f74e1bd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47961505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7097fbae6c1e0e43657c2cfc154c40c63c263f40b165222459db2517b34404e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:45:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 07:45:56 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 07:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:28:08 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Nov 2022 09:28:08 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 15 Nov 2022 09:35:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 15 Nov 2022 09:35:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 15 Nov 2022 09:35:28 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 15 Nov 2022 09:35:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 16 Nov 2022 00:34:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Wed, 16 Nov 2022 00:34:34 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Wed, 16 Nov 2022 00:34:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 16 Nov 2022 00:34:51 GMT
CMD ["python3"]
# Wed, 16 Nov 2022 01:07:14 GMT
ENV HY_VERSION=0.25.0
# Wed, 16 Nov 2022 01:07:14 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 16 Nov 2022 01:07:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Nov 2022 01:07:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a6e5b3ab314e2965853a4ddc03100cfb0fd0d2825cdc2fb4f1bc363cca39b9`  
		Last Modified: Tue, 15 Nov 2022 10:08:43 GMT  
		Size: 1.1 MB (1060732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3bf97a3f1d24ef3c317a4239629a23e487e535d4a1f174cbb35b724edfd618`  
		Last Modified: Tue, 15 Nov 2022 10:10:41 GMT  
		Size: 11.1 MB (11092558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3541569c674ee994d7cdcc2c6bf4172d29b701696d04d9fc5d98588d5b27b699`  
		Last Modified: Tue, 15 Nov 2022 10:10:38 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbcfeeb8136c7763ae102322e396b23d7bcfc814679c25a9fc95d2b424ff731`  
		Last Modified: Wed, 16 Nov 2022 00:40:51 GMT  
		Size: 3.2 MB (3175791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d912648e94ec38a47cbf58484d7c5099284c77ccbe9fc3e67cbbb43d938891c`  
		Last Modified: Wed, 16 Nov 2022 01:11:18 GMT  
		Size: 3.7 MB (3718066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; arm variant v7

```console
$ docker pull hylang@sha256:336d5bf833e75ebe58f7f7bfed50a993dd89874c581aa02511194f028df3db2d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45120819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef2df0e66f77973db752723aadba9b2504cc0238f776485e1f6bc56054c0107`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:06:28 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:06:28 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:06:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:50:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 07:50:47 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 25 Oct 2022 07:59:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 07:59:25 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 07:59:25 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 07:59:25 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 25 Oct 2022 07:59:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 07:59:25 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 07:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 07:59:39 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:08:58 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:08:58 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:09:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:09:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c3f1abf604fcfd2d98296c17bbfb654aaf261b67760acfc608f65727b1c03`  
		Last Modified: Tue, 25 Oct 2022 10:12:40 GMT  
		Size: 1.0 MB (1042809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0546504d9b1d0f529c2aa2cd899f8f12f1c8e56acd4aca780b7430d2bd51c6`  
		Last Modified: Tue, 25 Oct 2022 10:16:57 GMT  
		Size: 10.6 MB (10648598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24003300db6ed897f023149d48ec03a1bdf6ea9dc38a004a0e7c1b9263c0ba2e`  
		Last Modified: Tue, 25 Oct 2022 10:16:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c88fbe9a2a5382bbcd052140fbf2f0c56cfabbb267c5a83be21d6df50df323`  
		Last Modified: Tue, 25 Oct 2022 10:16:56 GMT  
		Size: 3.2 MB (3175915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f40fee561d641b482d8b584b0b5877749b7ea725d8065ff088a9d75060bfdb`  
		Last Modified: Wed, 09 Nov 2022 03:24:21 GMT  
		Size: 3.7 MB (3673971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:7a4728eb6fb59d63627cbf3fdf4fead192c854fbeef7ced78edf4ede658e78f1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49614675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ed2380e0b120613f2d6e99e9959e3edfc6c65ae0e5d81dfcfa113e21c0d78d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:41:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 07:41:31 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 07:41:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:55:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Nov 2022 09:55:06 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 15 Nov 2022 09:59:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 15 Nov 2022 09:59:54 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 15 Nov 2022 09:59:54 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 15 Nov 2022 09:59:54 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 16 Nov 2022 01:19:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Wed, 16 Nov 2022 01:19:59 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Wed, 16 Nov 2022 01:20:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 16 Nov 2022 01:20:09 GMT
CMD ["python3"]
# Wed, 16 Nov 2022 01:59:07 GMT
ENV HY_VERSION=0.25.0
# Wed, 16 Nov 2022 01:59:07 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 16 Nov 2022 01:59:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Nov 2022 01:59:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbd8719487c40bfcc7d42d53f202d1dbbbb7ac0fb4e4919ed791664b7f4e47b`  
		Last Modified: Tue, 15 Nov 2022 10:55:04 GMT  
		Size: 1.1 MB (1065870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d075b8f678bc7a1afae54847e43e1389ac7027754ee3db1687cc330255e83e`  
		Last Modified: Tue, 15 Nov 2022 10:58:05 GMT  
		Size: 11.6 MB (11590818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98dc5cb025b42d02464bfb57cd3733d24680e244cb98d0e5f669fce78291ff6`  
		Last Modified: Tue, 15 Nov 2022 10:58:03 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f8b51ed634cf27c6d602e36126aa4e9325664f9fc80bc5961788aa46ac6ce`  
		Last Modified: Wed, 16 Nov 2022 01:29:22 GMT  
		Size: 3.2 MB (3176270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4fefa50aabca1e071d0d097b12d64d5833d9fb34c5db4e32d7681c635e6595`  
		Last Modified: Wed, 16 Nov 2022 02:09:30 GMT  
		Size: 3.7 MB (3720879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; 386

```console
$ docker pull hylang@sha256:f47b721c76fe3036f2560c2d926c3b3ebf312ab2b910ea4cadf59a4c8a9e4f47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51616077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b694a7d2589b865a53f1094ea27f0e5eeec6c3adbe9d8e03fc60686b145b4161`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:57:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 12:57:11 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 12:57:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 16:12:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Nov 2022 16:12:54 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 15 Nov 2022 16:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 15 Nov 2022 16:19:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 15 Nov 2022 16:19:53 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 15 Nov 2022 16:19:54 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 16 Nov 2022 01:40:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Wed, 16 Nov 2022 01:40:58 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Wed, 16 Nov 2022 01:41:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 16 Nov 2022 01:41:13 GMT
CMD ["python3"]
# Wed, 16 Nov 2022 02:18:15 GMT
ENV HY_VERSION=0.25.0
# Wed, 16 Nov 2022 02:18:16 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 16 Nov 2022 02:18:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Nov 2022 02:18:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a4ead92cc7eae0396b0fbac1238e0bee3f677740a65a67474e08bcbaa003ba`  
		Last Modified: Tue, 15 Nov 2022 17:38:22 GMT  
		Size: 884.5 KB (884461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d9b05f241c85e973cec49fd1384d7e1e770d403a1c32e3c92a518055d1d395`  
		Last Modified: Tue, 15 Nov 2022 17:41:37 GMT  
		Size: 11.7 MB (11660735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad793bc8c97d59cbe6944c0b43d4364d1d1838c61f506f1804c7329bb76743`  
		Last Modified: Tue, 15 Nov 2022 17:41:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5f54f93403b2ac2d47b2d1835bd966138c34755893e116a43152661c1e6a6e`  
		Last Modified: Wed, 16 Nov 2022 01:55:11 GMT  
		Size: 3.0 MB (2959244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1925f6dcd6be47bff036ec790f1e1554b05dd03ca700439ab5854d8e68edc615`  
		Last Modified: Wed, 16 Nov 2022 02:34:14 GMT  
		Size: 3.7 MB (3718423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; mips64le

```console
$ docker pull hylang@sha256:e82b56d3b5f1e260bb29c9418f8da188e9a39eeadc8d9137a33453b41b330ca3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48575179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b1cc5c519c982f098cb030172f81106f7f6bed0cda5c289b979f827535b90b`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:43:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 05:43:44 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 05:44:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:48 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 06:40:50 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 25 Oct 2022 07:34:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 07:34:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 07:34:37 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 07:34:39 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 25 Oct 2022 07:34:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 07:34:45 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 07:35:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 07:35:43 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:29:53 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:29:56 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:30:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:31:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3080d7af0bacd81739264a89f5f4419d055a260eab400c2ded4bd862674a62`  
		Last Modified: Tue, 25 Oct 2022 09:16:25 GMT  
		Size: 845.6 KB (845609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024eb401443ab2d822304b7020b07a8d7e952b58e4b7074ca03c59f3b4e3fa94`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 11.5 MB (11454030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c799c1beba03f595a86f797fcfbc2bc4cd2c7c2e042376be36e1d8731b1265c`  
		Last Modified: Tue, 25 Oct 2022 09:16:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545c5926163f40fe2b15dd7c24a56b023252d0e1d1fb918d4e56fbfe82164dd`  
		Last Modified: Tue, 25 Oct 2022 09:16:27 GMT  
		Size: 3.0 MB (2960339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89edda14a2502836815b1385bea287f231a746310292ab6f18ab2cb23a31a8b`  
		Last Modified: Wed, 09 Nov 2022 00:34:58 GMT  
		Size: 3.7 MB (3674380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; ppc64le

```console
$ docker pull hylang@sha256:e727b6000cc4554b37497ad1f4990acde0e65f06790ecb009318eb3dd41e47bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55188059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc35a15777255c5883adaf11ae8ca53ab0a8f787191227ed5dcb9d61d3381684`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:29:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:29:25 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:50:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 04:50:44 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 25 Oct 2022 05:12:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 05:12:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 05:12:15 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 05:12:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 25 Oct 2022 05:12:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 05:12:16 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 05:12:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 05:12:40 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:38:03 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:38:04 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:38:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:38:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2d2456da999a2f483871184acad3d0038953e351e765a14f3082c03473cd9d`  
		Last Modified: Tue, 25 Oct 2022 05:17:20 GMT  
		Size: 1.1 MB (1096157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b62357bd7c2c5026f6010426ee0476cda435d8de83d6685a089c1d6247848db`  
		Last Modified: Tue, 25 Oct 2022 05:18:36 GMT  
		Size: 11.9 MB (11948910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52111a654f29536151573315e43fc2363992defeaa672c58a2bd34b56a6768cf`  
		Last Modified: Tue, 25 Oct 2022 05:18:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebadedd303797e8bff6f96ad191fc714bbeb48b9bc59ba54b33de3dd5b7f5a`  
		Last Modified: Tue, 25 Oct 2022 05:18:34 GMT  
		Size: 3.2 MB (3176809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61001c569e429f332afe422317a08d770ab7645fc99e18b848e9cfd6058788b8`  
		Last Modified: Wed, 09 Nov 2022 00:52:18 GMT  
		Size: 3.7 MB (3675865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9` - linux; s390x

```console
$ docker pull hylang@sha256:65f8c51914a26a9dc4e1e57f41828a3e734faaa1ac6d53d3e0aa80207ec6b7ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078e4db2972fcd236d0de6ddcd7eff8b45fd7dcd4c74ab07828675858c2ba5b4`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:52:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 10:52:16 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 10:52:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:21:36 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 15 Nov 2022 12:21:36 GMT
ENV PYTHON_VERSION=3.9.15
# Tue, 15 Nov 2022 12:30:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 15 Nov 2022 12:30:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 15 Nov 2022 12:30:42 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 15 Nov 2022 12:30:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 16 Nov 2022 00:50:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Wed, 16 Nov 2022 00:50:30 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Wed, 16 Nov 2022 00:50:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 16 Nov 2022 00:50:44 GMT
CMD ["python3"]
# Wed, 16 Nov 2022 02:29:41 GMT
ENV HY_VERSION=0.25.0
# Wed, 16 Nov 2022 02:29:42 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 16 Nov 2022 02:29:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 16 Nov 2022 02:29:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1487a90d7d45334f92d990a52e5750391ed66b11532972979f0792745cedca`  
		Last Modified: Tue, 15 Nov 2022 13:07:54 GMT  
		Size: 1.1 MB (1077428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895005c2f40ebaeb6c6de16fa6ba7d424b346d8ef4d1b940f61abc793d847f90`  
		Last Modified: Tue, 15 Nov 2022 13:09:56 GMT  
		Size: 11.4 MB (11385805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3511e04f8841e68e108462357972c07fd9321e60af998a35be97388f1c57167b`  
		Last Modified: Tue, 15 Nov 2022 13:09:54 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc61df5b4d9d4434b0610f448017d2424c3de4ab1ee797647f5ae886cc4f351`  
		Last Modified: Wed, 16 Nov 2022 01:01:09 GMT  
		Size: 3.2 MB (3176624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45fe15c6d07155fb54fe0c33fc73f6226100f0faee68364cd2af47bd19adb0`  
		Last Modified: Wed, 16 Nov 2022 02:41:11 GMT  
		Size: 3.7 MB (3721050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
