## `hylang:0-python3.8-buster`

```console
$ docker pull hylang@sha256:ecf6a92910c25fab08515ee78374f03e4f1d8f44f21a4ecc7a1e8e3c97fd757a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-python3.8-buster` - linux; amd64

```console
$ docker pull hylang@sha256:2f9505e11245cda1ad95504e8527be83b89501e2cf07505de71e5b359f7d0ed5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47837311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9e0fb607891b51d696da8c9d9bf26a80ff2f2cf20ca0885943f23a3ab9439`
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
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_VERSION=3.8.16
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:20:26 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 13:41:39 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 13:41:39 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 13:41:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 13:41:55 GMT
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
	-	`sha256:3ae62d6907d013c92879ed397b5707f5ae4adcd31a4061f04c457b9192594b4d`  
		Last Modified: Wed, 12 Apr 2023 07:23:43 GMT  
		Size: 10.9 MB (10879735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9ec96af43b6a10ba96048bbf7213bb0c409d440c38201550739467880fffe`  
		Last Modified: Wed, 12 Apr 2023 07:23:42 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68090968714daa7b724d93f2d59a41bf7d2b6f00bb374ba574f93593b937791`  
		Last Modified: Wed, 12 Apr 2023 07:23:42 GMT  
		Size: 3.2 MB (3195714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1297c67cf8798d2935a9d60dcec58dd7ee2c335ed8316f1181ab694b342f7`  
		Last Modified: Wed, 12 Apr 2023 13:48:40 GMT  
		Size: 3.8 MB (3840616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:1114f56f7a0c11857cc3be2c24169e77019e2167db828ad631130c0f7a04b3d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42390742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f40034b5ee8b988d0d21bb027c87bdf6397b22a58968162383e4fd78742ae8b2`
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
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_VERSION=3.8.16
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:00:02 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:00:02 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 12:41:09 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 12:41:09 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 12:41:25 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 12:41:25 GMT
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
	-	`sha256:66124a80e99182056c260cfc21462ba0abde360de3bac7c540eea0b1dcbc033c`  
		Last Modified: Wed, 12 Apr 2023 07:31:53 GMT  
		Size: 10.2 MB (10237287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ac6c85f97353227642512a525650c764ce9e5ea4e1295cf4e9ba2efc3edd2f`  
		Last Modified: Wed, 12 Apr 2023 07:31:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e3d818f754d06d5a05477959f792a71c37d97433b57c116e54a48d1f18109`  
		Last Modified: Wed, 12 Apr 2023 07:31:52 GMT  
		Size: 3.2 MB (3195048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a1aade4892f5f154f9808166e9f7aeebe5055d0e0edf469040d57c570e71fb`  
		Last Modified: Wed, 12 Apr 2023 12:44:54 GMT  
		Size: 3.8 MB (3840476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a98b51b75a21dd53615ce487dac0a20681bba7135e2fc5a6125f53c5b27a3578
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46571550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85a9c7e2b1bbca67aff55dc48cb628545d36d92ccc2e4f686b1b892902fe38c6`
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
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_VERSION=3.8.16
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 12 Apr 2023 00:40:02 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 12 Apr 2023 00:40:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 12 Apr 2023 00:40:02 GMT
CMD ["python3"]
# Wed, 12 Apr 2023 18:56:49 GMT
ENV HY_VERSION=0.26.0
# Wed, 12 Apr 2023 18:56:49 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 12 Apr 2023 18:57:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 12 Apr 2023 18:57:03 GMT
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
	-	`sha256:5d8243d7d96585d14542b1bc302be1078ec8865c69824dc2611d6729b0d88feb`  
		Last Modified: Wed, 12 Apr 2023 12:47:13 GMT  
		Size: 11.0 MB (10964927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bf1b5c9d39be1ccff9a83730b1d228741788094d54979e5b98b6a55338521e`  
		Last Modified: Wed, 12 Apr 2023 12:47:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee04eb4d16f7319ec9adf3ad932aa242e73a84e323fcb0b79be93d1d37ba35`  
		Last Modified: Wed, 12 Apr 2023 12:47:11 GMT  
		Size: 3.2 MB (3195259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6427f88a95ef152e41d0f3bcaabb3c97b474357fb5f0cb566e311a7339e623ac`  
		Last Modified: Wed, 12 Apr 2023 19:03:31 GMT  
		Size: 3.8 MB (3840383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.8-buster` - linux; 386

```console
$ docker pull hylang@sha256:55d41cb286c95c088778fb7620af586f7adaad41ec9a362a82c585711956d566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49065109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bbe41d3a450ca239793a45f2e39dce4013ae9b0814d556362fe82b4a81c8bd`
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
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_VERSION=3.8.16
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/0d8570dc44796f4369b652222cf176b3db6ac70e/public/get-pip.py
# Wed, 03 May 2023 00:01:24 GMT
ENV PYTHON_GET_PIP_SHA256=96461deced5c2a487ddc65207ec5a9cffeca0d34e7af7ea1afc470ff0d746207
# Wed, 03 May 2023 00:01:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Wed, 03 May 2023 00:01:24 GMT
CMD ["python3"]
# Thu, 04 May 2023 02:07:38 GMT
ENV HY_VERSION=0.26.0
# Thu, 04 May 2023 02:07:38 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 04 May 2023 02:07:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 04 May 2023 02:07:57 GMT
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
	-	`sha256:91f5fbaa269af31d738beed960d439a50a18f970fd5c6e49e3dea1ade8347ebb`  
		Last Modified: Wed, 03 May 2023 08:46:07 GMT  
		Size: 11.0 MB (10993986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932337972458f61eac833f61aeb41f776a3446d2414ce4c60ac0081a56f7b075`  
		Last Modified: Wed, 03 May 2023 08:46:04 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab70b3a0796195ac0ff8fc099a3b5d7f9a03865a114e88d62d64822fe46f9b14`  
		Last Modified: Wed, 03 May 2023 08:46:06 GMT  
		Size: 3.2 MB (3195601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a1340608a80c5adf4fd514aa67fb2104f4a65b9313d7f65db2c5897fbbd50a`  
		Last Modified: Thu, 04 May 2023 02:18:37 GMT  
		Size: 3.8 MB (3840862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
