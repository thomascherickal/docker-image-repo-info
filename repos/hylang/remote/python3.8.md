## `hylang:python3.8`

```console
$ docker pull hylang@sha256:0c85d0d097065f162e3960af37b73ede1ac134ab10ca35b986761109707ae0ff
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

### `hylang:python3.8` - linux; amd64

```console
$ docker pull hylang@sha256:48dee58c2f356053fe51cf0c6c84571bb3c2f357bd73dc05eac427ebd6eefa92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49895061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f3e1f1d90b79cc01e63108f13fe650b52b7977d8d01c7a6fd065f18579972a4`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:25:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 06:25:15 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 06:25:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:56:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 11 May 2022 08:24:36 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 11 May 2022 08:30:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 11 May 2022 08:30:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 08:30:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 08:30:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 02:43:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:43:33 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:43:46 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:30:59 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:30:59 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:31:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:31:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7d81b69b9af8e7d8748b3d3ccc7a4dd28dd7752c0e118ad1f3238d3b5f1ee6`  
		Last Modified: Wed, 11 May 2022 09:14:18 GMT  
		Size: 1.1 MB (1076137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62672c31d041d50e7816447f409d7730a3e04603b73ffef93d94fc4337a6b5eb`  
		Last Modified: Wed, 11 May 2022 09:17:34 GMT  
		Size: 11.3 MB (11333465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d5da64eaf1f9f1c781761e80c9f35090af94b4de5111c9e8da10e9f0edc50`  
		Last Modified: Wed, 11 May 2022 09:17:32 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b1a9d0a8abc24358e0d1d381bbf1f4a374fbea3ec5a86d5fe1f62f0b799bbd`  
		Last Modified: Wed, 18 May 2022 02:51:42 GMT  
		Size: 3.2 MB (3169147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760f8b491e62fb15f725e5444a34bd142e8a5a548d26c0a523bb2e777c709c`  
		Last Modified: Wed, 18 May 2022 04:35:19 GMT  
		Size: 2.9 MB (2936603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm variant v5

```console
$ docker pull hylang@sha256:0313f7b1130fd3e715208e277c982286187665c51d3165c4879fea6b4f8c3c08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47059479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6b80bb0d4538eb437e4121cdf4f36b2a5cbff184bd43225f38228919d6609f`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 20 Apr 2022 07:16:42 GMT
ADD file:f20c57847025604e1ea1a848af3f090f71d78b5fc2eb2ac795822da94d6e6a0a in / 
# Wed, 20 Apr 2022 07:16:43 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:44:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:44:35 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 07:44:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:14:57 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 20 Apr 2022 10:48:40 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 20 Apr 2022 11:02:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 20 Apr 2022 11:02:48 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 20 Apr 2022 11:02:49 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 20 Apr 2022 11:02:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 20 Apr 2022 11:02:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 20 Apr 2022 11:02:50 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 20 Apr 2022 11:03:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 20 Apr 2022 11:03:24 GMT
CMD ["python3"]
# Wed, 20 Apr 2022 12:09:42 GMT
ENV HY_VERSION=1.0a4
# Wed, 20 Apr 2022 12:09:42 GMT
ENV HYRULE_VERSION=0.1
# Wed, 20 Apr 2022 12:09:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 20 Apr 2022 12:09:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3edd9d296fa023e00f76828c9d6fd6cc5b03e626341a6a045c40d2ea16c32d08`  
		Last Modified: Wed, 20 Apr 2022 07:32:27 GMT  
		Size: 28.9 MB (28921085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed2c1245eb96eda46a0e4192199cfc951892d840544587819e0579fb94e6a0e`  
		Last Modified: Wed, 20 Apr 2022 12:02:36 GMT  
		Size: 1.1 MB (1059438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a740096f3bff6f3445262d08667a1aec1535ea5b9ab2204b79687fd9d3a20ae`  
		Last Modified: Wed, 20 Apr 2022 12:05:54 GMT  
		Size: 11.0 MB (10973775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad824d6b00d4c75e26f91c1ae1b9af3ee6683d064fd1296b362b7a59a71c43b`  
		Last Modified: Wed, 20 Apr 2022 12:05:46 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357b1782940b2dc971bf1eb8d7b68f0125be0c0affae2ced9e2aa33ead7bf36b`  
		Last Modified: Wed, 20 Apr 2022 12:05:50 GMT  
		Size: 3.2 MB (3168837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2757d346a556681183a86687fe9603f7d39d0c99be3aa4e92cb13d90f739ebf`  
		Last Modified: Wed, 20 Apr 2022 12:14:10 GMT  
		Size: 2.9 MB (2936113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm variant v7

```console
$ docker pull hylang@sha256:9418e23f487876d3d956acf35cd9200a74472e94f1430824077938aaf8620dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44186612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8330b0f88725d186c927cc16f84462010a3b38f0bfbb3af7f484b706cce337be`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Wed, 11 May 2022 22:35:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 22:35:41 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 22:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 03:57:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 05:02:52 GMT
ENV PYTHON_VERSION=3.8.13
# Thu, 12 May 2022 05:23:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 05:23:47 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 05:23:47 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 05:23:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 12 May 2022 05:23:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 05:23:49 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 05:24:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 05:24:18 GMT
CMD ["python3"]
# Fri, 13 May 2022 04:31:28 GMT
ENV HY_VERSION=1.0a4
# Fri, 13 May 2022 04:31:29 GMT
ENV HYRULE_VERSION=0.1
# Fri, 13 May 2022 04:31:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 13 May 2022 04:31:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ff35074445b92acef69cb3d3e497aad5d1e536b01e937c800b0c7cc33714c`  
		Last Modified: Thu, 12 May 2022 07:41:57 GMT  
		Size: 1.0 MB (1041444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f701177cf8b7501c2883929070d39296b2e229fedb6947953460641ff169d3f8`  
		Last Modified: Thu, 12 May 2022 07:47:10 GMT  
		Size: 10.5 MB (10463580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44e3e0703f9c3a143d354f44fb1aebf383377cffc23deb3fb4b2564976a311`  
		Last Modified: Thu, 12 May 2022 07:47:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36ccbfb4b178a005b292a7f203691b963edf6da8a253e97c4e63584f7c345e0`  
		Last Modified: Thu, 12 May 2022 07:47:07 GMT  
		Size: 3.2 MB (3168845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f75ef16dabf1f2785a504cff5cc4435b4bd6d8c67f171e6be1ba315161cb7e`  
		Last Modified: Fri, 13 May 2022 04:38:58 GMT  
		Size: 2.9 MB (2936838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:81b7d8b59baa263b85e9bd2cb4ab33ad71b22aa6265d048bf1f81c9f9997c0d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48149341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cdd8f6ffd39572391bec873482e73c47581f95192f65e5dfe66905edf184faf`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:04:46 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 09:04:47 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:40:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 11 May 2022 11:01:46 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 11 May 2022 11:06:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 11 May 2022 11:06:23 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 11:06:24 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 11:06:25 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 04:40:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 04:40:19 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 04:40:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 04:40:31 GMT
CMD ["python3"]
# Wed, 18 May 2022 05:44:37 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 05:44:38 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 05:44:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 05:44:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d252b4015fa93dc9f330d813bf7ba931736380ec2d1388cfd347ebeac41de7`  
		Last Modified: Wed, 11 May 2022 11:49:01 GMT  
		Size: 858.7 KB (858739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7d489fad3d29945aa7ae03a70439ca5d9c52c08de98874e4182b5a1e8f03`  
		Last Modified: Wed, 11 May 2022 11:52:43 GMT  
		Size: 11.3 MB (11338186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb85d5bb0e0b7a1093c5d63f74b1e01779ba8d6d8a7c76f182771817ea1418f`  
		Last Modified: Wed, 11 May 2022 11:52:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2f5b7406b183e3c4319a498358b27d03cdd115addbeba28a1c6e0851dbe4d6`  
		Last Modified: Wed, 18 May 2022 04:51:30 GMT  
		Size: 2.9 MB (2949952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ab42f8d4a5fff0612e2d9454b5e5b57e57a1c67279ea61af876278a884fc2`  
		Last Modified: Wed, 18 May 2022 05:51:11 GMT  
		Size: 2.9 MB (2936538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; 386

```console
$ docker pull hylang@sha256:43203c9620dcdfe026265361ae8a1f1ef53fdf33959eef548e5be6e761c3fab7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50593975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22619fe83c232ee2ca1a5c59935f3b63aaee4a501ef7d02dfd27a222f529f558`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 11:29:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 11:29:08 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 11:29:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 13:28:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 11 May 2022 13:56:35 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 11 May 2022 14:02:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 11 May 2022 14:02:49 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 14:02:50 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 14:02:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:16:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:16:15 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:16:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:16:29 GMT
CMD ["python3"]
# Wed, 18 May 2022 03:48:07 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 03:48:08 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 03:48:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 03:48:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d4e66ce305f11bba31caa2a6b196dc77e429159c3e02a28602ea2231242a09`  
		Last Modified: Wed, 11 May 2022 14:44:18 GMT  
		Size: 883.4 KB (883398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f48beda2754af5a0289e7e62eec3af589e396cb046d4bb18007099dbcee26`  
		Last Modified: Wed, 11 May 2022 14:48:06 GMT  
		Size: 11.4 MB (11434340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cf1a9ba20424b54eda9b270a0ca0db2dea390c4457b0f0a3d866b1b63c777a`  
		Last Modified: Wed, 11 May 2022 14:48:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411f90457e56094e23a20cfa32bc0eb82a8d404d9a2b635b110f67eaab7a9542`  
		Last Modified: Wed, 18 May 2022 03:27:58 GMT  
		Size: 2.9 MB (2949717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498c03bb6962dd49aac4eb202b934cab5b21308e3d6311ba09d6592f04a08700`  
		Last Modified: Wed, 18 May 2022 03:54:57 GMT  
		Size: 2.9 MB (2936511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; mips64le

```console
$ docker pull hylang@sha256:d1238c861132d4a3f9ca8527b8020d67448959eb2f0badf7f54cd958ded802d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47574222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8636b87ccfec35de571ee607f4eceddd8b184013e0b4799685300c477d87b9e2`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Thu, 12 May 2022 06:03:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 06:03:16 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 06:03:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 14:04:42 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 17:25:48 GMT
ENV PYTHON_VERSION=3.8.13
# Thu, 12 May 2022 18:13:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 18:13:43 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 18:13:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 18:13:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 12 May 2022 18:13:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 18:13:54 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 18:14:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 18:14:48 GMT
CMD ["python3"]
# Fri, 13 May 2022 11:01:49 GMT
ENV HY_VERSION=1.0a4
# Fri, 13 May 2022 11:01:52 GMT
ENV HYRULE_VERSION=0.1
# Fri, 13 May 2022 11:02:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 13 May 2022 11:02:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3682a4f1ec34c9d2ab438032d66c3a2fa55157f7695e217fc1c22df851f4429f`  
		Last Modified: Thu, 12 May 2022 22:46:26 GMT  
		Size: 844.4 KB (844398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e97898c2e6347be8494d7ecb2a630f230a8280ef9d50c9b20b45cc6852273bb`  
		Last Modified: Thu, 12 May 2022 22:50:30 GMT  
		Size: 11.2 MB (11201120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b2bf029e5c2b77465f372423dda12091ef56c6832935ec3fb11f4f9eb90636`  
		Last Modified: Thu, 12 May 2022 22:50:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ac23c5e05bea83d9b84a4031c795483a70997c7d925d01b926ecdc7e68e47c`  
		Last Modified: Thu, 12 May 2022 22:50:26 GMT  
		Size: 3.0 MB (2950620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8fa5bfe2231af78ba2fdf8fbb337f65dbc9501c74d5961ef18af63004d9f0`  
		Last Modified: Fri, 13 May 2022 11:04:44 GMT  
		Size: 2.9 MB (2936799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; ppc64le

```console
$ docker pull hylang@sha256:4f1f1abffe63d36ae324be6ec7c80a845904ff96ab3148d055c01c98266c1bb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54181913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e8f4f842f9cf22102471b59e207a7a6d37e2a3f667c312d6001af964214ee4`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 21:00:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 21:00:05 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 21:00:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 00:43:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 01:50:57 GMT
ENV PYTHON_VERSION=3.8.13
# Thu, 12 May 2022 02:11:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 02:11:32 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 02:11:43 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 02:11:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Thu, 12 May 2022 02:11:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 02:12:00 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 02:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 02:13:03 GMT
CMD ["python3"]
# Thu, 12 May 2022 21:33:33 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 21:33:40 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 21:34:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 21:34:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980057956258174120e46894eca1d570f19e6c2ab3421c954c166aa8b1e40ce0`  
		Last Modified: Thu, 12 May 2022 04:10:34 GMT  
		Size: 1.1 MB (1094573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df5cde7de8240bb9167732f2003ed4816b937941d639ab763f92bb9f9a472c`  
		Last Modified: Thu, 12 May 2022 04:15:18 GMT  
		Size: 11.7 MB (11692218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348227ad4e20950670a2a3dd502a0a2936b0e44525f4e77ec3d8ee8a7fe6a8fc`  
		Last Modified: Thu, 12 May 2022 04:15:15 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9640691163919846befa8d3438420c73edf9e9e72112f36c6387f13932aa1e4b`  
		Last Modified: Thu, 12 May 2022 04:15:16 GMT  
		Size: 3.2 MB (3170846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2508fcc6f80727e3dad63b327efb4fa6c23175cd0c9e17d161e655bb1b5c83`  
		Last Modified: Thu, 12 May 2022 21:41:23 GMT  
		Size: 2.9 MB (2937575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; s390x

```console
$ docker pull hylang@sha256:c1d63d92ed61b0874bc75d57731a5e0fe0fb5de88cec810545dc8dba5ee29042
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47990235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bbb05a7d3a879303ee8389242ceefeed7de413c4eb002a67684d2db14646659`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:39:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 06:39:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 06:39:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:55:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 11 May 2022 08:15:28 GMT
ENV PYTHON_VERSION=3.8.13
# Wed, 11 May 2022 08:19:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 11 May 2022 08:19:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 08:19:59 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 08:19:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 18 May 2022 03:02:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:02:40 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:02:54 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:52:01 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:52:01 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:52:04 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:52:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b56df21812720343417b7387b2763aaa28b9a23746a67bc00c31a2fdd6f6c0`  
		Last Modified: Wed, 11 May 2022 08:55:52 GMT  
		Size: 1.1 MB (1075546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd52dbf212c168fa7866ed934cbd303bde1f2f26001eedbc75fc3874a70faf12`  
		Last Modified: Wed, 11 May 2022 08:58:20 GMT  
		Size: 11.2 MB (11154672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eae242dd2d1eb2fe0a05ae3501f4919b10780d21b5e7df5734295eb945d97c`  
		Last Modified: Wed, 11 May 2022 08:58:18 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0437f86b61478202d42451a4cadc4a67954e6efe0b4b6fb83f773da5b1ba8b6f`  
		Last Modified: Wed, 18 May 2022 03:12:58 GMT  
		Size: 3.2 MB (3168579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c734d2bbc3cf8ed553db02b1b19d1a743a181ce41fe3d44d4ae3869c51c494e`  
		Last Modified: Wed, 18 May 2022 04:57:25 GMT  
		Size: 2.9 MB (2936466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
