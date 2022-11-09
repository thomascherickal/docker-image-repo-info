## `hylang:python3.8-bullseye`

```console
$ docker pull hylang@sha256:9ffd5a8bf0615373836898987596e56f04ddd86af44baa8edebe2a95e225f305
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

### `hylang:python3.8-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:a1806163759d4e9a8c8f1cb71285c8ad58b2c8b72436ec1ecaef79502142e7b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50793325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20733b7ffb773c504285f07cdcfc074255fd8aef38fa02928e7f59041b0247c0`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:49:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:49:48 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:43:10 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 05:58:19 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 06:04:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 06:04:50 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 06:04:51 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 06:04:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 06:04:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 06:04:51 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 06:05:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 06:05:03 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:34:46 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:34:46 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:35:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:35:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d7f077cdde3b5e7290d1bb6bb3371c6b35ac75c5026770996f25dc83b2b27b`  
		Last Modified: Tue, 25 Oct 2022 06:28:53 GMT  
		Size: 1.1 MB (1077964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6fcd4d0fffbf4a76cfacf475c2f9a31eac7be5f0a752b0882e4cd4a0f60385`  
		Last Modified: Tue, 25 Oct 2022 06:30:46 GMT  
		Size: 11.3 MB (11337749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13386400aeba3426c7e2dfb017d4a66095fb76b10def05634748a056eb06b85`  
		Last Modified: Tue, 25 Oct 2022 06:30:44 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc68737bf83b9d2642fce6d33fe36ea5c6a31a743564717e8fee90c13c178a9a`  
		Last Modified: Tue, 25 Oct 2022 06:30:45 GMT  
		Size: 3.2 MB (3179097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1cc83b795b08ce8a2189cff9994f8f7e0ebcd4d4dc6b09beae8e1b31db9fb7`  
		Last Modified: Wed, 09 Nov 2022 00:48:45 GMT  
		Size: 3.8 MB (3778245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; arm variant v5

```console
$ docker pull hylang@sha256:9d8a2969807956431a7e76c5bedab7687fdd1faf80f418dc31d63f65813a2e89
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47809188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19a89064247faf431831c4f86bf02c1dffce0af38f8c2860c557726e79de2ced`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:35 GMT
ADD file:015ddb23f9ceec681c3a46b6d48671071fd41c5d56a957f6c96b50b1fc089a36 in / 
# Tue, 25 Oct 2022 03:06:38 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:38:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:38:41 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:38:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:40:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 04:57:25 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 05:04:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 05:04:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 05:04:38 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 05:04:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 05:04:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 05:04:39 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 05:04:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 05:04:55 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:50:05 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:50:06 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:50:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:50:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0df644382ba7fd23e9e4166ec2a03ec88b6cc5f640fb45413ecd913ceb901e41`  
		Last Modified: Tue, 25 Oct 2022 03:11:52 GMT  
		Size: 28.9 MB (28918513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761974b2df130b4c32168a51b6aa0b566a21afb7a0fe9b7846f7173d2735aef2`  
		Last Modified: Tue, 25 Oct 2022 05:24:32 GMT  
		Size: 1.1 MB (1060762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20a93edfbbd2f1bca62e634794bb139d0685797dbb48399138cdba4aab748a2`  
		Last Modified: Tue, 25 Oct 2022 05:26:39 GMT  
		Size: 10.9 MB (10874898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ccfefb037bfe689ccfe1d5bb798ce32cdad9fe8ccfe656b37ef92ca30f1bc6`  
		Last Modified: Tue, 25 Oct 2022 05:26:37 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a49bd6da630af9775e096a3e628d0eac74e91d5bb035e8b01c3ca8bf53f8fb`  
		Last Modified: Tue, 25 Oct 2022 05:26:38 GMT  
		Size: 3.2 MB (3178322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28423c0b5a9d0c96952e8b236af723e19530d16faf2c0f23371b3b7b17bb5d`  
		Last Modified: Wed, 09 Nov 2022 00:54:17 GMT  
		Size: 3.8 MB (3776459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; arm variant v7

```console
$ docker pull hylang@sha256:305465670ee6f625cd93b193b1444172b63bc3b28484bd2ba84e44de70430303
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45025662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a2e964d8eff9fe8e40e81e4741c14282d0ebed23f695006c4f25764e6daa06`
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
# Tue, 25 Oct 2022 08:37:44 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 08:45:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 08:45:41 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 08:45:42 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 08:45:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 08:45:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 08:45:42 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 08:45:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 08:45:55 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:10:34 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:10:34 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:10:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:10:50 GMT
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
	-	`sha256:67a8010cbb902ab6c4b36ab51a4908f711c4e2286be1fc936b92c24b03d623a5`  
		Last Modified: Tue, 25 Oct 2022 10:18:39 GMT  
		Size: 10.4 MB (10448556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b47094ab4b9f7f172f1f73e36de1bc6ac21227b30e4c42acd08ea72969cd7b`  
		Last Modified: Tue, 25 Oct 2022 10:18:37 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f84b3113392aa70a88fdb2710c1b0211e5cf658f0bca1c725820472c68a5190`  
		Last Modified: Tue, 25 Oct 2022 10:18:38 GMT  
		Size: 3.2 MB (3178359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9d5d8a4aa227c0ca401e410f6f6035e4c8d4257441625bac0f61431de16f5b`  
		Last Modified: Wed, 09 Nov 2022 03:26:11 GMT  
		Size: 3.8 MB (3776413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d3ccd37588e27925add707bfdb5463bb4ce93d629813a5413149ab796533b5f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49428773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f91c20bdd121e674cf4521868cdba485d2ec546cede353c44efafb15da07f8`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:57:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 05:57:56 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 05:58:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:43:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 06:54:09 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 06:58:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 06:58:31 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 06:58:31 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 06:58:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 06:58:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 06:58:31 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 06:58:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 06:58:41 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:55:50 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:55:50 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:56:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:56:03 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149b609701a9fb25662f582f94a02f17e630ef4a33376bd41acf4697907b015d`  
		Last Modified: Tue, 25 Oct 2022 07:18:13 GMT  
		Size: 1.1 MB (1065845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ecc40d89ab4ed978d8b83a788d2e3b7685bfef4d8ef09eb36c48d1c074e9ac`  
		Last Modified: Tue, 25 Oct 2022 07:20:01 GMT  
		Size: 11.3 MB (11341743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1193e462fc58472f23a9c2d93af919fa9915555bdaa60da9efd1225baa826c5b`  
		Last Modified: Tue, 25 Oct 2022 07:20:00 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af808f93ada1dbbebed9878ac8772e1bb7a4d58f56f763e3b4f7f8e9759b2da0`  
		Last Modified: Tue, 25 Oct 2022 07:20:00 GMT  
		Size: 3.2 MB (3178816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1f1e52f560062c32a11c9692aa15f2ed9d542de095a072e007d51a1c95b471`  
		Last Modified: Wed, 09 Nov 2022 01:09:10 GMT  
		Size: 3.8 MB (3778227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:81bb12b365c0aae015829b77d87fd96bc6ad16aff8e1c51c22c118576447330e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51435735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101d67806127c30f8abfd39874395edaac126cefbab9159a2c3d3d6dba12adc2`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:36:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:36:23 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 02:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:43:25 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 03:58:56 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 04:05:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 04:05:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 04:05:35 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 04:05:36 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 04:05:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 04:05:38 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 04:05:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 04:05:52 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:49:03 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:49:04 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:49:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:49:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e30e3c31efc1c2f0df5c6a661d62caa0fae09006043e85e75d4bec69baf3e1`  
		Last Modified: Tue, 25 Oct 2022 04:32:59 GMT  
		Size: 884.5 KB (884485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f60d98d07285e6a8b68ec0b8c5a318dc0fdd6c8c4135de2ef618fad5568cdbf`  
		Last Modified: Tue, 25 Oct 2022 04:35:19 GMT  
		Size: 11.4 MB (11416339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ce76b7838c276cb350f2ae97907a7f22f0402d10c3c2f8dd0ecbb4239a8ab7`  
		Last Modified: Tue, 25 Oct 2022 04:35:17 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e008a80d96573227f923e45f5e47a52ccb9e959802cdd8e70e4bdece968fdc23`  
		Last Modified: Tue, 25 Oct 2022 04:35:18 GMT  
		Size: 3.0 MB (2961602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d9e26b144adace92cf2bbaac53bcd96bbebb9d3826b3aa143aaa040503a5c3`  
		Last Modified: Wed, 09 Nov 2022 01:09:03 GMT  
		Size: 3.8 MB (3776693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; mips64le

```console
$ docker pull hylang@sha256:7daa52a28dbb671706bc6d414bb0ecc526c5586374803c572532c70e1017d873
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48428121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4732c576578ed6877a6f92ce87a84f5dfb42884b8060d2e8aab78a93fb6713b5`
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
# Tue, 25 Oct 2022 07:36:05 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 08:24:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 08:24:47 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 08:24:50 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 08:24:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 08:24:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 08:24:58 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 08:25:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 08:25:51 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:31:20 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:31:23 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:32:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:32:34 GMT
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
	-	`sha256:39c70bd9f0492c4397ae14bcc39967e1b3a93174ba68ca61c61968495b48301c`  
		Last Modified: Tue, 25 Oct 2022 09:16:54 GMT  
		Size: 11.2 MB (11202017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d99e26df415b930f66a1f03ebf3e7eb16d7863452593c40a1247b0f5ecfe807`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303b3f62bb1842d0ef967176068997d0d9fe7322cf18018f616467a5f81f57b0`  
		Last Modified: Tue, 25 Oct 2022 09:16:49 GMT  
		Size: 3.0 MB (2962620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709bffa0f78b60c3d020460174ab027f5fc924d7f7fee3dbba1198c8f537365a`  
		Last Modified: Wed, 09 Nov 2022 00:35:18 GMT  
		Size: 3.8 MB (3777053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; ppc64le

```console
$ docker pull hylang@sha256:259dd73dc6c56482e8058e9f120c59c843e9153d8240f3f3fa72f7d1c5dadfd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55042896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ded72a20d73dfb385e66188e53cb6d93ef23f6dd4b3ca867f506c803154e9c`
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
# Tue, 25 Oct 2022 05:13:11 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 17:24:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 17:24:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 17:24:52 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 17:24:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 17:24:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 17:24:53 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 17:25:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 17:25:16 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 00:40:11 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 00:40:12 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 00:40:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 00:40:48 GMT
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
	-	`sha256:1daad972a960cc7cd587dd0709add341fa467f18605f81906ee82af96cc40e44`  
		Last Modified: Tue, 25 Oct 2022 17:51:31 GMT  
		Size: 11.7 MB (11698847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e520fcca54360bfa03dbf349f2f6ce323d9ddbb610ae3dfbdc9403034dacd58`  
		Last Modified: Tue, 25 Oct 2022 17:51:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6732d3b331d47012b67d1fc29784c3f3d2a598c28d1166056449381d0bf3096a`  
		Last Modified: Tue, 25 Oct 2022 17:51:29 GMT  
		Size: 3.2 MB (3179208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0872ebf38e3f9224abf931cc97d6f36326b1b64cc9f0111d31a39f39352de24e`  
		Last Modified: Wed, 09 Nov 2022 00:53:34 GMT  
		Size: 3.8 MB (3778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-bullseye` - linux; s390x

```console
$ docker pull hylang@sha256:0931da838deb646db05249fe50f15df160c7e28148bb16a492914ca0c383dd16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48842957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c6d6e06ca18f9a658f5be6e6247cd3fd3324b45d6c4ebbbb2df9273a22ef1d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:42 GMT
ADD file:1bb8efa7f80e494b9d2831490a7e74810350c1f9ee2d100596d2e1cb4c62f529 in / 
# Tue, 25 Oct 2022 01:14:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:25:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 01:25:51 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 01:25:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 01:47:30 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 25 Oct 2022 01:53:20 GMT
ENV PYTHON_VERSION=3.8.15
# Tue, 25 Oct 2022 01:57:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 25 Oct 2022 01:57:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 25 Oct 2022 01:57:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 25 Oct 2022 01:57:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 25 Oct 2022 01:57:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6d265be7a6b5bc4e9c5c07646aee0bf0394be03d/public/get-pip.py
# Tue, 25 Oct 2022 01:57:46 GMT
ENV PYTHON_GET_PIP_SHA256=36c6f6214694ef64cc70f4127ac0ccec668408a93825359d998fb31d24968d67
# Tue, 25 Oct 2022 01:57:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 25 Oct 2022 01:57:56 GMT
CMD ["python3"]
# Wed, 09 Nov 2022 03:34:25 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 03:34:25 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 03:34:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 09 Nov 2022 03:34:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:abc14eb2518761d53b91fc564a31b657914f96b531f99a74ac8268f0717b007e`  
		Last Modified: Tue, 25 Oct 2022 01:19:01 GMT  
		Size: 29.7 MB (29650722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238d7a3937351f888bc695341ee2ecdfec34ecb7f9b2a4cbe690e7bdb800eeaa`  
		Last Modified: Tue, 25 Oct 2022 02:06:33 GMT  
		Size: 1.1 MB (1077352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff54cd9e6da9a740b1cc821970c0216c1266219cb6add08f505ac6627efbaa1`  
		Last Modified: Tue, 25 Oct 2022 02:07:45 GMT  
		Size: 11.2 MB (11157709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3192ef519574ab57fa3de56c6b8a5f581fff56d644e0f08550767c90acccc03`  
		Last Modified: Tue, 25 Oct 2022 02:07:44 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803c4a7c2da1ff5b55adca98e4cfbe2be580096cbc21a2fdeae17ad4cd0ed257`  
		Last Modified: Tue, 25 Oct 2022 02:07:44 GMT  
		Size: 3.2 MB (3178658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d15462eb662be3687276c853cc1e4cfc4efe9078641b8ed8768662f6f6bfe9`  
		Last Modified: Wed, 09 Nov 2022 03:43:21 GMT  
		Size: 3.8 MB (3778284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
