## `hylang:0-python3.10-bullseye`

```console
$ docker pull hylang@sha256:0220431ea6ca7e1070f2fd49c625d8e904b535c6b7920d4c377dd78849a1e257
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hylang:0-python3.10-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:c4978fe1ac6554b7df3ade04bdc02c6bef8f8b313cad56fb5f93f203cb46c4c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51107877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f77a45187f11dc18840e7ec0896a98e43146e0c41102478d9d40b4c0ba10146a`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:57:08 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:57:09 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:57:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:57:21 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb0f1d192947f14a4b39d3c834d07ba99bdd44fd87c51df64e0c443a9e2471c`  
		Last Modified: Wed, 29 Nov 2023 06:26:22 GMT  
		Size: 872.1 KB (872059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9a4cd9bb63fa4b6a758fe6b19075f8fa75b2b99f5eee2149ea0e023f1a6896`  
		Last Modified: Wed, 29 Nov 2023 06:28:06 GMT  
		Size: 11.5 MB (11540467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06955aa06248b2cb143e7fc84f862b24a3c874046d71c78ca59e2b2bff8ccc7`  
		Last Modified: Wed, 29 Nov 2023 06:28:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71af22f3b66b4ce0583aa73d1d7fa67cf97563c430976daeaf6fa4e843562fb`  
		Last Modified: Wed, 29 Nov 2023 06:28:06 GMT  
		Size: 3.2 MB (3157889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73216c5c587b6a764d0dbc49e0a6397fe4d4802c7f45abecb970136f5d64a373`  
		Last Modified: Fri, 01 Dec 2023 20:04:55 GMT  
		Size: 4.1 MB (4119405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; arm variant v5

```console
$ docker pull hylang@sha256:90d400c8f48f1fc367b6b3bed04a4c2722e888dce0b57800dfe995a2604efeba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48357339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5685d9fb147b2efbfc47d21b18e190dfced26b6a7d04c5ec6965d5a1f42c1f98`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:38:08 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:38:08 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:38:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:38:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d663c9904a1d311068ae97e9cf8b7e066caf39790953a8ffd1e496152443bf8`  
		Last Modified: Wed, 29 Nov 2023 07:53:46 GMT  
		Size: 856.2 KB (856177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe6c44125a68cb0688ba47b6c6ea2c4ab96657516637b12c5a9ec482e398b87`  
		Last Modified: Wed, 29 Nov 2023 07:54:56 GMT  
		Size: 11.3 MB (11302836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3b8ff9a2481c1c5805ccba0eccee2943c1f32304ff21c05ee363569dba0943`  
		Last Modified: Wed, 29 Nov 2023 07:54:56 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4c1081d56efe0c79dab9f2f8a6a85b435e40b69188b929801161873a462e1`  
		Last Modified: Wed, 29 Nov 2023 07:54:56 GMT  
		Size: 3.2 MB (3157413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674ff3ff27ba54e04b85500d93458f8de9708ad8bc9c1f39ed241130080c005c`  
		Last Modified: Fri, 01 Dec 2023 19:41:34 GMT  
		Size: 4.1 MB (4119414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; arm variant v7

```console
$ docker pull hylang@sha256:27cf2039a0e1ba98695938f0e55d110d26c8a02e014a8d95eab42500eb4b2bfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45574617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0576f00098b8d42f586acecb530126480b4958d225a6ad4e4164315ef76f68e4`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:51:17 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:51:17 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:51:31 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:51:31 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bbb4df0219ace7c34407004596f50c37aa4245fbf341b00147a6ddbd4e4417`  
		Last Modified: Wed, 29 Nov 2023 10:11:27 GMT  
		Size: 837.5 KB (837526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0e6e27f0b45f7487dd51357084f5091d46d2e7fc754bf8582b09bf57c34cc`  
		Last Modified: Wed, 29 Nov 2023 10:13:06 GMT  
		Size: 10.9 MB (10881083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81f4291fd9df0fd33df35647ddd4fb3158b0cac8f7a59e93212c3cc445231c2`  
		Last Modified: Wed, 29 Nov 2023 10:13:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9555e10be8206489cd26842d4d6eb40e20f385540d8869f7bff46f40e29573`  
		Last Modified: Wed, 29 Nov 2023 10:13:05 GMT  
		Size: 3.2 MB (3157330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e330263340f3fae7d1a42d543d3284d2d8ba9b8a510150b5fc3c98b18d51144`  
		Last Modified: Fri, 01 Dec 2023 19:58:37 GMT  
		Size: 4.1 MB (4119431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a186879fc06bda44c0566f7787b8322233495a224e5b08680023bc7ae5f7b963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49818317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb92eb2254d15a0de3a6856dab1ddc2abc6325b46927842c9f9cefeefb67d6c3`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:18:31 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:18:31 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:18:41 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:18:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84582cf09db769114e9f673cc8d7713ffa8d08802a4eab66f69c3d49ec2b2d7`  
		Last Modified: Wed, 29 Nov 2023 05:41:24 GMT  
		Size: 860.0 KB (860007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78244eddcde84ec66c6a4b10c55ef0f5f9676f4f1621acc210c3f93dabd8bf2`  
		Last Modified: Wed, 29 Nov 2023 05:43:04 GMT  
		Size: 11.6 MB (11616966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce7a746198ea7aa542ff1fe99da373020d28c4026022b50e925635b52db1b1`  
		Last Modified: Wed, 29 Nov 2023 05:43:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35c731ed944b32983b014986199e382728ecd410b521c0d9ab9d3199a8974c9`  
		Last Modified: Wed, 29 Nov 2023 05:43:04 GMT  
		Size: 3.2 MB (3157616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacfa8b7c94ee86f1004971ee3d2b774eb798535e91558bb1b4a258a4e67027a`  
		Last Modified: Fri, 01 Dec 2023 20:25:35 GMT  
		Size: 4.1 MB (4119372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:313810bf69929b6bcb58d043ec9b98fba4753ec618c8bf0f2beac712fc41f854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52234141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578f5fc8768244db62afdb06d1e2108e8beba07e02a2c60f5b99c1754dfc7b25`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:09:15 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:09:16 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:09:34 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:09:34 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2441c99198efc43d746a317d9e439d2db0bdb5432219a88a3fcf113079382e37`  
		Last Modified: Wed, 29 Nov 2023 10:17:45 GMT  
		Size: 885.1 KB (885069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afd344d1842f1272df06979d018834cb1ecb82e9bceb078dc63a0e4aa13786d`  
		Last Modified: Wed, 29 Nov 2023 10:19:31 GMT  
		Size: 11.7 MB (11669005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66133992b74a36fd199a59f89588e5a838499eacd00c074d1ab2aa5642a868d0`  
		Last Modified: Wed, 29 Nov 2023 10:19:30 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e5b8ca115ecc1052628e5eaf852bba7917a61addb3c02ae7defb733cd38fac`  
		Last Modified: Wed, 29 Nov 2023 10:19:31 GMT  
		Size: 3.2 MB (3157681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e092d8571e3888bf9efdf08f1b43f923d7d2ec274607251cd97796837e4a75`  
		Last Modified: Fri, 01 Dec 2023 20:18:13 GMT  
		Size: 4.1 MB (4119521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; ppc64le

```console
$ docker pull hylang@sha256:686fc99bcc04350e5d9d475e677bc81f9667f0e9cfc70689b67b67ead720be3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55347577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:621c4bee7af0398ad9114fe458854c9a255b3da7de9336e4d8f776afda1e2ccb`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:55:57 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:55:58 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:56:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:56:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc316fc7b226b39c68057e4196cd4dfe717f8ff2977a6ac4a7d0a73d92eab5af`  
		Last Modified: Wed, 29 Nov 2023 08:21:49 GMT  
		Size: 891.0 KB (891031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e0478e28f4da3b37921a4d693ca4b8d678df934a07c3d25fbeb4f233af65a`  
		Last Modified: Wed, 29 Nov 2023 08:23:38 GMT  
		Size: 11.9 MB (11885032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7f7b18afff7952559197e07537796c5b2e4827c02dbef646fccf7f6f3b26d8`  
		Last Modified: Wed, 29 Nov 2023 08:23:37 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44d1e270ee7e86fa02902d2f739ae34c67bfc527993b3eff356baaa8af1b536`  
		Last Modified: Wed, 29 Nov 2023 08:23:38 GMT  
		Size: 3.2 MB (3158205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a83e9de19d456c8480d5bd96852deb149d727e3566cf6187c52fb4ae5c1890`  
		Last Modified: Fri, 01 Dec 2023 20:05:19 GMT  
		Size: 4.1 MB (4119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.10-bullseye` - linux; s390x

```console
$ docker pull hylang@sha256:15e5119e50076cd2bb6a436d281c37ad6e67468db3e5a93635cf6762e986e74d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49273393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9055ffa3b26b71cac81aa4a43823d7261c9c6e83ea0343daf31ca72fc5d6577e`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 15:49:12 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 15:49:12 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_VERSION=3.10.13
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 15:49:12 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 15:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 15:49:12 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 20:13:20 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 20:13:20 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 20:13:30 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 20:13:31 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144e34c2e04673034d9eb7234ca76e0e610aefa578d44df62b35a022af55b1ae`  
		Last Modified: Wed, 29 Nov 2023 06:23:21 GMT  
		Size: 872.4 KB (872371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493cdcc73246d4d4ca486250537499f82bf9746df39c26035ed416ad6dd3563e`  
		Last Modified: Wed, 29 Nov 2023 06:24:48 GMT  
		Size: 11.5 MB (11467317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d135c2b7ac1951e11c1e9ccdaaa836f203e992b3838081bfa7400570891f643`  
		Last Modified: Wed, 29 Nov 2023 06:24:48 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb6768373d849ed63f7d0be4448add14aef696a7a1bfbb50ae8e3d2dee17a3e`  
		Last Modified: Wed, 29 Nov 2023 06:24:48 GMT  
		Size: 3.2 MB (3157359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc831cc4979ea71077ccc62b0d4a79360f21c0d64336f141e04a1b501392177`  
		Last Modified: Fri, 01 Dec 2023 20:20:01 GMT  
		Size: 4.1 MB (4119177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
