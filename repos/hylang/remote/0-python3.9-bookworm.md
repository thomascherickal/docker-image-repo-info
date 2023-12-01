## `hylang:0-python3.9-bookworm`

```console
$ docker pull hylang@sha256:3ac18394a07dafc5b2802ddd64f87fcbf268438c3299dc465988393bfffa5f38
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

### `hylang:0-python3.9-bookworm` - linux; amd64

```console
$ docker pull hylang@sha256:296920633196e1931254bb26ee216bc84c311f4bd21da88f781ec4fe48f738c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50881764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f402dd6630463537bcfc65b9b5839ef92165d210602cc8fb6c17eb43782e1225`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 21:17:19 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 21:17:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_VERSION=3.9.18
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:58:00 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:58:00 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:58:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:58:13 GMT
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
	-	`sha256:342f11d60b1e5fa9671af8474bbd959d419fc7ad2fd68d2f9b096acae58fb560`  
		Last Modified: Wed, 29 Nov 2023 06:28:25 GMT  
		Size: 11.9 MB (11892334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b3e82cff54cc371f8552487e2d528f14c27ee8177e768fc784e286128258db`  
		Last Modified: Wed, 29 Nov 2023 06:28:24 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec926eb426a4a498f7ee46020e53da3210bb124c47ebb568206828ac272aa1ae`  
		Last Modified: Wed, 29 Nov 2023 06:28:25 GMT  
		Size: 2.9 MB (2927451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584731dc8f3423243e3a1edb28ddda797f30af870166aba027a958f65b193af4`  
		Last Modified: Fri, 01 Dec 2023 20:05:52 GMT  
		Size: 3.6 MB (3596766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; arm variant v5

```console
$ docker pull hylang@sha256:5a9b651927e63845e07958d6d4493c124f3bb75c2d99c4b45aff456f125178fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47761261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96d4071fca04fe28eb60b9290d96f21e11201157f19a8aa6ec059f80f3fe91f`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 21:17:19 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 21:17:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_VERSION=3.9.18
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:38:24 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:38:25 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:38:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:38:38 GMT
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
	-	`sha256:bb7edb6cc29c8c2bb1971e89cf461ce74764464c11876d3f4e1255d79c615824`  
		Last Modified: Wed, 29 Nov 2023 07:55:06 GMT  
		Size: 11.4 MB (11432052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444bd7253a9eb93189f5e554f45506d9eb2a885d620e73e23ecdae7396307a25`  
		Last Modified: Wed, 29 Nov 2023 07:55:05 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c28d687aa6bd031e6574f7ebb5266b33e624e044348b484b1c7c187016886`  
		Last Modified: Wed, 29 Nov 2023 07:55:06 GMT  
		Size: 2.9 MB (2927137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d835eefa105b624af912e97258f60e7be8e41a7723d127f929b388f34942c`  
		Last Modified: Fri, 01 Dec 2023 19:41:47 GMT  
		Size: 3.6 MB (3596630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; arm variant v7

```console
$ docker pull hylang@sha256:d23c5003934341b4f32b5fb02e0aec7152ba1bd5732228256e7d7d16cec1271a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45025083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3a7d8f8ee9fe7f3f4a01e0c1cc34e6a7d04f4b763aa2825c9e400b4a8131d`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 21:17:19 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 21:17:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_VERSION=3.9.18
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:52:07 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:52:07 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:52:21 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:52:22 GMT
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
	-	`sha256:b02daa219669c537bc27c4741d04a00d150b288ecfe1eb7833657bb77d12e61a`  
		Last Modified: Wed, 29 Nov 2023 10:13:27 GMT  
		Size: 11.0 MB (11034114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e300b93db1aff3af9597907849985824ecda88f14d5e17ef7a3126bd8959005c`  
		Last Modified: Wed, 29 Nov 2023 10:13:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dae08ed3186c08d5c832e5e7b4a84bca8c0b2de1cd5954e6ff236f9eccc562`  
		Last Modified: Wed, 29 Nov 2023 10:13:27 GMT  
		Size: 2.9 MB (2926824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b227b0f8110570f7ec6b2528fbbf687edacfed097e61c5a5fd1e3e53c95c7`  
		Last Modified: Fri, 01 Dec 2023 19:59:26 GMT  
		Size: 3.6 MB (3596578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:a3163212ba0d6eddbb11e016061ef80076f12090470603d1455953ca8766f319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51100113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c617e6aabc04339494e7b35a66b89c2942b3bfd794a316f6f2ea13f6638393`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:44:51 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_VERSION=3.9.18
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
CMD ["python3"]
# Wed, 22 Nov 2023 04:28:42 GMT
ENV HY_VERSION=0.27.0
# Wed, 22 Nov 2023 04:28:42 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 22 Nov 2023 04:28:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 22 Nov 2023 04:28:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4906d053db500056f4d92f6658d5c6d9db98074ff2543087ba68e029166b327`  
		Last Modified: Tue, 21 Nov 2023 19:44:41 GMT  
		Size: 3.3 MB (3327658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f2a3e07ca3a1643f7a7819930fe05b448932dd03f1ed78931412b6aa42c9f4`  
		Last Modified: Wed, 22 Nov 2023 04:14:56 GMT  
		Size: 11.9 MB (11862563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14107c73f8cc081c57e1a39e33b7d72a86fa4d2d6b175834cd4a3f3408935b19`  
		Last Modified: Wed, 22 Nov 2023 04:14:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b3200af26cc5db55b20ac852a05e47b5c19d74787d18d879244ba12364769`  
		Last Modified: Wed, 22 Nov 2023 04:14:54 GMT  
		Size: 3.1 MB (3133883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979a58b839bfb40c6efe916961aa455eddcf149d64c948a4709540dcfc42b412`  
		Last Modified: Wed, 22 Nov 2023 04:35:00 GMT  
		Size: 3.6 MB (3596488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; 386

```console
$ docker pull hylang@sha256:f2dfba3579b65079493447c9dba966120ca88c78fc2a33e68d3c4010ceffff2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52554483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ef1d3cd39f9a77707729e65313fe588de7703d8b80ae722ac146081352d7b9`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:44:51 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_VERSION=3.9.18
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
CMD ["python3"]
# Wed, 22 Nov 2023 08:29:51 GMT
ENV HY_VERSION=0.27.0
# Wed, 22 Nov 2023 08:29:51 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 22 Nov 2023 08:30:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 22 Nov 2023 08:30:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8102c4750038de6474e21ba207b80bb8be15dbf37f6ef9e462b18c751496cd59`  
		Last Modified: Wed, 22 Nov 2023 00:58:35 GMT  
		Size: 3.5 MB (3505438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0388e64302f0a6ec26174388aab35cde7d36936d802276b7b4c3aaf54a19de`  
		Last Modified: Wed, 22 Nov 2023 01:02:42 GMT  
		Size: 12.2 MB (12154408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5235608d51fc903872e91fd2ed0e77a84b3e2e88e2c21665d252ebc508046ea1`  
		Last Modified: Wed, 22 Nov 2023 01:02:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820d5b5dd78c85c741efc3dc13c7ab1a7c8e3b57add634cb7994ff972a34f01a`  
		Last Modified: Wed, 22 Nov 2023 01:02:40 GMT  
		Size: 3.1 MB (3133427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce06bf14e453946c50b8947065ed28ca839d05f226fbd8709d7ae29e56c97b44`  
		Last Modified: Wed, 22 Nov 2023 08:38:33 GMT  
		Size: 3.6 MB (3596858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; mips64le

```console
$ docker pull hylang@sha256:634425fe977d7b9c2c2aab942fecca0437e678f079a7d2727910cbc4eac67e9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50046253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c193ac5907fb51f1c7d44df2ec9d4a3c5f8092033f4c9b105d6ab201059827c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:44:51 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_VERSION=3.9.18
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
CMD ["python3"]
# Thu, 23 Nov 2023 00:09:37 GMT
ENV HY_VERSION=0.27.0
# Thu, 23 Nov 2023 00:09:40 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 23 Nov 2023 00:10:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Nov 2023 00:10:49 GMT
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
	-	`sha256:c040426ee3a87dc27e63a33897efc7da389e7d984b3481af2c3bcc0599e722e1`  
		Last Modified: Wed, 22 Nov 2023 06:56:27 GMT  
		Size: 11.7 MB (11672901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a95faf2d3105d78f3685ed263e86e085a4aec2e64145a1b8e693d7eef5523c6`  
		Last Modified: Wed, 22 Nov 2023 06:56:18 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e719b9f45ca82544068e4c223ecf8d222043adbab54261ee9ac381f13a4994`  
		Last Modified: Wed, 22 Nov 2023 06:56:22 GMT  
		Size: 2.9 MB (2927884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca525e52b16574f6d06ddd1418d9b41f319404146bc590105f27adacaf33162b`  
		Last Modified: Thu, 23 Nov 2023 00:15:47 GMT  
		Size: 3.6 MB (3595547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; ppc64le

```console
$ docker pull hylang@sha256:b77a7195cb537aa3409b2bf6e1221d3c020036ec2c9e5e1bf296a71a28e9bee0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55654802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c405f931eb4a4bfe56cbac0e3600206b35efd35d82b6e8f5a9279f5a9070bd7`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 21 Oct 2023 21:17:19 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["bash"]
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 21:17:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_VERSION=3.9.18
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py
# Sat, 21 Oct 2023 21:17:19 GMT
ENV PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6
# Sat, 21 Oct 2023 21:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Sat, 21 Oct 2023 21:17:19 GMT
CMD ["python3"]
# Fri, 01 Dec 2023 19:57:07 GMT
ENV HY_VERSION=0.27.0
# Fri, 01 Dec 2023 19:57:07 GMT
ENV HYRULE_VERSION=0.4.0
# Fri, 01 Dec 2023 19:57:28 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Fri, 01 Dec 2023 19:57:29 GMT
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
	-	`sha256:283237411142161a5eb2901490b190b2fe26ccb95bd9134411bf31fda2055cdf`  
		Last Modified: Wed, 29 Nov 2023 08:24:00 GMT  
		Size: 12.5 MB (12475026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1708a5e092023e368289aee1f67dbdffce6489b418c42a7c621ccdf41b1d5cda`  
		Last Modified: Wed, 29 Nov 2023 08:23:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0e837e4170e5d73325711cc83478fe3f40bd00651574dfa6d08286827bdd6`  
		Last Modified: Wed, 29 Nov 2023 08:24:00 GMT  
		Size: 2.9 MB (2928405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730d4c82e6ede78cede2bc0784c181e529af0c62bf4bdc14d14a8801bd0d0a6e`  
		Last Modified: Fri, 01 Dec 2023 20:06:14 GMT  
		Size: 3.6 MB (3596822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-python3.9-bookworm` - linux; s390x

```console
$ docker pull hylang@sha256:f3d483b07a46e21c5b2c9bdd6bed473ae10c6af8588f4d510c49f22bad6053fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49194395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4686fea5deb84faafa014d3bf84213487cbe37cb0bdaffd3ac0acba4afa2728c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Oct 2023 02:44:51 GMT
ENV LANG=C.UTF-8
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_VERSION=3.9.18
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); printf "*%s\n", so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_PIP_VERSION=23.0.1
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c6add47b0abf67511cdfb4734771cbab403af062/public/get-pip.py
# Mon, 16 Oct 2023 02:44:51 GMT
ENV PYTHON_GET_PIP_SHA256=22b849a10f86f5ddf7ce148ca2a31214504ee6c83ef626840fde6e5dcd809d11
# Mon, 16 Oct 2023 02:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Mon, 16 Oct 2023 02:44:51 GMT
CMD ["python3"]
# Tue, 21 Nov 2023 18:29:50 GMT
ENV HY_VERSION=0.27.0
# Tue, 21 Nov 2023 18:29:50 GMT
ENV HYRULE_VERSION=0.4.0
# Tue, 21 Nov 2023 18:30:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 21 Nov 2023 18:30:03 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975f3e8f619807a631887210a50f86925e11aef820b6ec79197b248cbe866bce`  
		Last Modified: Tue, 21 Nov 2023 15:04:43 GMT  
		Size: 3.2 MB (3169517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b697408117aa8b5709289f8bf8d31e61dcbb6f47696b806da5f6f1b3ddda263`  
		Last Modified: Tue, 21 Nov 2023 15:07:29 GMT  
		Size: 11.8 MB (11781556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121bd1aaa32f86aebb615006df784b27239e58de63949d80e5307e7db91db69b`  
		Last Modified: Tue, 21 Nov 2023 15:07:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec95c6591a914249835c552e031b50fc033c0a2f77357219ab689ea2da28e75`  
		Last Modified: Tue, 21 Nov 2023 15:07:28 GMT  
		Size: 3.1 MB (3133476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891aebea9d9e08ac1f2bf36011d6a21842dfe0645bba0f37e097b410ef648e00`  
		Last Modified: Tue, 21 Nov 2023 18:34:14 GMT  
		Size: 3.6 MB (3596717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
