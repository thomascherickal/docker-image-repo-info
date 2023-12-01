## `hylang:0-python3.8`

```console
$ docker pull hylang@sha256:df01981c9066ab3b3f326f9ad02207fddad896160feb2c1e67dbd4723b4c7017
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

### `hylang:0-python3.8` - linux; amd64

```console
$ docker pull hylang@sha256:147aa3629dcaf99d65a9eee562ea19c5ef4986f739bbe3cddd7845a34be0b872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52845430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a52ccfa33843b60d9722bd1ad926bfaa1fd3c313760f2bbd012ca30e4a11829`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:59:08 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:59:09 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:59:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:59:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442c5d63eafd969b755d7c8e0914319677ca8d5112a84e851b16677a4fc1d189`  
		Last Modified: Wed, 29 Nov 2023 06:26:10 GMT  
		Size: 3.3 MB (3315073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b64aefe47cbfa37759552a8864ab919a9b5a9687ef9089a8d27cb0b8e896df`  
		Last Modified: Wed, 29 Nov 2023 06:28:55 GMT  
		Size: 13.7 MB (13747993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5319590ca294258d4b2bcb339c05af534cdbc4879400b5c36b43ea2e3ff5eccc`  
		Last Modified: Wed, 29 Nov 2023 06:28:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef256e9b23e3a9de10cd933f658113bea148b1623f3b3b9749a5488a87a983ae`  
		Last Modified: Wed, 29 Nov 2023 06:28:55 GMT  
		Size: 2.9 MB (2929593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b210b55c532e4e1d7c6f6e6760c417a59554254292de7254b4fac90d7596b6`  
		Last Modified: Fri, 01 Dec 2023 20:06:53 GMT  
		Size: 3.7 MB (3702630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; arm variant v5

```console
$ docker pull hylang@sha256:5478151782e729a475991a203663ab1bc5ccc47e617da19333952efd0c796349
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49762773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cd5290058b126d11d86ec98edeb984ba94fca2615a848bd40c325ebe7156a2c`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:38:57 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:38:57 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:39:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:39:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5192ceb5c7aaf07109f91921011fdf22c93679916b01e8f7e0743a9893bd7512`  
		Last Modified: Wed, 29 Nov 2023 07:53:36 GMT  
		Size: 2.9 MB (2883057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b49c7c43c8ae5d0b1982346ae582efef15d6fdbefc5b495a3815feb0e78602`  
		Last Modified: Wed, 29 Nov 2023 07:55:22 GMT  
		Size: 13.3 MB (13325587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c0f2e35e0d717e23fd9498b985df26340533351330b03aa0e69fb21e39f06a`  
		Last Modified: Wed, 29 Nov 2023 07:55:21 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0cd9b1dcfbabb52ab0f42d71f66a7dfbc7797602a8eabeb3874534b09a6f40`  
		Last Modified: Wed, 29 Nov 2023 07:55:21 GMT  
		Size: 2.9 MB (2929203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd5dd8fc74b2de522afda8dc3e566919d96b3e95fa4a43b3cf9417dff5524af`  
		Last Modified: Fri, 01 Dec 2023 19:42:14 GMT  
		Size: 3.7 MB (3702540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; arm variant v7

```console
$ docker pull hylang@sha256:2f6cfbcc4a31a5c2af1706f5cf4a4c80120b45fa2cb99ea1177ce0a1c3ec5405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47030769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f00a68e0068521e7917f21988f6d53f17560e25a8fec1f4152606840541749a`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:53:14 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:53:15 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:53:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:53:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8036227e195be18eed6acb163b4c51732d0e0babb6ff01d02040111aa82008d`  
		Last Modified: Wed, 29 Nov 2023 10:11:15 GMT  
		Size: 2.7 MB (2718411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abc7fa3470d6d97b80f01dd403eb60f0504ba8c883de35b353f68a37ddc98d1`  
		Last Modified: Wed, 29 Nov 2023 10:13:56 GMT  
		Size: 12.9 MB (12931691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd8186b87b7a8e75c7be708a5b7f6db8980e8e320a502b00c6e661be7bcb2fb`  
		Last Modified: Wed, 29 Nov 2023 10:13:55 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801b7eb9c1337e1c13b5f0a92849a6867d87c70ce359526bb31fdcd6c89f1162`  
		Last Modified: Wed, 29 Nov 2023 10:13:56 GMT  
		Size: 2.9 MB (2928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef21f17b9f030e2b9b23031242578511f903ff2c2ba4b285502ec342000bc9ec`  
		Last Modified: Fri, 01 Dec 2023 20:00:43 GMT  
		Size: 3.7 MB (3702550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:ca86ce9ed267f405652db92189c0413fcb0e08a06788db0616ecd313b1cd8d5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52682201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297d46a00f126deb3d7c8d872470d12d686318850eb4ae2576918d86d6c84af9`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:20:08 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:20:08 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:20:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:20:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f2d5a72edf611dea7729627f20616bddc71a961e6f104cc6b3c5d62cfe3122`  
		Last Modified: Wed, 29 Nov 2023 05:41:14 GMT  
		Size: 3.1 MB (3132530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19e3d997f9c78c5829baeb8a50f604925d5ac3423d2bd4d8e8974345b9f92fa`  
		Last Modified: Wed, 29 Nov 2023 05:43:53 GMT  
		Size: 13.7 MB (13738133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85495d3e2cac01a9bc6f995a164f9d6a0dd354192fab6482992b424fabff748e`  
		Last Modified: Wed, 29 Nov 2023 05:43:52 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1006733521947c7d9438ed5102d32edcc23f1c331ef939442147fb3e2fed3b`  
		Last Modified: Wed, 29 Nov 2023 05:43:52 GMT  
		Size: 2.9 MB (2929589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f083a3ac9c33855bf72c57a773a254bdbf1923db1dd37650c63849a73d355d`  
		Last Modified: Fri, 01 Dec 2023 20:27:30 GMT  
		Size: 3.7 MB (3702439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; 386

```console
$ docker pull hylang@sha256:777c01346340d445380c705df825bff89f517ddd52abd28c77e06cafe322607c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54126324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22c3af44142617c4419e3951765e60d99a1964815e46e073957b31876b18aae`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:11:59 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:11:59 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:12:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:12:20 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f13291dffad304e24d83d00d2b24f51af580d92ea7a1047549b77860c8f1d51`  
		Last Modified: Wed, 29 Nov 2023 10:17:34 GMT  
		Size: 3.3 MB (3309977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17424c375a7d0847f45e0f0dcbebe75451cabf7841109fbe010db30d9b4d817`  
		Last Modified: Wed, 29 Nov 2023 10:20:26 GMT  
		Size: 14.0 MB (14020394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c5dc588c76df0b7ac73533e5401fa9bbb5ca4e63fc054b57797f676767c00f`  
		Last Modified: Wed, 29 Nov 2023 10:20:25 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5924166685e8f6b619a1e9d6101bbb1e91afc3f8862b69a106ce6efc9dd780ef`  
		Last Modified: Wed, 29 Nov 2023 10:20:26 GMT  
		Size: 2.9 MB (2929157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad86744fdccb443ad0c76f2cb041841c263e94611e5b9b996326b97287f97d93`  
		Last Modified: Fri, 01 Dec 2023 20:20:10 GMT  
		Size: 3.7 MB (3702455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; mips64le

```console
$ docker pull hylang@sha256:6c5578d1bd05b98c2dc6bb67b1c78da1f7626d6d946741912d2af91bb680b3a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52010362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdc794810b21c79c1ea756c25ad9f485e49dc16b0e9a080ba1cd43afafd5465`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:17:05 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:17:09 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:18:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:18:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2824ba78f6c9db19eead22ac09e1b17e9e6039512e67d5e32a007e0376337242`  
		Last Modified: Wed, 22 Nov 2023 06:56:21 GMT  
		Size: 2.7 MB (2707704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387add8ecff5c6f04563da68be2ab3bf3688a07a21d0babdc73207889e0fb8f5`  
		Last Modified: Wed, 22 Nov 2023 06:57:45 GMT  
		Size: 13.5 MB (13530512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913d27c796b1ba19034e8b0787fcbf3cc23cc88a632e1c3a197a90cd25688ea0`  
		Last Modified: Wed, 22 Nov 2023 06:57:38 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5170b162ecbd3e78c32ff06654396f217a751c58fb1d034845cfc25b1bb25b19`  
		Last Modified: Fri, 01 Dec 2023 19:55:52 GMT  
		Size: 2.9 MB (2929863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06edacddbbce31f080c0699d84eb66fd057ec0e776cc33263ac16c28b0855a9f`  
		Last Modified: Fri, 01 Dec 2023 20:20:52 GMT  
		Size: 3.7 MB (3700066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; ppc64le

```console
$ docker pull hylang@sha256:fbbdbafc7dfbaff2aa0ce4bfbb71ca59501f0932ec91ca7130789056a624d416
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57624494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3245b7e23d2df177808cb3486be4b7fd6179a357650804d9fdead29e90ad7976`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:58:58 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:58:58 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:59:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:59:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615de041661daf80c60e11281035c816244cd4dbf6fed45d2c7cdcdff4425741`  
		Last Modified: Wed, 29 Nov 2023 08:21:39 GMT  
		Size: 3.5 MB (3512709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd558cff1ca359691a13baf52d9046d0da8c5ff0f6530f1331c3e1da3bce84cf`  
		Last Modified: Wed, 29 Nov 2023 08:24:33 GMT  
		Size: 14.3 MB (14337125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dae8a19ac8eb231f19c0d8e36eba5b05252d8b4219645910046d6b811098b39`  
		Last Modified: Wed, 29 Nov 2023 08:24:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9b3501a072ee01b57b552e16dc654d29fa73cf5a258d665bee0bd3bd4606df`  
		Last Modified: Wed, 29 Nov 2023 08:24:32 GMT  
		Size: 2.9 MB (2930281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c1abb4334955eb37931e17fc6056fcce975bc39fefd35cca115b518b6448df`  
		Last Modified: Fri, 01 Dec 2023 20:07:23 GMT  
		Size: 3.7 MB (3702541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8` - linux; s390x

```console
$ docker pull hylang@sha256:1ef6cdcb0c1f0e75032565f70e8c8e00e23d0e4f414502362cca76b9ec8c66fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50781650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c990c0020f69c40ce649c91cdc7043880f6258f975907b07d52d2f55b647a1d`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 20:47:05 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 20:47:05 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_VERSION=3.8.18
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 20:47:05 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 20:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 20:47:05 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:15:32 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:15:33 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:15:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:15:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48722dfee7273d665d1953dd9e7594d512a38f3156ed97136a9b64104472724`  
		Last Modified: Wed, 29 Nov 2023 06:23:12 GMT  
		Size: 3.0 MB (2974364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7bb1ffd2284705f349f7434f10cf164dd0966a40b27bc95d5f1359bfb6d1d3`  
		Last Modified: Wed, 29 Nov 2023 06:25:34 GMT  
		Size: 13.7 MB (13662774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c33049c719427b9427ae82e515f014ecdb3367a45060ebc8e43e3016c43162`  
		Last Modified: Wed, 29 Nov 2023 06:25:33 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12f62318d35e0117f48937ce1c4f4d17f1d6fa229ef50eb7189c65b8752c4f`  
		Last Modified: Wed, 29 Nov 2023 06:25:34 GMT  
		Size: 2.9 MB (2929163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc0b21b1bea2b0ca419db16a1b4b77ba6eba50c7b245cab134236c09a3d898e`  
		Last Modified: Fri, 01 Dec 2023 20:21:06 GMT  
		Size: 3.7 MB (3702231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
