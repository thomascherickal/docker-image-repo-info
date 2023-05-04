## `hylang:python3.10-buster`

```console
$ docker pull hylang@sha256:829e632a84889601041ed2bb94e70a1b205cbe8db7690cdc37db3ae1b153be44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:python3.10-buster` - linux; amd64

```console
$ docker pull hylang@sha256:08e373d1e7c71960abbf88a7785276b561d4570c45f1d08ffc93845402dd9dbd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c6a7ed9595aff525a4bb613ecf5b986917fb47167ac2fba17ee05cb9683c0`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 00:20:26 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_VERSION=3.10.11
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 13:40:23 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 13:40:24 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 13:40:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 13:40:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25702e0699eca20ab682bbfa60f6bb7775e4fb18ef65c038ffda342fdab9e3a`  
		Last Modified: Wed, 12 Apr 2023 07:21:49 GMT  
		Size: 2.8 MB (2782083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf6e8027509be41b79122b1745365bd5c0c43586ce2976493dd69943d2d179e`  
		Last Modified: Wed, 12 Apr 2023 07:22:53 GMT  
		Size: 11.5 MB (11499177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68430a46d9dab42676a2ca1d8e9ae1ee8c6c19082a6bcece3e8e935231138a2`  
		Last Modified: Wed, 12 Apr 2023 07:22:51 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433875ea4139d286599691131e06d480b4b5c742a7558320f567f9789c097820`  
		Last Modified: Wed, 12 Apr 2023 07:22:52 GMT  
		Size: 3.4 MB (3370821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e7b5267dee90d0ecd3f7e815e079bb82591127ae208642d943bae54e38846c`  
		Last Modified: Wed, 12 Apr 2023 13:47:41 GMT  
		Size: 4.2 MB (4160084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:97fd321bff9fc986d93cc6aa5b6a2f08403d1a9da0276d6c76cd5ace732653a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43479654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb60b1ea591f3496089bf4d261f0f9f548d8033a554e3e115e0733e02973ad2`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:02 GMT
ADD file:72785c92abeacda7808e9e65787e604ed7fbc159c53eb4b2337628501418e9ce in / 
# Wed, 12 Apr 2023 00:00:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 00:00:02 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_VERSION=3.10.11
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 12:39:58 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 12:39:58 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 12:40:11 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 12:40:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2f777f2c33b3c8a258e4118224a280169c60be31db805388525da1f620f59a86`  
		Last Modified: Wed, 12 Apr 2023 00:03:58 GMT  
		Size: 22.7 MB (22747664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afcd873f81b90f3b0d383e4a6d01261410889219634980912c5e8b91c97718`  
		Last Modified: Wed, 12 Apr 2023 07:29:56 GMT  
		Size: 2.4 MB (2370024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02559042e7a6f75e54e22c3ee627f5005cc07b467a8d19719c8ec92993e335`  
		Last Modified: Wed, 12 Apr 2023 07:31:01 GMT  
		Size: 10.8 MB (10831364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d72a5266b78117ceabbf48eb1f9f765edabbfe0af8937de63a62ff094a188ed`  
		Last Modified: Wed, 12 Apr 2023 07:30:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f33c7287b70ea57df93f27a8a795a24627222060e17f12f812dc6bd72bf7d`  
		Last Modified: Wed, 12 Apr 2023 07:31:00 GMT  
		Size: 3.4 MB (3370149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6227bcc83db00be429792cef3d18e98312c82504f87ec8b17af3b46a058e5b4`  
		Last Modified: Wed, 12 Apr 2023 12:43:56 GMT  
		Size: 4.2 MB (4160209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:56787b6a31635350098547715a496d02fb63705ac2f9ae235ac63d2e52495ca1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47688188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf495fd2ecdfb79c4643208906503222de92fba94cee74a8949f9290b3d3b5de`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:02 GMT
ADD file:39d4ef5cc48487567b857a8527ab3c106b5099eafffbeaa8b70df450fb8409e3 in / 
# Wed, 12 Apr 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 00:40:02 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_VERSION=3.10.11
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 18:55:44 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 18:55:44 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 18:55:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 18:55:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:27bec964ec41cf69bd5df2ffd45c27623ae4bb0eb6f9f366179f7ac9b47d9840`  
		Last Modified: Wed, 12 Apr 2023 00:43:11 GMT  
		Size: 25.9 MB (25922011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348d3149d4c29a7c15853576f602f1e1b3ab3c1dde4c90efac6394e52c6682`  
		Last Modified: Wed, 12 Apr 2023 12:43:58 GMT  
		Size: 2.6 MB (2648723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7592c73d5b14aed211cfcf9ba7ff9a952f7f2f785e06d5cfa5ed797451334d33`  
		Last Modified: Wed, 12 Apr 2023 12:45:50 GMT  
		Size: 11.6 MB (11586750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587524b4e5aeba5d9872c2532761f4bfa9c96bad68c46a1303b15b144ea8e400`  
		Last Modified: Wed, 12 Apr 2023 12:45:48 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c978abf97f402d5507fabe5128996c288180d18d1f1bbdb55c905a4673699131`  
		Last Modified: Wed, 12 Apr 2023 12:45:49 GMT  
		Size: 3.4 MB (3370436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3b831f2086ab08f9a2a4fe4a0577e3fc5133d54ff8de3d069ec6712ea9216e`  
		Last Modified: Wed, 12 Apr 2023 19:02:31 GMT  
		Size: 4.2 MB (4160024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; 386

```console
$ docker pull hylang@sha256:8dfb30b62e4ce293615da1ea456f2f90b6c592f4902b6ff525df2a0eda3d75ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50184833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ac52191c1f589313c1d08deac23fb5901f767379ad78a942e982e18e83f4f73`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 03 May 2023 00:01:23 GMT
ADD file:b7d2995d8b654298ee7120d8293ac370802e2fda8c311516a581edef93d9e19f in / 
# Wed, 03 May 2023 00:01:24 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:01:24 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 00:01:24 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 03 May 2023 00:01:24 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_VERSION=3.10.11
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/0d8570dc44796f4369b652222cf176b3db6ac70e/public/get-pip.py
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_GET_PIP_SHA256=96461deced5c2a487ddc65207ec5a9cffeca0d34e7af7ea1afc470ff0d746207
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 03 May 2023 00:01:24 GMT
CMD ["python3"]
# Thu, 04 May 2023 02:04:50 GMT
ENV HY_VERSION=0.26.0
# Thu, 04 May 2023 02:04:50 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 04 May 2023 02:05:05 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 04 May 2023 02:05:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f1fd7e2201a19e853151f73eb8915b83c7c87b3dae495eef72019fecfbc76b3e`  
		Last Modified: Wed, 03 May 2023 00:05:57 GMT  
		Size: 27.8 MB (27797590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb40685373ebf7f4082c3c0f82a3ac9b6cf8333f6bf10a263492b1c21b8811`  
		Last Modified: Wed, 03 May 2023 08:40:45 GMT  
		Size: 3.2 MB (3236828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a8f27f21384c6789d858ce6c343c951d5c7fdb1557c56525d15d77de00c9e4`  
		Last Modified: Wed, 03 May 2023 08:43:41 GMT  
		Size: 11.6 MB (11618978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df83edcc1f3feac680413ce1a48ed047d29b0f75ad38c58c194ec52e1f88eb7e`  
		Last Modified: Wed, 03 May 2023 08:43:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843b50f30a63cff914094959bd37a58cbf79e706460ea4f54fbec679e779bdc3`  
		Last Modified: Wed, 03 May 2023 08:43:40 GMT  
		Size: 3.4 MB (3370775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f4079fd820fe415beb44ea2a2e6aed7d35714267719c6f14e167e201b790ce`  
		Last Modified: Thu, 04 May 2023 02:16:33 GMT  
		Size: 4.2 MB (4160418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
