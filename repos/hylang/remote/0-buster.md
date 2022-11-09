## `hylang:0-buster`

```console
$ docker pull hylang@sha256:38e7b52975253131b4b56d16660c7bc588e830f7ff5a8f30a3c632f72d614840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-buster` - linux; amd64

```console
$ docker pull hylang@sha256:6c725ccbaabd7bb3eeabab4041fdb28eb651e16bc1c5c68e7c181941c36858b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51821913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd51b63c24cbae2e05deb9eb02cf02794499416ad2e7e07432e8253a07ba0d3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:04:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 05:04:59 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 05:05:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:05:05 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 25 Oct 2022 05:05:05 GMT
ENV PYTHON_VERSION=3.11.0
# Tue, 25 Oct 2022 05:19:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 05:19:48 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 05:19:48 GMT
ENV PYTHON_PIP_VERSION=22.3
# Tue, 25 Oct 2022 05:19:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.0
# Tue, 25 Oct 2022 05:19:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 05:19:49 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 05:20:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 05:20:02 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:31:29 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:31:29 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:31:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:31:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa89787764f0d8c8485166dfb4ff7f5ff2909fd336cb4391a9d6c064308ebe5`  
		Last Modified: Tue, 25 Oct 2022 06:29:19 GMT  
		Size: 2.8 MB (2781006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c23ee1bf76a31c08588b84e03d0b15c2a096de39dcefc336050dad2b0070`  
		Last Modified: Tue, 25 Oct 2022 06:29:21 GMT  
		Size: 12.5 MB (12476868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413d878c196c3bd3860c13017b2c232ab1c46aec1219e9395735a44e7f8f966`  
		Last Modified: Tue, 25 Oct 2022 06:29:19 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf767885ed216c2e135ad969c5a6dcbd76894c555b8d4a995c8893d7730e307`  
		Last Modified: Tue, 25 Oct 2022 06:29:20 GMT  
		Size: 3.3 MB (3345269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a654cc81b11ee4028775b6364ed76375fd4b68885812218d78991fa56239c96`  
		Last Modified: Wed, 09 Nov 2022 00:44:28 GMT  
		Size: 6.1 MB (6077704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:d54b1f63db1045b92863c2c9917bba60722ab18d6d8927e4869c4fdc446d1019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46131789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:257b086f8716db81e9f1af66d41eb28cd27ce765dcbaa3c97c5f15057997f825`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 03:15:00 GMT
ADD file:d3bb9b1f86a2639e67a7615e4d07996af61820f6d866ee4f6c5c8e5396da794d in / 
# Tue, 25 Oct 2022 03:15:00 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:54:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:54:25 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:54:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:54:36 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 25 Oct 2022 04:54:37 GMT
ENV PYTHON_VERSION=3.11.0
# Tue, 25 Oct 2022 05:17:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 05:17:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 05:17:49 GMT
ENV PYTHON_PIP_VERSION=22.3
# Tue, 25 Oct 2022 05:17:50 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.0
# Tue, 25 Oct 2022 05:17:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 05:17:50 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 05:18:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 05:18:03 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:06:09 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:06:09 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:06:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:06:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e4ea50bd37db50088d8cad765fade1138e096b0f83b40a13e3127931b49bab77`  
		Last Modified: Tue, 25 Oct 2022 03:22:12 GMT  
		Size: 22.8 MB (22750167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a076b1badbba9df89fc685a043044922797a850bb3a7a6c0026d0b98358c0ac1`  
		Last Modified: Tue, 25 Oct 2022 10:13:39 GMT  
		Size: 2.4 MB (2368343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa433cc48987352e199dfac9c2d278da0be687a854d957dda74c94cd20887e61`  
		Last Modified: Tue, 25 Oct 2022 10:13:41 GMT  
		Size: 11.6 MB (11594582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91ff31af71049baab991a7d388e4a7b6e99ce92279228eedcecb9a7195d367`  
		Last Modified: Tue, 25 Oct 2022 10:13:39 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408cc8c9e039541787c7333df884e33901ab38257bf51b7d9b3d8d9ea5b5091`  
		Last Modified: Tue, 25 Oct 2022 10:13:40 GMT  
		Size: 3.3 MB (3344576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a00b951fbe0df9137abc2c6dfa9d10de6b85a9effbf01453eae5638c913004`  
		Last Modified: Wed, 09 Nov 2022 03:20:15 GMT  
		Size: 6.1 MB (6073887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:2575901f60e48f89d527e75732ce7e4b3813d8a2cb56b1462d2e331c7a7715c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50470202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4238913111378d122623fb93fd431b1835474d5132dea86dc2a9b52dd726521`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:11:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 06:11:51 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:11:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:11:56 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 25 Oct 2022 06:11:56 GMT
ENV PYTHON_VERSION=3.11.0
# Tue, 25 Oct 2022 06:24:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 06:24:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 06:25:00 GMT
ENV PYTHON_PIP_VERSION=22.3
# Tue, 25 Oct 2022 06:25:00 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.0
# Tue, 25 Oct 2022 06:25:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 06:25:00 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 06:25:14 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:53:08 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:53:08 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:53:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:53:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9353727c2c340da2074ff7954456841315eaa1c1db324a467cc2cdb3d9af7c35`  
		Last Modified: Tue, 25 Oct 2022 07:18:39 GMT  
		Size: 2.6 MB (2646671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57302907a1e0c94cc733cd34f2e462ee467f08d6986f045c88a2da3c2b1c6d2b`  
		Last Modified: Tue, 25 Oct 2022 07:18:41 GMT  
		Size: 12.5 MB (12485397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23907d31e599dd9da47020b5d7a7dfdc7ea46604e0f278e911d60aaa75b1f47`  
		Last Modified: Tue, 25 Oct 2022 07:18:39 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010847120b630ebc00ec43655040454fd4d8c3452133b2588754d4d26f28fbc2`  
		Last Modified: Tue, 25 Oct 2022 07:18:40 GMT  
		Size: 3.3 MB (3344948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4847501edd75ff941a991e150f40d6d31998b65198399a789ab808401668d64`  
		Last Modified: Wed, 09 Nov 2022 01:04:59 GMT  
		Size: 6.1 MB (6078069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-buster` - linux; 386

```console
$ docker pull hylang@sha256:a56df806b60f707c94ced65610087a0a13d0b0b83c7915f945c3329868a7de42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52378106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f434317d08dc4aa7b3567b1fa6164af4b3be0af66208dec1cbf5956a9e5cbe7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:02 GMT
ADD file:49981fa4bc36bce6e4fdd74b2c4429cc4faef5498c3d8fb20fb98b426bbf8c4d in / 
# Tue, 25 Oct 2022 02:23:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:01 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 02:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:08 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 25 Oct 2022 02:56:09 GMT
ENV PYTHON_VERSION=3.11.0
# Tue, 25 Oct 2022 03:16:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 03:16:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 03:16:25 GMT
ENV PYTHON_PIP_VERSION=22.3
# Tue, 25 Oct 2022 03:16:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.0
# Tue, 25 Oct 2022 03:16:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 03:16:28 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 03:16:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 03:16:42 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:44:13 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:44:13 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:44:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:44:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:32caca2e9abac2a8ffc2b083d202d57e1970d8adc212be17451a992441fad01b`  
		Last Modified: Tue, 25 Oct 2022 02:29:19 GMT  
		Size: 27.8 MB (27799224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b76fbf13d4fc0083f4fb8571e3d89a1b8a6b8bdfeed8cab34bbaaf466696b9`  
		Last Modified: Tue, 25 Oct 2022 04:33:33 GMT  
		Size: 2.8 MB (2788348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a34ce81d1dfa2f1e4d31ee17398225835ea2cb5c324701ec0e5ef663cd610bc`  
		Last Modified: Tue, 25 Oct 2022 04:33:35 GMT  
		Size: 12.6 MB (12582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5c66dfcc267eca4f440ea7014f121129bf724472938cd247449f7419c4d72f`  
		Last Modified: Tue, 25 Oct 2022 04:33:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1442563dfc2cfd1d86729d50ef4d493a737364fc9f4cf45c89944834749e0bb`  
		Last Modified: Tue, 25 Oct 2022 04:33:33 GMT  
		Size: 3.1 MB (3132312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcf04fd22d0c99b56fa2d8f33683cc6bc09aa9fb809e5068f8a1b88b10bc43`  
		Last Modified: Wed, 09 Nov 2022 01:04:00 GMT  
		Size: 6.1 MB (6075580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
