## `hylang:python3.9-buster`

```console
$ docker pull hylang@sha256:aed0efd48b82482512c176b62d21ecb0200681e0685114a93aca7fdfe574dae1
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

### `hylang:python3.9-buster` - linux; amd64

```console
$ docker pull hylang@sha256:ab4ca4ba133e4dd9ee0597ee6a2ea7907ce5a56c4e07cadb4317bee01e2633f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49258480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef3c0bda2622e36ebaafb04780a692af70868e071c7325b9ae9ad725e686cec`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:53:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 06:53:31 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 06:53:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 08:11:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 02:26:15 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 02:33:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 18 May 2022 02:33:13 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 02:33:13 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 02:33:13 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 02:33:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:33:13 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:33:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:33:26 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:30:40 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:30:40 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:30:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:30:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6ad99ea909a8e7e56d780af197688927f3e510afee112f9347d538941bf4ed`  
		Last Modified: Wed, 11 May 2022 09:14:48 GMT  
		Size: 2.8 MB (2779154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff5e7ed593f92f792e8fca89882ed0b67cd35e6892ba11567b972e0173c199`  
		Last Modified: Wed, 18 May 2022 02:50:55 GMT  
		Size: 13.3 MB (13257427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccd39b73226bbd356af2ed3feeb5efdd41a76c0a4c63f00c9d773cdd9db91c4`  
		Last Modified: Wed, 18 May 2022 02:50:48 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6da97eafde18741c4f6cf62ae48860caec351ffcd3900e9f2a613965fb9b4ec`  
		Last Modified: Wed, 18 May 2022 02:50:49 GMT  
		Size: 3.2 MB (3163557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73f3ff51f68078a7aaed05367b39f792d9378b9cf28a4df8dcc1f35de11d58`  
		Last Modified: Wed, 18 May 2022 04:34:43 GMT  
		Size: 2.9 MB (2917387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:835cd0b5bca68c389420648896ac9d613f534e4356424c7fb83898a98d180b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44676520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787e47ea1c1f4266e08b24031a9488f210ee65c3bf00808cf45d07a57357e351`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:51:34 GMT
ADD file:c4087f224dff43064778eac76e711d30ca4882a1d3b571b1cd509089166abc0d in / 
# Wed, 11 May 2022 00:51:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:54:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 17:39:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 11 May 2022 17:39:50 GMT
ENV PYTHON_VERSION=3.9.12
# Wed, 11 May 2022 17:55:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 11 May 2022 17:56:01 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 17:56:01 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 17:56:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 17:56:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 17:56:02 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 17:56:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 17:56:37 GMT
CMD ["python3"]
# Thu, 12 May 2022 13:11:48 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 13:11:49 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 13:11:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 13:11:58 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:69d6138017be389335ab570ff643096d0ea914f563d41f238e7ff3520fe8e93f`  
		Last Modified: Wed, 11 May 2022 01:07:20 GMT  
		Size: 24.9 MB (24889917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c9cbc55462b64ecb80392c71ae9e8fe4012fd5d23e56aa12186ff73e82f50c`  
		Last Modified: Wed, 11 May 2022 19:41:03 GMT  
		Size: 2.5 MB (2465908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2790d1e4536fd63910c65951aee74146146eeb9acee36fab6234c7de3215a86`  
		Last Modified: Wed, 11 May 2022 19:43:47 GMT  
		Size: 11.2 MB (11239909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c589001d2920dcb62ad19130a47b1f14d9e3cd638d166485c16c301e628540b`  
		Last Modified: Wed, 11 May 2022 19:43:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6c55808958606c07c220e9024014856d724316a209d3b7d394bfd45ccda0`  
		Last Modified: Wed, 11 May 2022 19:43:43 GMT  
		Size: 3.2 MB (3163058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebe00789e24c284386fa9857b825a88b0000a1018844f8568ad4df3994fcee6`  
		Last Modified: Thu, 12 May 2022 13:15:33 GMT  
		Size: 2.9 MB (2917495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:87828de4f777a372e88719ac6eb1bf27e70588ddf2c4178ee0d7af043cdf8d55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41960047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cdcc19e9678212b69696ce076a251e5738e323161bb72687aa2d70b0a34469`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 12 May 2022 00:24:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 00:24:13 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 00:24:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:19:44 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 04:19:44 GMT
ENV PYTHON_VERSION=3.9.12
# Thu, 12 May 2022 04:40:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 04:41:00 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 04:41:00 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 04:41:01 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 12 May 2022 04:41:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 04:41:02 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 04:41:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 04:41:33 GMT
CMD ["python3"]
# Fri, 13 May 2022 04:30:47 GMT
ENV HY_VERSION=1.0a4
# Fri, 13 May 2022 04:30:48 GMT
ENV HYRULE_VERSION=0.1
# Fri, 13 May 2022 04:30:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 13 May 2022 04:30:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2666dbd22c5ecdda848152028666a8b0af6b9a293097b8d17e14a821b798e4`  
		Last Modified: Thu, 12 May 2022 07:42:43 GMT  
		Size: 2.4 MB (2366766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03631337e1920ba3f86e41a3b7ec1b2593dec0c06efb9ca955be3f393892ff56`  
		Last Modified: Thu, 12 May 2022 07:46:22 GMT  
		Size: 10.8 MB (10764812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54a1d0bd5bfdd75df75612c969d0db97b6fa70dd0ecfbd2317d9f5fec68473b`  
		Last Modified: Thu, 12 May 2022 07:46:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a68e28409e9c5247a83c38c47026eedf4220b9148fd520bc31fd63e9bbd17c4`  
		Last Modified: Thu, 12 May 2022 07:46:18 GMT  
		Size: 3.2 MB (3163048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c3167b3a7b748a29d1f43a8bf78c1ef545e1446661795a8a42dd91d37eb9ee`  
		Last Modified: Fri, 13 May 2022 04:38:34 GMT  
		Size: 2.9 MB (2917324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:bf5b6a3754be49ee83bc7def44131ca078dfce9c1bcee2a2c8fea0a214e33889
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47553785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24bd9083681a3779eb74a429bfa7bd95c4bb8c2d7321d14b76c8b445ef01b17d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:36:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 09:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 09:36:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:51:10 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 04:24:08 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 04:29:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 18 May 2022 04:29:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 04:29:34 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 04:29:35 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 04:29:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 04:29:37 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 04:29:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 04:29:50 GMT
CMD ["python3"]
# Wed, 18 May 2022 05:44:04 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 05:44:05 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 05:44:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 05:44:09 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac2dc30cdb0e169a8e4b71c92f0d26d2a491db21e38d4aeb17254b1d44f258e`  
		Last Modified: Wed, 11 May 2022 11:49:34 GMT  
		Size: 2.6 MB (2642958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5224d0b8a514f79a5937ef1383df2930ee7865584decfdc22f4de458fb8ace`  
		Last Modified: Wed, 18 May 2022 04:50:34 GMT  
		Size: 13.1 MB (13138707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42a44c433964932482dacbd9262af7e8047ff4eaac63d2ef9e89142458c93f5`  
		Last Modified: Wed, 18 May 2022 04:50:31 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1da2b4268578dc0995dfc715eaee4a996982f633e4ca94b47ca08c6e59b092`  
		Last Modified: Wed, 18 May 2022 04:50:32 GMT  
		Size: 2.9 MB (2947405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b5628c1cde403c19848fff48245ada70e2458ad279073a1725bf47e5956561`  
		Last Modified: Wed, 18 May 2022 05:50:29 GMT  
		Size: 2.9 MB (2915467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; 386

```console
$ docker pull hylang@sha256:f692732fea14f4e5657bab96d207a632d3e30c7cb63382a6817f3f278e39c074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49838913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1513b9a3f24c2ab31d6d44485fac8b13bad3dd8bcbf38e12eaefc4de318bee6`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:09:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 12:09:01 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 12:09:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 13:42:43 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 02:57:02 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 03:04:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 18 May 2022 03:04:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 03:04:13 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 03:04:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 03:04:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 03:04:16 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 03:04:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 03:04:32 GMT
CMD ["python3"]
# Wed, 18 May 2022 03:47:30 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 03:47:31 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 03:47:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 03:47:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b4fda249c769104bec88ea5a7682b1c32c70f3e9fb9c075fd3296f5f4fa55c`  
		Last Modified: Wed, 11 May 2022 14:44:53 GMT  
		Size: 2.8 MB (2787351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd8be4db734b79281369162f9a87996a100aa54b2ba2724a2c6d1250fbc76d`  
		Last Modified: Wed, 18 May 2022 03:27:03 GMT  
		Size: 13.4 MB (13389468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7322f28e945ac7ecf98e6bcc6f8510724e057adfce846072340f0c25bd49c4`  
		Last Modified: Wed, 18 May 2022 03:26:59 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8764ab8a8b3e8e47bc567d7067d58daa5c80e1f357e83044530e63dd9aaf52da`  
		Last Modified: Wed, 18 May 2022 03:27:00 GMT  
		Size: 2.9 MB (2947351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf01eb22549d0f3a6549cfcee3ba6936ada4a27ce0e95fe868a33e06b2d2cc4`  
		Last Modified: Wed, 18 May 2022 03:54:14 GMT  
		Size: 2.9 MB (2915360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:03dde0fad047ebe9f9da46272206a892a1c973b409116036d69945e9f829024d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45458069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bd24426be758569521c556139425427b7b9b2db4be786c7b388cfb54f49ec11`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 02:24:43 GMT
ADD file:caccabd8a6e13c6bee91558efc76401078239e82c1a4a939aaf89520fab347fd in / 
# Wed, 11 May 2022 02:24:48 GMT
CMD ["bash"]
# Thu, 12 May 2022 07:59:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 07:59:08 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 07:59:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 15:47:34 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 15:47:37 GMT
ENV PYTHON_VERSION=3.9.12
# Thu, 12 May 2022 16:37:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 16:37:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 16:37:58 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 16:38:01 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 12 May 2022 16:38:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 16:38:06 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 16:39:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 16:39:05 GMT
CMD ["python3"]
# Fri, 13 May 2022 11:01:11 GMT
ENV HY_VERSION=1.0a4
# Fri, 13 May 2022 11:01:14 GMT
ENV HYRULE_VERSION=0.1
# Fri, 13 May 2022 11:01:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 13 May 2022 11:01:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:04988468cf482e6d371e4ebf5a6fb630cd38493fcc79fe45f15650a319a1a0a5`  
		Last Modified: Wed, 11 May 2022 02:35:04 GMT  
		Size: 25.8 MB (25814525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1845dd3de82063eeeb8c2c0c7042519475a6a07878ada84aa4177ded38cc67`  
		Last Modified: Thu, 12 May 2022 22:48:19 GMT  
		Size: 2.3 MB (2326917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d56a49421b1ab65bc195cf841291edd8f053cb4ad8332da940b9d68efecdf`  
		Last Modified: Thu, 12 May 2022 22:49:52 GMT  
		Size: 11.5 MB (11453011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f656163d616c95cc287175af4edf26c18dca2afbd08a5b65da1628fb1554192`  
		Last Modified: Thu, 12 May 2022 22:49:45 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97db3c7560b23303076b766df517e7bcb8dc0b4f695de02d253d0e9ae0978306`  
		Last Modified: Thu, 12 May 2022 22:49:48 GMT  
		Size: 2.9 MB (2947900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fceeff0f1d396052248f7320f9417b59592d448662962b13a8ce6db8b362feb`  
		Last Modified: Fri, 13 May 2022 11:04:32 GMT  
		Size: 2.9 MB (2915483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:6e156820a2966659fdf9a1cb52a116406c0ae70ab4a31e95a9293a472f61970c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51945822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779cc849a66680467c33adca5f8bb4fa45d98c578847927dd95ac8ba22fd9380`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:33:31 GMT
ADD file:57fcc3eadd20c2481e373ef3b56a194006f65b3c7ae29bd1747e625efcd89124 in / 
# Wed, 11 May 2022 01:33:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 22:12:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 22:12:08 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 22:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:16:15 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 12 May 2022 01:16:20 GMT
ENV PYTHON_VERSION=3.9.12
# Thu, 12 May 2022 01:37:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 12 May 2022 01:37:22 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 01:37:29 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 01:37:37 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 12 May 2022 01:37:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 01:37:50 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 01:38:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 01:38:48 GMT
CMD ["python3"]
# Thu, 12 May 2022 21:32:21 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 21:32:26 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 21:33:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 21:33:11 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:97c4e3bbd0d14c4a194ce9c48b362e1649c341b249c2ad560738b06fe8576dc3`  
		Last Modified: Wed, 11 May 2022 01:44:06 GMT  
		Size: 30.6 MB (30560544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a266e9eda2566633b06e4ae3f00f0e2b788950cc668610f85b99e86a8e9ac55d`  
		Last Modified: Thu, 12 May 2022 04:11:21 GMT  
		Size: 2.9 MB (2892838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8c7e9d28873f3e70b3ed644a62c2f2b33e1ea8dc4b32358a31e150225bd6da`  
		Last Modified: Thu, 12 May 2022 04:14:38 GMT  
		Size: 12.4 MB (12409108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b06123324ec724dbe5c99221632089d114bb586fb0b27d291511aea2058f67`  
		Last Modified: Thu, 12 May 2022 04:14:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78bbc4fc19593ae0f5182a7def37f91a161a715d66e5a4a6f42372b29504c78`  
		Last Modified: Thu, 12 May 2022 04:14:36 GMT  
		Size: 3.2 MB (3165042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a87dd5b0be5350f6aa31974c77dc4a3985b9a4f2f0c5a156cddceb44dad9b3`  
		Last Modified: Thu, 12 May 2022 21:41:04 GMT  
		Size: 2.9 MB (2918057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; s390x

```console
$ docker pull hylang@sha256:2fb27df713eec4d799d17008100f2425a25e4b0e7dd6e1aa551c9c66343eb579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47098726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e36949f891438bc509b2bae20888c6a0d7ae937bb11cb8eabb6e48dd1657f`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:03:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 07:03:11 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 07:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 08:05:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 18 May 2022 02:44:56 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 18 May 2022 02:51:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 18 May 2022 02:51:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 18 May 2022 02:51:18 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 18 May 2022 02:51:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 18 May 2022 02:51:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2d26a16e351a22108b46fa11507aa57a732d4074/public/get-pip.py
# Wed, 18 May 2022 02:51:18 GMT
ENV PYTHON_GET_PIP_SHA256=530e7077f9e31f0378b5ee7cc90c8d99b7aef832f3d4ea96b42c2072e322734e
# Wed, 18 May 2022 02:51:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 18 May 2022 02:51:30 GMT
CMD ["python3"]
# Wed, 18 May 2022 04:51:20 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 04:51:20 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 04:51:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 18 May 2022 04:51:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ebb4ded3b72921760d855885c8cd5df2d1cb473ff54cdc141f98fd017bc30c`  
		Last Modified: Wed, 11 May 2022 08:56:14 GMT  
		Size: 2.5 MB (2466610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc745417b2e23fd87a46b2c21329dda2f735406e6aa0f8cfd01a02ad456e01`  
		Last Modified: Wed, 18 May 2022 03:12:22 GMT  
		Size: 12.8 MB (12792542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab61bc8e71ccda80c990251f64ee1d62ab0a3296d312d39719145b9036a9966`  
		Last Modified: Wed, 18 May 2022 03:12:21 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8716ca10553860387460ce9e2f02c383ce5224ce67b58c17b3bfa32576823333`  
		Last Modified: Wed, 18 May 2022 03:12:21 GMT  
		Size: 3.2 MB (3163148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be6139e923de744f387eb8bac966fa171c98cfe134b1ca48ab27c3d58e7332`  
		Last Modified: Wed, 18 May 2022 04:57:00 GMT  
		Size: 2.9 MB (2917453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
