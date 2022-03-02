## `hylang:python3.8-buster`

```console
$ docker pull hylang@sha256:358fcfc72b87270fd1b9ac888e4e0890d293febdbaf58862f71c7a99a1b01c61
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
$ docker pull hylang@sha256:24ce23c81f59f0a59aa4aa39e5d14f1d1e49c039e6a9404739d628c56bc355f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45869009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfc83ccf1593d56d7329f9cb5b2c256f42758dea4f954850bcb7a0b9f6dbacb`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 20:36:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 20:36:00 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 20:36:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:15:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 05:26:04 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 00:34:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 00:34:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 00:34:24 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 00:34:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 00:34:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 00:34:24 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 00:34:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 00:34:36 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 02:50:11 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 02:50:11 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 02:50:15 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 02:50:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4887dad22fda8ead06b653271b8a6fde0f36b5d8aaa804f12f79a0fef138de5`  
		Last Modified: Wed, 26 Jan 2022 22:34:52 GMT  
		Size: 2.8 MB (2770186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23c272deba62327d1980dead8630984a05b0058baffd8363236a1e0692266a5`  
		Last Modified: Sat, 26 Feb 2022 01:55:25 GMT  
		Size: 10.7 MB (10728704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7085100acf3523088a2adf4a3381c1696c68f63af73427730333a0b39c0c5e4`  
		Last Modified: Sat, 26 Feb 2022 01:55:22 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc542d1460c40e995056622dd915b11c66ace58dabba79599218e6939f1ad3d`  
		Last Modified: Sat, 26 Feb 2022 01:55:23 GMT  
		Size: 2.6 MB (2636558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b91c727908e947b5fe51c360df6bfb2ff01aee4961d880ae774ad4871dd78d`  
		Last Modified: Sat, 26 Feb 2022 02:55:15 GMT  
		Size: 2.6 MB (2579589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:65f3ec74540ac081b7a645a62a6772a7e8e038b43f3816a31ffa093b37a8d045
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42957002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ca4164ccb50caeb3ed3c47dec90a7f6945accfcddb2f43ad251d6c83902998`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 18:13:37 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 18:13:37 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 18:13:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:36:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 22:35:39 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 22:50:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 22:50:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 22:50:30 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 22:50:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 22:50:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 22:50:32 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 22:51:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 22:51:04 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 14:58:26 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 14:58:26 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 14:58:33 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 14:58:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1812dca044a6fc378d00f59bd6b41dde5387808cc2f1dc9155398ed2678760`  
		Last Modified: Wed, 02 Mar 2022 00:13:08 GMT  
		Size: 2.5 MB (2460696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadb079814f178cc1b879018c05e7f9211c23f73415cf9efad28c64f731b1171`  
		Last Modified: Wed, 02 Mar 2022 00:18:44 GMT  
		Size: 10.4 MB (10394125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a08772e16c8ce57285554c68b968d5f1ee4aa1d634f25816be15974c4064df`  
		Last Modified: Wed, 02 Mar 2022 00:18:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc28024f06a4538b571ad4535d20a647c46d531b9492e7384befb0b72afa158b`  
		Last Modified: Wed, 02 Mar 2022 00:18:41 GMT  
		Size: 2.6 MB (2635953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca05ef0cd14d3d6ef167a599a9167bc2f5df2b69866f76b98301794a7922a9`  
		Last Modified: Wed, 02 Mar 2022 15:03:40 GMT  
		Size: 2.6 MB (2579765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:24422bbe98eec3dc01a332ab0078e868e3d5dd34863ecd7ccca0629ecc96de63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ee82212c62322b9a55215802fe5261656eb3e8dda491a5591a8c62e5dabc45f`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 20:37:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 20:37:11 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 20:37:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:14:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 10:39:16 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 06:25:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 06:25:07 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 06:25:07 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 06:25:08 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 06:25:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 06:25:09 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 06:25:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 06:25:37 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 09:58:56 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 09:58:57 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 09:59:03 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 09:59:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f32624e5e559ac5a8f1bb77f6a911c89c41aa160f211c42ca2c48ce4ec9d41`  
		Last Modified: Thu, 27 Jan 2022 01:35:50 GMT  
		Size: 2.4 MB (2359014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ea5b037e995d7e606172325c2c514d7881ed36f506abced21612e20e96803d`  
		Last Modified: Sat, 26 Feb 2022 09:07:59 GMT  
		Size: 9.9 MB (9936349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66155e1289ca56c503ff62c603d35da010e9c5b9bf04eba01bf50e54c805f6d9`  
		Last Modified: Sat, 26 Feb 2022 09:07:53 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096f1936b97dbb4c2d98ca55ec5c74d3da09d69758337d4cd76f0ca2e80bbd9d`  
		Last Modified: Sat, 26 Feb 2022 09:07:55 GMT  
		Size: 2.6 MB (2636030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ccb7f0c12070fcab25bf1e8007ad73f9f7a29d30cbe18b6f5899f4fc43e74`  
		Last Modified: Sat, 26 Feb 2022 11:48:36 GMT  
		Size: 2.6 MB (2579741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:e7f527b64b5d0d9a2b8b63d0af7f6fc71dff39ce6da52a26bdd8651e0ce9f95d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44296663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54bf9c648f0adaf5bfbdd2348ca7d4ed4c64d3ef05c1936f59d9737ef861e9c7`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:47:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 19:47:24 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 19:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 20:58:13 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 21:19:30 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 21:24:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 21:24:22 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 21:24:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 21:24:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 21:24:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 21:24:25 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 21:24:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 21:24:38 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 15:35:21 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 15:35:21 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 15:35:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 15:35:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d2ad45cad19756f963eafcc80d7f87fbe4ac96f5fce0a6afe21e83af6fb45`  
		Last Modified: Tue, 01 Mar 2022 21:57:33 GMT  
		Size: 2.6 MB (2636110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5e7e852b7596ec07874029e3f250f258b4ae2d19ab265e67735e0976b74a39`  
		Last Modified: Tue, 01 Mar 2022 22:01:15 GMT  
		Size: 10.7 MB (10735271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdba4da0515d767c555fbb4151d5b6fa1baec306c25b07a16c02d24b5e3a3a5`  
		Last Modified: Tue, 01 Mar 2022 22:01:13 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3de83a89b14b1bb2a3ab3ec1362bce2c379a68830df1e3660cd5cbd3c2306d`  
		Last Modified: Tue, 01 Mar 2022 22:01:14 GMT  
		Size: 2.4 MB (2424444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb38209744ea17d66130c2dd54537380a0b50338e3a3737dd0b5d03f35ca6755`  
		Last Modified: Wed, 02 Mar 2022 15:40:39 GMT  
		Size: 2.6 MB (2577462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; 386

```console
$ docker pull hylang@sha256:5b6f4605ff250fbda044ca0b7e84245919ad10d872b03e039167eca1c9909c3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46641217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de530c8c0dc8de10672835f7c7b833c4334665ef3380ba586fd931b85e50eee`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 23:00:37 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 23:00:37 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 23:00:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 01:03:33 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 02 Mar 2022 01:34:54 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 02 Mar 2022 01:45:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 02 Mar 2022 01:45:45 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Wed, 02 Mar 2022 01:45:45 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 02 Mar 2022 01:45:45 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 02 Mar 2022 01:45:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Wed, 02 Mar 2022 01:45:45 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Wed, 02 Mar 2022 01:46:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 02 Mar 2022 01:46:01 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 09:33:17 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 09:33:17 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 09:33:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 09:33:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3732310af3a21f79d28ad07be855cf934da0caadc03263a18b52b7b0a94c0d6`  
		Last Modified: Wed, 02 Mar 2022 02:39:02 GMT  
		Size: 2.8 MB (2781563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c5d038b4af3c35d4de1e26d0ff8224393124bd9fd35c286903732f7df864a5`  
		Last Modified: Wed, 02 Mar 2022 02:43:09 GMT  
		Size: 10.8 MB (10839139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088c5c23e8db079c72eeb4ea7da590cc378bdda2f752daf778bbdb78d3d898e`  
		Last Modified: Wed, 02 Mar 2022 02:43:06 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6975ac5e44c92aafbf307fd05f5d6bb34dde38897971c7efc1e3c4e38bf5906`  
		Last Modified: Wed, 02 Mar 2022 02:43:07 GMT  
		Size: 2.6 MB (2636096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9021c9ab32d2c76906b429057ed81b8c2580a09f84cc157c6e8c594a0ae42ece`  
		Last Modified: Wed, 02 Mar 2022 09:39:32 GMT  
		Size: 2.6 MB (2579595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:83daf89b59bd2bb6b1f66ec6e4a32d50993a92eac221c4074751a2a0704d5025
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43980773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e248281036e5b99f118ed28ec33306d5fe3cb18e43e6971099f275a559b4c770`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:36 GMT
ADD file:b2143098bd05f6236a82c9b6af4be48c891bbf2fa7173ce2b1861a35662888e3 in / 
# Wed, 26 Jan 2022 01:43:37 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 05:02:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Jan 2022 05:02:43 GMT
ENV LANG=C.UTF-8
# Thu, 27 Jan 2022 05:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 05:03:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 13:20:21 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 06:37:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 06:37:38 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 06:37:38 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 06:37:39 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 06:37:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 06:37:39 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 06:38:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 06:38:20 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 09:45:27 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 09:45:27 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 09:45:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 09:45:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:242530af5dd081cf94e328c4f8df0c53e28e53a9f2da9733e46d21f187b2b727`  
		Last Modified: Wed, 26 Jan 2022 01:52:48 GMT  
		Size: 25.8 MB (25820216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a509dc22b79d4a00bf97a49dcf21dfabb069c2d5cc6bdbaca7c81e22a8684547`  
		Last Modified: Thu, 27 Jan 2022 11:24:04 GMT  
		Size: 2.3 MB (2321407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e4cc5a484e15efef179b3118eb063c65e35d77900e1ada79c0157a1663ab46`  
		Last Modified: Sat, 26 Feb 2022 09:27:32 GMT  
		Size: 10.6 MB (10625001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1bd733b21e5006ea34752b8faf641e93d94520b2f4305929dfbaf9c5176a2d`  
		Last Modified: Sat, 26 Feb 2022 09:27:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139c430bf5781431544778f4bae21472b76bf39ffbef0fc86eca52cd0f7aa0e`  
		Last Modified: Sat, 26 Feb 2022 09:27:28 GMT  
		Size: 2.6 MB (2635801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d488d669cdae5e10a0a711a60b760e1bee7dc53c6224a872fd96a6aeb5035621`  
		Last Modified: Sat, 26 Feb 2022 09:47:10 GMT  
		Size: 2.6 MB (2578107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:f45368fcf4432c46abdcbfda1ad1e862e9e8dc9702b9db5c42a12e3c85e9e1ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50179648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfd41ddfd7753f008a58cd0d5d75fecf8b3b2e6a8d007fec760be87231596dd`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:06:09 GMT
ADD file:005ec6e437fc9cf8458edb6369462ce53feb585501ea6b5e5f4a6264557b3a01 in / 
# Tue, 01 Mar 2022 02:06:14 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:08:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 19:08:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 19:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:47:41 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 22:26:11 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 22:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 22:40:07 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 22:40:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 22:40:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 22:40:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 22:40:19 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 22:41:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 22:41:06 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 07:33:40 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 07:33:47 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 07:34:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 07:34:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3cee81bb9485c9d0b620c87842e566d7a1f93086ef88c00a4d7175fc776b7f3f`  
		Last Modified: Tue, 01 Mar 2022 02:16:22 GMT  
		Size: 30.6 MB (30562288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2ceee1a1325a3d6743de7471b6bed2f51edc3acb819f882064c9932632261b`  
		Last Modified: Tue, 01 Mar 2022 23:57:12 GMT  
		Size: 2.9 MB (2887538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe70af923229f44498535b3b7f05fc2e64a2d5fd14181d3c556250f4518963a6`  
		Last Modified: Wed, 02 Mar 2022 00:01:48 GMT  
		Size: 11.5 MB (11512068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0219eb9a0e496cec4555a6e7faff378348cdb80c8b6c9c5da34f2e30f11aab`  
		Last Modified: Wed, 02 Mar 2022 00:01:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a284d661685f9364c852e8174db5c9bdf4fa4fdda0eba89a4767e0cbae5b3a`  
		Last Modified: Wed, 02 Mar 2022 00:01:47 GMT  
		Size: 2.6 MB (2637463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d792dca5a3b8addfec26e8dd85f600c7a765ef5ce4a51bc44952cdb34b22e43`  
		Last Modified: Wed, 02 Mar 2022 07:41:06 GMT  
		Size: 2.6 MB (2580054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8-buster` - linux; s390x

```console
$ docker pull hylang@sha256:e7fce0a2d02fa150e4e1084d55d941c50e8e11dab99230d9cf40cbc3b62335c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44026079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9a9f3daf0b80099edce7c7ad4989a6cd3f311548ebb1420b05863eadca51ca`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:27 GMT
ADD file:908bd36a2b17b792aa02339ed6a72d1051267279d72330b1c5cd8617ca5d819e in / 
# Tue, 01 Mar 2022 02:02:28 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:53:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 10:53:55 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 10:53:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 11:55:42 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 12:11:16 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 12:16:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 12:16:04 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 12:16:04 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 12:16:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 12:16:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 12:16:05 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 12:16:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 12:16:15 GMT
CMD ["python3"]
# Tue, 01 Mar 2022 20:52:03 GMT
ENV HY_VERSION=1.0a4
# Tue, 01 Mar 2022 20:52:03 GMT
ENV HYRULE_VERSION=0.1
# Tue, 01 Mar 2022 20:52:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 01 Mar 2022 20:52:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cb73b674076b2da947cefa0692c1d193bda8bfd443c178f9bb39bbae7656ead8`  
		Last Modified: Tue, 01 Mar 2022 02:08:05 GMT  
		Size: 25.8 MB (25769053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfef4d19cc7d3537586233da8e2d4f810a292090eaedd6b56849d4e798b431b`  
		Last Modified: Tue, 01 Mar 2022 12:41:17 GMT  
		Size: 2.5 MB (2459523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9aa040f23a8f32eb922436d5098e99a5c5b1cc440ad9ac1be35cfb4781d9c1`  
		Last Modified: Tue, 01 Mar 2022 12:43:34 GMT  
		Size: 10.6 MB (10581777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208fc17884b2c3324941de8d506e5e2ab0bb9c5ce218fd8d499fdc0ab08fa58`  
		Last Modified: Tue, 01 Mar 2022 12:43:32 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028f8bf9ca2d17500dcd2c5cdb562774f350c4715c4dc441880c4c11449d6427`  
		Last Modified: Tue, 01 Mar 2022 12:43:33 GMT  
		Size: 2.6 MB (2635883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee96b7429785f0a7fce5f03249571ae4c60d475d40f047cfcdfe657d26f20f7`  
		Last Modified: Tue, 01 Mar 2022 20:56:24 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
