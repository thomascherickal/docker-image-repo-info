## `hylang:python3.9-buster`

```console
$ docker pull hylang@sha256:6d8c863f9856cc1af3ce052ccabbb06d2830cd55c75961464941c1b23494db86
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
$ docker pull hylang@sha256:282f3af38de95440a04e98b4a5ba5cb0c863b50a4789d654b1b41e0b5a233a55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47569353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7389b539643b7ee11bb1a693e9a0c3f1fa17fc4e77534dafead197700b12417`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 04:33:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 04:33:38 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 04:33:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 06:01:12 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 06:01:12 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 06:09:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 06:09:10 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 06:09:10 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 06:09:10 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 06:09:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 06:09:10 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 06:09:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 06:09:22 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 07:07:54 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 07:07:54 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 07:07:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 07:07:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66684bb0aed0b036dcc1554d122cca5f9c10d87952cd6f3c2d9227a47b6d7a8a`  
		Last Modified: Thu, 17 Mar 2022 07:01:48 GMT  
		Size: 2.8 MB (2770160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bcf33017dadc93097ff30214a9206fa1613e00d962e3cb1dc5b34ef1276cec`  
		Last Modified: Thu, 17 Mar 2022 07:03:46 GMT  
		Size: 11.6 MB (11565904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b8eeb7bbc41e2f9ffab932bff2f9b563dfde96d424cb39e02b5bdcbb89b12`  
		Last Modified: Thu, 17 Mar 2022 07:03:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c31d94fb4497c939fba3c5bdad7147b298cc03fc5f03f8da2c65e488fc5c6e`  
		Last Modified: Thu, 17 Mar 2022 07:03:45 GMT  
		Size: 3.2 MB (3163368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac542f634d5b575bf60d4e7882854a77e89aa8cf3db259276b9d749901b96c`  
		Last Modified: Thu, 17 Mar 2022 07:11:59 GMT  
		Size: 2.9 MB (2915856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:6921b68f8b9f04d336a6ed4e4c42c6dfe78fd6249a0b63fd0cbf1176387c5a45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44664398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78391d8a7796d0668ed683adfc0437eb15f71ceb3e394f8964e648245e909b88`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 05:48:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 05:48:49 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 05:49:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 07:57:59 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 07:58:00 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 08:14:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 08:14:40 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 08:14:40 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 08:14:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 08:14:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 08:14:41 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 08:15:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 08:15:16 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 09:24:37 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 09:24:38 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 09:24:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 09:24:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7317dbc5bee434b7c76ae48f8d6b9a5a6b4193188cc65ea8293f4956e7bbf82`  
		Last Modified: Thu, 17 Mar 2022 09:19:03 GMT  
		Size: 2.5 MB (2460624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30299c8ffd3e5199af42b9ef0afc5594e0cf309743231b3aba2b0e4e85f812b6`  
		Last Modified: Thu, 17 Mar 2022 09:21:16 GMT  
		Size: 11.2 MB (11238012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ca77b16e26bca8dc9abf47a2d089c0bc7f922526fb57549538e24f0d6b12fa`  
		Last Modified: Thu, 17 Mar 2022 09:21:09 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb488e04e940d4a407efef0a082c869774b9d68f29386f76fabfc7b7a9efef7e`  
		Last Modified: Thu, 17 Mar 2022 09:21:12 GMT  
		Size: 3.2 MB (3162984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416ea6b259a47a27912545b10442d8531541ee9659ba794f7fb3a61e1a69d484`  
		Last Modified: Thu, 17 Mar 2022 09:29:11 GMT  
		Size: 2.9 MB (2916348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:dd8c1692d3ed98c74ae906cecf24acef2abf90bc8d6cdbe80bd9a57f7173a5b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41955853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3053b8aec99ec861d88cb0687e8635c8471c73eb41d19433964289ed33d6cae`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 09:32:07 GMT
ADD file:ca7a6b7c138de7fd85996719398396d0ed0f059d2e12b7f401cd460b64924e25 in / 
# Thu, 17 Mar 2022 09:32:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:52:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 10:52:59 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:35:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 14:35:53 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 14:56:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 14:56:48 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 14:56:49 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 14:56:49 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 14:56:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 14:56:50 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 14:57:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 14:57:21 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 17:26:31 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 17:26:31 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 17:26:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 17:26:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0b8f06901fc5e8a29999e260b4ada4ee1cc4415e5c1a16fb7bb21cc2ac995f72`  
		Last Modified: Thu, 17 Mar 2022 09:48:01 GMT  
		Size: 22.8 MB (22754389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ef568202072c1523f8058da66248dda1578fb3d941702749c2c683bdcc2696`  
		Last Modified: Thu, 17 Mar 2022 17:13:40 GMT  
		Size: 2.4 MB (2358951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79d0376c119db8d9aeee68a659671e8a855051151ccd3e0e8dffa0ae4e3a034`  
		Last Modified: Thu, 17 Mar 2022 17:17:08 GMT  
		Size: 10.8 MB (10762921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021c97cf6610a845d2e288d88c0af15dfa3d5969ab47622df27653f5fac1d68`  
		Last Modified: Thu, 17 Mar 2022 17:17:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523e8a8f8e3af47a296f6895dfb5902c080e1c994969c1e2f44b7965d199f4d`  
		Last Modified: Thu, 17 Mar 2022 17:17:04 GMT  
		Size: 3.2 MB (3163087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7014ccfbfff25e8abb663d0d6c276f1893b8615f10fa4e703163b2c79e7a9319`  
		Last Modified: Thu, 17 Mar 2022 17:36:25 GMT  
		Size: 2.9 MB (2916270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a138217c1f4e603a5f7799562d8cce6bf251a9548af804f6732cfff1eb2cb4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45996925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb2c4b191886aa1f44fcc9c4b6cb8d01afb8816cbedaaf5df0da68688e140289`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 03:50:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 03:50:43 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 03:50:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 05:01:12 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 05:01:13 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 05:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 05:06:40 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 05:06:41 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 05:06:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 05:06:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 05:06:44 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 05:06:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 05:06:58 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 05:53:39 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 05:53:40 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 05:53:44 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 05:53:44 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15861050d98a70d3176176b7d15904107c38ebb5479912883c458e22b8b5b5d9`  
		Last Modified: Thu, 17 Mar 2022 05:47:14 GMT  
		Size: 2.6 MB (2636109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0abfa9c4b41536a5fa2ff1ae766238d9dab93c603ef00bdfe38278be9bfaf0b`  
		Last Modified: Thu, 17 Mar 2022 05:49:14 GMT  
		Size: 11.6 MB (11575511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26149b54d62e72c159e639b34485abe3755e0129afd2e870c6c331651e5f2b1d`  
		Last Modified: Thu, 17 Mar 2022 05:49:12 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e0c1edbfaf811cc5728d89cbe7c1a350a77b245ee823956a9c2f4d272c0869`  
		Last Modified: Thu, 17 Mar 2022 05:49:13 GMT  
		Size: 2.9 MB (2947277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a679c6e72327650d3b3da65aac3287fc318f0eefca7c3cd61596950fa6421430`  
		Last Modified: Thu, 17 Mar 2022 06:00:08 GMT  
		Size: 2.9 MB (2914561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; 386

```console
$ docker pull hylang@sha256:fd8abba92bb0a989756b0d4d5974dab17c0ffa198ab701a319998e3a17fd4817
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48144682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb1ba8261a445e5c568693b388bfc5545e1702d8af7df64ceb99318060c372c`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 08:16:28 GMT
ADD file:39b40ec7bd2f4e691b74f0287e43ab64ef32f99953e606d9e4b72d058659209c in / 
# Thu, 17 Mar 2022 08:16:29 GMT
CMD ["bash"]
# Thu, 24 Mar 2022 01:52:28 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 01:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 01:52:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 24 Mar 2022 04:25:04 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Mar 2022 04:25:04 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 24 Mar 2022 04:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 24 Mar 2022 04:31:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 24 Mar 2022 04:32:00 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 24 Mar 2022 04:32:01 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 24 Mar 2022 04:32:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 24 Mar 2022 04:32:03 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 24 Mar 2022 04:32:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 24 Mar 2022 04:32:19 GMT
CMD ["python3"]
# Thu, 24 Mar 2022 14:42:52 GMT
ENV HY_VERSION=1.0a4
# Thu, 24 Mar 2022 14:42:52 GMT
ENV HYRULE_VERSION=0.1
# Thu, 24 Mar 2022 14:42:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 24 Mar 2022 14:42:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cef703cf0f3e19a7a5f8b305254c02563c8b07f5b842bb99741d3a2fd136e9f0`  
		Last Modified: Thu, 17 Mar 2022 08:24:59 GMT  
		Size: 27.8 MB (27804570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23a34d6fb34891b88f0045cff8b3a0e2c55315044d971dd88336d7dd9e2210`  
		Last Modified: Thu, 24 Mar 2022 06:04:50 GMT  
		Size: 2.8 MB (2781210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e472a84b9e59015577d55c2f62b3036a93aaa5b1eece5fbc44c68befd6891f4`  
		Last Modified: Thu, 24 Mar 2022 06:08:41 GMT  
		Size: 11.7 MB (11696702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9722165d45d71fb330b4b40f03cdf4f5d0c98c59785ebb7af873c771e0be627c`  
		Last Modified: Thu, 24 Mar 2022 06:08:39 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c96a3812a96ae68d0fa389fc69bc23efed11332a46085bedcc851cf8621aa81`  
		Last Modified: Thu, 24 Mar 2022 06:08:39 GMT  
		Size: 2.9 MB (2947294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460e9b410f3f0b9122149526f749ea0ba176016e5da48f51daa10d1656983bef`  
		Last Modified: Thu, 24 Mar 2022 14:50:37 GMT  
		Size: 2.9 MB (2914671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; mips64le

```console
$ docker pull hylang@sha256:4da1365652c5266d8fdb4e78ba75238e8489650442acd571bfe03e291f3ec25f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45459071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb13496c7438f0cc25da326c64886e8f03328955d8a1bed00bc347d56cdba8d`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 08:54:09 GMT
ADD file:47b03990ddc290dac99c4fb2fb851724325624d58fc57f6c9902ba2a98a54bea in / 
# Thu, 17 Mar 2022 08:54:13 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:29:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 12:29:15 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 12:29:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:56:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 14:56:14 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 15:46:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 15:47:04 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 15:47:06 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 15:47:09 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 15:47:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 15:47:14 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 15:48:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 15:48:13 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 19:02:59 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 19:03:02 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 19:03:20 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 19:03:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4563fe17a75d3d628ff1f7de39c0d8aa8e256bebfcca83591111dc19e4b15795`  
		Last Modified: Thu, 17 Mar 2022 10:44:40 GMT  
		Size: 25.8 MB (25820197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32b070b930c804e1b2791f58add53e7eae8a312b7a2144bfeae0e075af9a988`  
		Last Modified: Thu, 17 Mar 2022 18:59:50 GMT  
		Size: 2.3 MB (2321381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ea9b927bb006312b13f11c2901ec23ae4f9c0f074090d56ff5f2155721bc5`  
		Last Modified: Thu, 17 Mar 2022 19:00:42 GMT  
		Size: 11.5 MB (11454369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f180015c0c941b81cf5825b2abc585ca626d5b316e8fd76a6598cf144d408d2`  
		Last Modified: Thu, 17 Mar 2022 19:00:35 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc1f7c81c96225556c04720c798e5727569e6c1bbc060676aafac6e99bcb71a`  
		Last Modified: Thu, 17 Mar 2022 19:00:38 GMT  
		Size: 2.9 MB (2947974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ab79f7e904e2615570debcdb43a44365ce8f376ebc991d47da0c6d07524b73`  
		Last Modified: Thu, 17 Mar 2022 19:06:12 GMT  
		Size: 2.9 MB (2914914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:f1992020c74f1f9462e0dc3d95d21ec4b3bdaae07c650d88e68c908b38622cf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51927475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee813c09d0b0377d86c8e535c5adb5396312ede7d732d2625815ccf7761d8df`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 11:19:08 GMT
ADD file:0af430b7759619d4d40ea316f823599879e4f3e0dfc8877bdee731020fb2620d in / 
# Thu, 17 Mar 2022 11:19:12 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:44:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 12:44:08 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 12:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 15:47:42 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 15:47:47 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 16:09:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 16:09:42 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 16:09:47 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 16:09:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 16:09:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 16:10:01 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 16:11:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 16:11:27 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 18:26:58 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 18:27:08 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 18:27:37 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 18:27:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:303d92340e7868a8dc0fdad5d6c67a8a819a74a2bc47038b26339d5be6084bf4`  
		Last Modified: Thu, 17 Mar 2022 11:29:21 GMT  
		Size: 30.6 MB (30562350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbcf63ce6fcafda2d6446763c0834ffe1d09c58ef06d2111f021cfa86b8b708`  
		Last Modified: Thu, 17 Mar 2022 18:11:17 GMT  
		Size: 2.9 MB (2887668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569083c4c52917175733cef75dccef6ff39c53d27b954cfbd8f475948a21fea9`  
		Last Modified: Thu, 17 Mar 2022 18:14:08 GMT  
		Size: 12.4 MB (12395403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744d6255a7d8149756548e51c89c18dbdc7843b04b06bc8c72e899dcab9ff067`  
		Last Modified: Thu, 17 Mar 2022 18:14:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9de7ebf2b65150ea0870571006bd363d9ff320c1d6085e28bfef6d014370d82`  
		Last Modified: Thu, 17 Mar 2022 18:14:06 GMT  
		Size: 3.2 MB (3165166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de311d0539296b8f0adb03c18081ec99f93a08504f2a9c617c5beb51596c5818`  
		Last Modified: Thu, 17 Mar 2022 18:41:47 GMT  
		Size: 2.9 MB (2916651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.9-buster` - linux; s390x

```console
$ docker pull hylang@sha256:88020833906ac291ae1ea7ef786a02ff0c96dada90d553968e75bdcc7d1b660f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45719452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f510568fb4a158676d1e31253418ad3fc55299445dd33ad31c7c0ffe74df2c`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 03:28:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 03:28:09 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 03:28:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 04:21:34 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 17 Mar 2022 04:21:34 GMT
ENV PYTHON_VERSION=3.9.11
# Thu, 17 Mar 2022 04:26:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 04:26:44 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 04:26:44 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 04:26:44 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 04:26:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 04:26:45 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 04:27:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 04:27:01 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 05:12:57 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 05:12:57 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 05:13:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 05:13:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94ead178e7de89691cb16c8442b4adcdbd9e663b23dacd2963a01f70016b`  
		Last Modified: Thu, 17 Mar 2022 05:08:42 GMT  
		Size: 2.5 MB (2459527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc826a50fda56a07946d9338e65377efba6e530e2a5a404dc0cbd42dc5c5d6d5`  
		Last Modified: Thu, 17 Mar 2022 05:09:55 GMT  
		Size: 11.4 MB (11411813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f069a7ccb8f1a56e3d3be9724d64462d31bf60490d79aeb371e17491be11a61f`  
		Last Modified: Thu, 17 Mar 2022 05:09:54 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efe10402d4a8e5783c1b898c3bc343e8c9a1ab9d3fd88794f4f93644cdd3fdf`  
		Last Modified: Thu, 17 Mar 2022 05:09:54 GMT  
		Size: 3.2 MB (3162789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6515a3ede5bd31f0a5c0c8ff39b480dffe4c4e0f282a9ea07210db610675f1b8`  
		Last Modified: Thu, 17 Mar 2022 05:18:01 GMT  
		Size: 2.9 MB (2916013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
