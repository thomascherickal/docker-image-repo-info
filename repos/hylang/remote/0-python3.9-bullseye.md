## `hylang:0-python3.9-bullseye`

```console
$ docker pull hylang@sha256:c4668c8c21223a33324a38c21d419ecf73973bc4cf90946dbffccc9cf9282274
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

### `hylang:0-python3.9-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:1473b61949cddef43781466e68dd68b2b8b8f3f9811a74ef29bee69b68a80806
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50530281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9131016bb449848298dbaf2c2d042eca4e968dc6fe95e44ba2bbbee3fee861b9`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:09:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 14:09:04 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 14:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 15:46:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 15:46:16 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 02:45:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 02:45:44 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 02:45:44 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 02:45:45 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 02:45:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 02:45:45 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 02:45:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 02:45:56 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 03:29:40 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 03:29:40 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 03:29:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 03:29:54 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d9937f91c017aba99f0f612c832a63021706b0ebe3e2f1cf33c382135ad5fd`  
		Last Modified: Wed, 01 Mar 2023 16:33:19 GMT  
		Size: 1.1 MB (1076315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f85f51b17d5503d4d500800b104999fe309d8ac00c6df684e0177c9fb57db`  
		Last Modified: Fri, 17 Mar 2023 03:11:23 GMT  
		Size: 11.1 MB (11111125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c153184ac519506d6816629a9d801b311499f86054f6950ffddbfc2e0438163`  
		Last Modified: Fri, 17 Mar 2023 03:11:21 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c37649d3f36913775e2810ca8382dfbd98a8bb04985aec4ecb83360d5499f97`  
		Last Modified: Fri, 17 Mar 2023 03:11:22 GMT  
		Size: 3.2 MB (3195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca42281b4b30c3a0f4b45e8da5baa63c1aadac5f40ae6fe7194da73072dc7e4`  
		Last Modified: Fri, 17 Mar 2023 03:35:39 GMT  
		Size: 3.7 MB (3735658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; arm variant v5

```console
$ docker pull hylang@sha256:164e84370367241d23e2a98935cb6fc0420b2bdfad509ce26b3ea660a6d57e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47749858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2542d182cc481ba053bcbf1a0ac8222bf2d116334d90f0183c1d701652d5de`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:26:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 08:26:27 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 08:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:35:55 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 09:35:55 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 01:27:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 01:27:40 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 01:27:40 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 01:27:40 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 01:27:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 01:27:40 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 01:27:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 01:27:56 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 02:04:25 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 02:04:25 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 02:04:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 02:04:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4719092c5bc8220e9305fe499a72a7f5b64940eb648ad0604787ba4e15135e`  
		Last Modified: Wed, 01 Mar 2023 10:02:24 GMT  
		Size: 1.1 MB (1059621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b813da839c6db56795ec2ecf24c19ff0ff857218027f6b889a4236f8f0c656`  
		Last Modified: Fri, 17 Mar 2023 01:41:34 GMT  
		Size: 10.8 MB (10843577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce8ef86a41ff4c40b692f24e382425b976cd8e611880bb412729d383b7c7da3`  
		Last Modified: Fri, 17 Mar 2023 01:41:32 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fb6924be58a33e0f7630cb6eb310a52f0bfb436819e981bbbcf3ff7433ad4f`  
		Last Modified: Fri, 17 Mar 2023 01:41:33 GMT  
		Size: 3.2 MB (3195001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d9206fe4d321665229aae540a6a47d76b1bbbb14ae5bcae37c8c585414850d`  
		Last Modified: Fri, 17 Mar 2023 02:07:49 GMT  
		Size: 3.7 MB (3735649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; arm variant v7

```console
$ docker pull hylang@sha256:c5c17784a374defc3156ea3177516e2faedf4270a3978001c8ec029991b197c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44932749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0923fd652fb3964d404b98c8bd70804beac8f27cfbfe279996c73e440376ec8`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:28:28 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 12:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:28:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:51:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 14:51:44 GMT
ENV PYTHON_VERSION=3.9.16
# Tue, 14 Mar 2023 05:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 14 Mar 2023 05:28:39 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 14 Mar 2023 05:28:39 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 14 Mar 2023 05:28:39 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 14 Mar 2023 05:28:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Tue, 14 Mar 2023 05:28:40 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Tue, 14 Mar 2023 05:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 14 Mar 2023 05:28:54 GMT
CMD ["python3"]
# Tue, 14 Mar 2023 07:16:24 GMT
ENV HY_VERSION=0.26.0
# Tue, 14 Mar 2023 07:16:24 GMT
ENV HYRULE_VERSION=0.3.0
# Tue, 14 Mar 2023 07:16:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 14 Mar 2023 07:16:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af9b3c4eb38bb24a678196d8644743abcf256fde021a4dec6a02209c741df7`  
		Last Modified: Wed, 01 Mar 2023 15:46:39 GMT  
		Size: 1.0 MB (1041592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96649a548d9f9be3274ff5405c4212048616455293d27bc2f2b418fab9dbc1f`  
		Last Modified: Tue, 14 Mar 2023 06:54:16 GMT  
		Size: 10.4 MB (10435051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256aeba4e0ae26a1b129546d278e8707df9bb5e920dc3285490e829864f1c954`  
		Last Modified: Tue, 14 Mar 2023 06:54:14 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0315163c78b01f8389cf6a0bafdaabe302209e7eba01395fa16f8f7cd21b7572`  
		Last Modified: Tue, 14 Mar 2023 06:54:15 GMT  
		Size: 3.2 MB (3170821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdfa473464ac21031e13a118bc4552a9d26ae491eeaafd61e196f4ec8d937bf`  
		Last Modified: Tue, 14 Mar 2023 07:29:12 GMT  
		Size: 3.7 MB (3707761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:633e694c487b51b15db4da0027a43ebe0cc2439f6b239cf4bbabc28179cb8155
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49221500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56aade77aab1783a31e1a2ed36b25d07c9d8a6016b1a9a0803b88faf47aff31`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 10:01:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 10:01:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 10:02:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 11:41:43 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 11:41:43 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 03:10:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 03:10:43 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 03:10:43 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 03:10:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 03:10:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 03:10:44 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 03:10:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 03:10:54 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 03:51:46 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 03:51:46 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 03:51:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 03:51:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3ba05aa6dc6bcf7f4f57d5eaec80fd3edffbffde2e9727df29d63c978f0b99`  
		Last Modified: Wed, 01 Mar 2023 12:22:35 GMT  
		Size: 1.1 MB (1064143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf9f0b72d2789dec3d8defaaf38035c62e5c83286895a4c5f88fef99e1992e`  
		Last Modified: Fri, 17 Mar 2023 03:33:55 GMT  
		Size: 11.2 MB (11163451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2895efc607baf44bdb472b73e618a3d9334712e1d66fa743b50fa5c1a0d00573`  
		Last Modified: Fri, 17 Mar 2023 03:33:54 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59b2b6b4754ec1254893c9a9e96e4e95747272e1830c5417941a21bfaeb6b0e`  
		Last Modified: Fri, 17 Mar 2023 03:33:55 GMT  
		Size: 3.2 MB (3195251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1bd827e453216716194319114c8d475ea8057cd7d67175c016f5c8180dc292`  
		Last Modified: Fri, 17 Mar 2023 03:57:35 GMT  
		Size: 3.7 MB (3735607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:41e72289910a18b0d907f7db03a2cb95b99708d22f21e18d4ae447989c48ed5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51604784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627e1e1949e788282f8a352efa8437fdf1e4d2b513ac96d4084aebd389772713`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:14 GMT
ADD file:7ff48f7b36d13400120a726cd394769a4c39e8424877f5b080aeb9da07eacebe in / 
# Wed, 01 Mar 2023 01:39:15 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:25:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 03:25:42 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 03:25:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 06:27:41 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 06:27:41 GMT
ENV PYTHON_VERSION=3.9.16
# Tue, 14 Mar 2023 05:52:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 14 Mar 2023 05:52:16 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 14 Mar 2023 05:52:16 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 14 Mar 2023 05:52:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 14 Mar 2023 05:52:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Tue, 14 Mar 2023 05:52:16 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Tue, 14 Mar 2023 05:52:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 14 Mar 2023 05:52:31 GMT
CMD ["python3"]
# Tue, 14 Mar 2023 08:22:39 GMT
ENV HY_VERSION=0.26.0
# Tue, 14 Mar 2023 08:22:39 GMT
ENV HYRULE_VERSION=0.3.0
# Tue, 14 Mar 2023 08:22:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 14 Mar 2023 08:22:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2b884ef8a2d2b7c2016a8d2926b5b284f2130128ee049cae31a2da609cda7257`  
		Last Modified: Wed, 01 Mar 2023 01:44:44 GMT  
		Size: 32.4 MB (32396138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fa070e83c0acbfea4573d59d648116fe43215014c76a618c92c5423b466703`  
		Last Modified: Wed, 01 Mar 2023 07:43:50 GMT  
		Size: 1.1 MB (1088797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b5144ff0172a190e36f4d76e896eb55615cf4529a185061792ebff2e34e5cc`  
		Last Modified: Tue, 14 Mar 2023 07:47:18 GMT  
		Size: 11.2 MB (11240896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3ecfe2bde57e0585dafcc53d706ccf7540f441422876fa47bc5cbe992246e2`  
		Last Modified: Tue, 14 Mar 2023 07:47:15 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e03a1a522a349a51426313ef2c86e48ae3de08c31aab04a0c2a4a7b40bda94`  
		Last Modified: Tue, 14 Mar 2023 07:47:17 GMT  
		Size: 3.2 MB (3170908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995b8fa8f26d1db60a5992b3a92b5fed7c126c95b395a0efc2c13496dad62936`  
		Last Modified: Tue, 14 Mar 2023 08:36:32 GMT  
		Size: 3.7 MB (3707811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; mips64le

```console
$ docker pull hylang@sha256:5412d81677f42ea6003ded1e3400a7b613a2ad428b5438eae1cf0bf64a088530
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48267316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ac601a11e7fd5a97847696f0ae173fb01d1e4fce5699087bd7e12a34f7e802`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 11:28:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 11:28:52 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 11:29:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 11:29:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 11:29:19 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 02:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 02:55:06 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 02:55:09 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 02:55:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 02:55:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 02:55:17 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 02:56:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 02:56:17 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 04:15:20 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 04:15:23 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 04:16:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 04:16:33 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510f877c98026855aef7888e84a820a73eea05e4bf6e97fef57a13f03f42b456`  
		Last Modified: Wed, 01 Mar 2023 12:45:43 GMT  
		Size: 844.8 KB (844847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dcaf47d812835a019ecc18aa0138002aaf2dead491d878ce4188f419b951cc`  
		Last Modified: Fri, 17 Mar 2023 03:59:07 GMT  
		Size: 11.1 MB (11073694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c956876aa214ff5e88ab91a5fedd0d97c24d58bebf6d03be3f712c93797b7c0b`  
		Last Modified: Fri, 17 Mar 2023 03:59:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba43e27fc965c632bd4762cd0b2885b8893273085e95ffab449c48340e3a12`  
		Last Modified: Fri, 17 Mar 2023 03:59:03 GMT  
		Size: 3.0 MB (2980483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2924ad82b2bc54637c73fc42b272b710e5b0d25aaf006a1849afc4a29e0f301`  
		Last Modified: Fri, 17 Mar 2023 04:20:13 GMT  
		Size: 3.7 MB (3733571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; ppc64le

```console
$ docker pull hylang@sha256:ac23f0a0b1310fc554de2d6aecd664a9b886d95fd827b4e7ca7e5c12cb399ec9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54762815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9b9988a1ecd9e1f471fa582ad4a220f16b34ca35a019bf5b4aa119cef02735`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 11:23:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 11:23:11 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 11:23:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:32:57 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 13:32:58 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 03:50:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 03:50:53 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 03:50:53 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 03:50:53 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 03:50:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 03:50:54 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 03:51:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 03:51:24 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 04:55:56 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 04:55:56 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 04:56:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 04:56:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbec5187317d706e9b9249c96ba67e8c0f2b35a746b26dc54f69538723b5d789`  
		Last Modified: Wed, 01 Mar 2023 14:35:25 GMT  
		Size: 1.1 MB (1094703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea138c1e96e54ff60509dd2fadc847d055a9a3e7293a9893cc3d2f1a0701f3af`  
		Last Modified: Fri, 17 Mar 2023 04:26:24 GMT  
		Size: 11.4 MB (11447478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b30ea101f3c549d8ed0cde732c2b8275eed4a56f9288fd493cbc52df15bc7e`  
		Last Modified: Fri, 17 Mar 2023 04:26:21 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f640a32ea325d1a75926e1c1be6ef797c62e22bc5d1e184ef50263c8be7750`  
		Last Modified: Fri, 17 Mar 2023 04:26:22 GMT  
		Size: 3.2 MB (3196108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258e0273c38e9744b45006177d1260badd39159c59c0e1e21d7c972315f91878`  
		Last Modified: Fri, 17 Mar 2023 05:03:27 GMT  
		Size: 3.7 MB (3736188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bullseye` - linux; s390x

```console
$ docker pull hylang@sha256:48f2c99157832f30092b6eec6b343f76fff69b96a008b6fc9445902cc02d4e2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48686452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3576e7c2813be8bdb6bfe5e0481dd33439e84e042843ba9b0eef70b631f0ca72`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:31:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 05:31:43 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 05:31:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 06:13:30 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 01 Mar 2023 06:13:30 GMT
ENV PYTHON_VERSION=3.9.16
# Fri, 17 Mar 2023 02:38:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Fri, 17 Mar 2023 02:38:44 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Fri, 17 Mar 2023 02:38:44 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Fri, 17 Mar 2023 02:38:44 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Fri, 17 Mar 2023 02:38:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 17 Mar 2023 02:38:44 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 17 Mar 2023 02:38:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 17 Mar 2023 02:38:55 GMT
CMD ["python3"]
# Fri, 17 Mar 2023 03:08:35 GMT
ENV HY_VERSION=0.26.0
# Fri, 17 Mar 2023 03:08:35 GMT
ENV HYRULE_VERSION=0.3.0
# Fri, 17 Mar 2023 03:08:47 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 17 Mar 2023 03:08:47 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56317fef265c36d4ae3871856e6a4337a5bb43101089de813e2285c1d67ca8d2`  
		Last Modified: Wed, 01 Mar 2023 06:33:54 GMT  
		Size: 1.1 MB (1075793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c714add9ffc0446031c7ca54d27786c29a05c4f231fee4fe09ec9b816a4ddf27`  
		Last Modified: Fri, 17 Mar 2023 02:51:11 GMT  
		Size: 11.0 MB (11032596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d190aa11422d6504ff7ef6ed76bde27182fd4a536efd87365b47b1c5e9e7a0`  
		Last Modified: Fri, 17 Mar 2023 02:51:10 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b8762009cd81d5c5c18377bc01b70d3f7e226bec55273d5e12e16282fb82e`  
		Last Modified: Fri, 17 Mar 2023 02:51:10 GMT  
		Size: 3.2 MB (3195158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333c441e753f6ed11dde8ef088a27321b53163ca37b4bc87d631ec7514e58922`  
		Last Modified: Fri, 17 Mar 2023 03:14:11 GMT  
		Size: 3.7 MB (3735817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
