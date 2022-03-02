## `hylang:python3.8`

```console
$ docker pull hylang@sha256:da93a1608e4b62e4ce5dfe79442d578101205c1540bf3e1d7deddaf4aa5fd0f3
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
$ docker pull hylang@sha256:84d08275f8cef0ae329962b351eac2171700f175ee3c98fd97c281e38a660cad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48433374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33878d338ec022fbdd3cd48cde0cb2285457cc3bfdfa335b3f1e7fc33d11a39d`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 19:41:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 19:41:08 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 19:41:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:58:07 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 05:07:18 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 00:16:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 00:16:50 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 00:16:50 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 00:16:50 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 00:16:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 00:16:51 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 00:17:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 00:17:03 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 02:50:04 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 02:50:04 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 02:50:08 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 02:50:08 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c69ac0246d0815a09c65c7b9a19e8a486a5ba057aed0c83bce1794bdd856f67`  
		Last Modified: Wed, 26 Jan 2022 22:33:25 GMT  
		Size: 1.1 MB (1075873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda7900819bb44d1743910b2328364c21a2b2d70cd65c990695500106ca05a8a`  
		Last Modified: Sat, 26 Feb 2022 01:54:54 GMT  
		Size: 10.8 MB (10771545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafdd3bd3311a164b11bfd8058b2944cbbe514f2ca33f998f13dfad14978fc1d`  
		Last Modified: Sat, 26 Feb 2022 01:54:52 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc656e4e028601cc6196dd0b2d66f19e3c05adc03deb4a3e529914fd30a342`  
		Last Modified: Sat, 26 Feb 2022 01:54:53 GMT  
		Size: 2.6 MB (2639864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4a8dfc05ba342c0b5c428731bff6e45712c3e55f45313da9b3e27d65eb61de`  
		Last Modified: Sat, 26 Feb 2022 02:55:05 GMT  
		Size: 2.6 MB (2579595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm variant v5

```console
$ docker pull hylang@sha256:2900b5be44d0d7cf288a488c09ba90ba417e071013a4c6ce6f3443e0641c5887
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45516612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8baca103e90f4c03c29a4624e375d816d7ac6597029d817d833211f3e9a9a54`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:53 GMT
ADD file:eb61ee802e5118b26e1fec2c7fc58e34de0de54a5fd47dc6318c11a039ef528f in / 
# Tue, 01 Mar 2022 02:02:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 17:32:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 17:32:09 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 17:32:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:05:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 22:06:19 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 22:20:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 22:20:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 22:20:30 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 22:20:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 22:20:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 22:20:32 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 22:21:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 22:21:05 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 14:58:05 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 14:58:05 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 14:58:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 14:58:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4aa6e26b4dfdac27e5b5e15b7ebf4366149755a79dd653a5b68d9d93dd94c695`  
		Last Modified: Tue, 01 Mar 2022 02:18:33 GMT  
		Size: 28.9 MB (28909528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb765ddcf868286aae388a54f7f7a5dee147972844794d14ff82c63e4205e2`  
		Last Modified: Wed, 02 Mar 2022 00:14:04 GMT  
		Size: 1.1 MB (1059088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6dc343d8a5184c6ced6d336abcec6783ede3b44cbf47c6fbc3d88dc74cf9eb`  
		Last Modified: Wed, 02 Mar 2022 00:17:58 GMT  
		Size: 10.3 MB (10328567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5410c7c22252220ab4098d00b1a3d72529c3d099eef5c0e42bfda1a830a14e`  
		Last Modified: Wed, 02 Mar 2022 00:17:50 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9213dd0f3215c90725891aaae861f32fda61fba25a153609e8fc42cd4c48d2dc`  
		Last Modified: Wed, 02 Mar 2022 00:17:53 GMT  
		Size: 2.6 MB (2639411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45776174fa8afe5386b9f968ac095211cd3817aaf611163ad02648981872d390`  
		Last Modified: Wed, 02 Mar 2022 15:03:21 GMT  
		Size: 2.6 MB (2579781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm variant v7

```console
$ docker pull hylang@sha256:b7428276c13d1c9e512c69b4993b4a6725ff239c568c8b2c1527729a6dda005a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42727299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9309060ced2c309143b326361f05d91fdf2f55d9256ff6ad0103ab0085967c`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 18:09:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 18:09:36 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 18:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:32:18 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 09:59:43 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 05:47:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 05:47:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 05:47:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 05:47:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 05:47:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 05:47:35 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 05:48:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 05:48:03 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 09:58:34 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 09:58:35 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 09:58:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 09:58:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f2c140f38d26ad2b6602faf024e7f3386f720fe3522f95ff6bb1b180a54b77`  
		Last Modified: Thu, 27 Jan 2022 01:33:23 GMT  
		Size: 1.0 MB (1041343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0332d82442a86b571c4cc13e3635fc48747c944f81cb9e15f53d7cb9d17b63`  
		Last Modified: Sat, 26 Feb 2022 09:07:11 GMT  
		Size: 9.9 MB (9901486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd5ba838dd08f599b9cc4d04fd9793c1c537775f17ef095ca13f56262ac2d4c`  
		Last Modified: Sat, 26 Feb 2022 09:07:04 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138b4170dd0b28165c29d7463bf7a7c8386a41baa72d4e28fcb554ddf4d88b6f`  
		Last Modified: Sat, 26 Feb 2022 09:07:07 GMT  
		Size: 2.6 MB (2639483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfd029f436ac86034f98d3f7df47f6d5248bb0600197763d6e0c0e81c8e1696`  
		Last Modified: Sat, 26 Feb 2022 11:48:22 GMT  
		Size: 2.6 MB (2579815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:1abacf761f967bc1c4d4201627ecdf3d603be0bef8f00cf6d0d1e3c15435dbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46895667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac0c18a4234041ef72f98964076b3071778118db1dea6c7a79f8e53f49f8c83d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:18:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 19:18:20 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 19:18:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 20:47:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 21:09:04 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 21:14:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 21:14:05 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 21:14:05 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 21:14:06 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 21:14:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 21:14:08 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 21:14:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 21:14:20 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 15:35:09 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 15:35:10 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 15:35:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 15:35:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035530c613019c233e8c92570cc5d166a19b90cab677f02cd842b59f494d70f6`  
		Last Modified: Tue, 01 Mar 2022 21:56:28 GMT  
		Size: 1.1 MB (1064031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430f5ca6cd82b44e6866ef8d115ed37568e2f583f93643bd4381aa67aec7c3ff`  
		Last Modified: Tue, 01 Mar 2022 22:00:43 GMT  
		Size: 10.8 MB (10772555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594f692a6b578ff0cd4bb350aed66260c95112c46aea91f790514615f67e85dd`  
		Last Modified: Tue, 01 Mar 2022 22:00:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642a9dd65073d74a0290adefd3473b6ec56f145cd60f2966f16ca861141d7a4f`  
		Last Modified: Tue, 01 Mar 2022 22:00:41 GMT  
		Size: 2.4 MB (2424304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969972b78ef14c0f485aa013c34fd9f5bcf35f5645054dfe0cff500fed8d14cc`  
		Last Modified: Wed, 02 Mar 2022 15:40:24 GMT  
		Size: 2.6 MB (2577531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; 386

```console
$ docker pull hylang@sha256:4ff444c6851b0ea4b23e00104c5765a7891320fd68e10e71b63f9774f4967426
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49556679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e4133e1ac7c8356366e9f5b8d0dde26785da8a34af35da9333fdc865ddeab`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:16:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 22:16:47 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:16:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 00:42:13 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Wed, 02 Mar 2022 01:24:02 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 02 Mar 2022 09:56:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 02 Mar 2022 09:56:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Wed, 02 Mar 2022 09:56:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 02 Mar 2022 09:56:33 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 02 Mar 2022 09:56:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Wed, 02 Mar 2022 09:56:34 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Wed, 02 Mar 2022 09:56:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 02 Mar 2022 09:56:47 GMT
CMD ["python3"]
# Wed, 02 Mar 2022 10:28:56 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 10:28:56 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 10:28:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 10:28:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63dcfb8da56cf07b5cffd0becf1ed7f576ad2d4a3614d661c1965326792adfc`  
		Last Modified: Wed, 02 Mar 2022 02:37:31 GMT  
		Size: 1.1 MB (1088320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870291c288d1f0718ca760e1c275e733b1fe9b9969a82c379170b3bfa34e61b6`  
		Last Modified: Wed, 02 Mar 2022 10:02:14 GMT  
		Size: 10.9 MB (10871819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fcd5ef61f9b1b4a51a5e98a3da19e7e5f3d3a5c48fca867acae82f4cd3818c`  
		Last Modified: Wed, 02 Mar 2022 10:02:12 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6a6ca523d8aaaf5bb12953181c7e5dc2d58a0165bc105ce2213ade469da262`  
		Last Modified: Wed, 02 Mar 2022 10:02:13 GMT  
		Size: 2.6 MB (2639296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a73811578fb09c644b22a8b42164fda22c7de1c0be4a8b2d741545395101c2`  
		Last Modified: Wed, 02 Mar 2022 10:33:12 GMT  
		Size: 2.6 MB (2579620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; mips64le

```console
$ docker pull hylang@sha256:7f3e0f0c94bb40f62d5b9d5140789de5d81f7e178ccfe19a686b9801d3a40ee2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46536359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4701bfde3f5921f3af4e6d7c08d25c1ae5c53a3f3546bf651ec36f65ffa47a`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 01:15:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Jan 2022 01:15:35 GMT
ENV LANG=C.UTF-8
# Thu, 27 Jan 2022 01:15:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 03:31:57 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 11:55:08 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 05:16:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 05:16:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 05:16:52 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 05:16:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 05:16:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 05:16:53 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 05:17:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 05:17:35 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 09:45:12 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 09:45:12 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 09:45:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 09:45:22 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a6c51f2dbb998dba27bc54dd51b58820bbaac9d06b62eaeb5f807f5ba42f8`  
		Last Modified: Thu, 27 Jan 2022 11:22:27 GMT  
		Size: 1.0 MB (1049303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342f9a69330fcbf2625d6f3b83740b620cb8ce1536f54c762a039e30e69de7b7`  
		Last Modified: Sat, 26 Feb 2022 09:26:48 GMT  
		Size: 10.6 MB (10636664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea83892efe8b915b6e09ec8da3fc52eae162336b017c7467d3ea4e29be21ebc`  
		Last Modified: Sat, 26 Feb 2022 09:26:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25942c1d7e98f3c35f753eece78ea262b7a469415db2d5b0f3b0f1c654e3add6`  
		Last Modified: Sat, 26 Feb 2022 09:26:43 GMT  
		Size: 2.6 MB (2639128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120749a2fa13cbeb452a521dda84a56532819fe5b0e3887390eaa279580ffaf6`  
		Last Modified: Sat, 26 Feb 2022 09:46:57 GMT  
		Size: 2.6 MB (2578191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; ppc64le

```console
$ docker pull hylang@sha256:2a63d093de469c9e12f90612be115f8fc0a437f387e6d759894b5a2b6b4fa02a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52715608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0310558eac2cee95f55f2dec0db3e7d5623ee49ff0b65faa0d496c114624edc`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 14:37:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 14:37:38 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 14:37:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:46:58 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 29 Jan 2022 07:38:16 GMT
ENV PYTHON_VERSION=3.8.12
# Sat, 26 Feb 2022 03:39:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Sat, 26 Feb 2022 03:39:57 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Sat, 26 Feb 2022 03:40:06 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 26 Feb 2022 03:40:11 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 26 Feb 2022 03:40:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Sat, 26 Feb 2022 03:40:23 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Sat, 26 Feb 2022 03:41:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Sat, 26 Feb 2022 03:41:07 GMT
CMD ["python3"]
# Sat, 26 Feb 2022 07:59:06 GMT
ENV HY_VERSION=1.0a4
# Sat, 26 Feb 2022 07:59:12 GMT
ENV HYRULE_VERSION=0.1
# Sat, 26 Feb 2022 07:59:41 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sat, 26 Feb 2022 07:59:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9ac9a9a11bb9e08e160ed77196aada8f8279f4086eab125501a518a2e6d5`  
		Last Modified: Wed, 26 Jan 2022 19:24:59 GMT  
		Size: 1.1 MB (1094416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e4623f6bb9f5d5787fcf795ba766274d0ee4a07cbfda0aeda05c6323d91ca9`  
		Last Modified: Sat, 26 Feb 2022 06:18:18 GMT  
		Size: 11.1 MB (11126240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396d528ae756bd0cd5ac4851d7401e0d50142b1a72de448aa7aba511b043e135`  
		Last Modified: Sat, 26 Feb 2022 06:17:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da2d9c8446a06f80f487b649d86ac241b2daf1a73cb3e94a9511e78878199b1`  
		Last Modified: Sat, 26 Feb 2022 06:18:08 GMT  
		Size: 2.6 MB (2641656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f6849bc5bee99f79a49b274a284be6d3757d14e94ccbbf2a34280ebdf8b681`  
		Last Modified: Sat, 26 Feb 2022 08:14:36 GMT  
		Size: 2.6 MB (2580027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.8` - linux; s390x

```console
$ docker pull hylang@sha256:7edb3d9198476052c595ecde8b48852dab9e580d6e4c3fa0dfe309dfe64070d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46531133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abd7425a393225cb4f9b561405fb8716ca42cb3b2d10529e8fd54df45de6ba9`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:32:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 10:32:10 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 10:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 11:45:25 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 01 Mar 2022 12:05:56 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 01 Mar 2022 21:04:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 01 Mar 2022 21:04:17 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Tue, 01 Mar 2022 21:04:17 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 01 Mar 2022 21:04:17 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 01 Mar 2022 21:04:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Tue, 01 Mar 2022 21:04:17 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Tue, 01 Mar 2022 21:04:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 01 Mar 2022 21:04:27 GMT
CMD ["python3"]
# Tue, 01 Mar 2022 23:17:53 GMT
ENV HY_VERSION=1.0a4
# Tue, 01 Mar 2022 23:17:53 GMT
ENV HYRULE_VERSION=0.1
# Tue, 01 Mar 2022 23:17:55 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 01 Mar 2022 23:17:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e2d1576afb1f1f1a821f4c7327ae75bce0954c56bc387b877c8b773f4ec6fe`  
		Last Modified: Tue, 01 Mar 2022 12:40:55 GMT  
		Size: 1.1 MB (1075376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa583f4ad4cdec1b1889e6ce84d10e4a9b071c0c1b005216ae448613627871`  
		Last Modified: Tue, 01 Mar 2022 21:09:50 GMT  
		Size: 10.6 MB (10589633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf7d15c02d9502ed11304db341200702b9dcb8677c9858531a87573e00cf7d1`  
		Last Modified: Tue, 01 Mar 2022 21:09:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4059cd7ee65e85272b33039c1d68279d9ced39032131dc580ae0b4d4c752d5`  
		Last Modified: Tue, 01 Mar 2022 21:09:49 GMT  
		Size: 2.6 MB (2639211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309c1f5f439f96677bac9689eaf22fdcf578f870b9d602a2e264a773f4318a26`  
		Last Modified: Tue, 01 Mar 2022 23:21:34 GMT  
		Size: 2.6 MB (2579547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
