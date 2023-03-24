## `hylang:python3.11-buster`

```console
$ docker pull hylang@sha256:351d8565ef662ee1e1b0c3ffa6471e17a79a10a2a3f374dde83d9e9b090ca830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:python3.11-buster` - linux; amd64

```console
$ docker pull hylang@sha256:64070d40b7bf75e37a83afffc9210f926b9a4955bbe04ddfdfcc69e8c5d32302
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51404291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90998021059880564e8a2dba60b23d635cb06fbc607ac0f3ed1eab91d96b1c5d`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 01:30:51 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 01:30:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 23 Mar 2023 01:30:51 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 23 Mar 2023 01:30:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Thu, 23 Mar 2023 01:30:51 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Thu, 23 Mar 2023 01:30:51 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Thu, 23 Mar 2023 01:30:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 18:03:14 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 18:03:14 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 18:03:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 18:03:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8cd5f36469921b82be5c046d0fe82365de8fcee96a4caa8259939d06d99bef`  
		Last Modified: Thu, 23 Mar 2023 05:41:22 GMT  
		Size: 2.8 MB (2782122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80384e04044fa9b6493f2c9012fd1aa7035ab741147248930b5a2b72136198b1`  
		Last Modified: Thu, 23 Mar 2023 05:42:48 GMT  
		Size: 12.0 MB (11990866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe06c6a3fe34fe65c406b3dfcd8f504972ef83a65287a88d2be3bbe81eeaf56`  
		Last Modified: Thu, 23 Mar 2023 05:42:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0712d0bdb159c54d5bdce952fbb72c5a5d2a4399654d7f55b004d9fc01e189e`  
		Last Modified: Thu, 23 Mar 2023 05:42:46 GMT  
		Size: 3.4 MB (3369508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ee5f2ca3ec66bd4d06fde833867aca1017dcbb560db3ec191a9f52993c192`  
		Last Modified: Thu, 23 Mar 2023 18:13:15 GMT  
		Size: 6.1 MB (6121681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.11-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:ab0dd83cd0ea728414856ee503ba546e80e2cfb9b9907328d9abe2e5e3170600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45862092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca8c3fbe4ed5ce07ae1c316a8f03a8108379c3091db0c04ef210c71a56b4c88`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:33 GMT
ADD file:b3a5424864097d73516302c7e0a8fe9394880555c85f25a82a020ec3fc887eb8 in / 
# Thu, 23 Mar 2023 01:20:34 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 01:20:34 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 01:20:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 23 Mar 2023 01:20:34 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 23 Mar 2023 01:20:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Thu, 23 Mar 2023 01:20:34 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Thu, 23 Mar 2023 01:20:34 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Thu, 23 Mar 2023 01:20:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Thu, 23 Mar 2023 01:20:34 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 16:51:10 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 16:51:10 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 16:51:22 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 16:51:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:369fe072796976e1501c1a8d490c05b9ac47287c34c004013e0982d2dd4bb7c2`  
		Last Modified: Thu, 23 Mar 2023 01:33:32 GMT  
		Size: 22.7 MB (22748632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78c571d500d0a096c013129bff2bbd0c1b02e6d17def7a936bdc92a847c6d03`  
		Last Modified: Thu, 23 Mar 2023 07:41:16 GMT  
		Size: 2.4 MB (2370028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a90c7bccfe2a07915d63638d4248d3961c552682de5645563b081549e35ca4`  
		Last Modified: Thu, 23 Mar 2023 07:41:17 GMT  
		Size: 11.3 MB (11252580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc21b8e5892c502e531d52fb00e83037efb833783f5adc35851a93a43f9c81`  
		Last Modified: Thu, 23 Mar 2023 07:41:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700afc783937d693f17867038d80aa6b748c3cc3b53cf0f44db6b8d647f19140`  
		Last Modified: Thu, 23 Mar 2023 07:41:16 GMT  
		Size: 3.4 MB (3368827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebb3f5022d7fd4f3cea1b849887a45ce196c3b1ba42318717ff41973c5f2b27`  
		Last Modified: Thu, 23 Mar 2023 16:58:02 GMT  
		Size: 6.1 MB (6121783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.11-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:c7005cf55df433f29ebd2e9f88e947850be9ad28b404a84e89c47e9012fc17f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50144923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6435eef810f7bf7f933dc5d0ef26a3fa2bb3ee5030a5364db9c57e97b35916`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:45:23 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 00:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 23 Mar 2023 00:45:23 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 23 Mar 2023 00:45:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Thu, 23 Mar 2023 00:45:23 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Thu, 23 Mar 2023 00:45:23 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Thu, 23 Mar 2023 00:45:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 15:06:22 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 15:06:22 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 15:06:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 15:06:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e11a7826c6ce9b3366e1d2c4dfbdec39133e62fe15bca830f2947fd1064b6c`  
		Last Modified: Thu, 23 Mar 2023 05:31:52 GMT  
		Size: 2.6 MB (2648728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a79e484c85524a9518ed521a6da01406628e5c55cec47c59102370156207769`  
		Last Modified: Thu, 23 Mar 2023 05:33:13 GMT  
		Size: 12.1 MB (12082369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512300f3f60f5881c40788691060131b98ea2ddd1218c3d40ecaf8257728cc2`  
		Last Modified: Thu, 23 Mar 2023 05:33:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d0b90d56060877b3e214d3d7d820594f685a18d1d659e14d0b5d03e8fdce1d`  
		Last Modified: Thu, 23 Mar 2023 05:33:12 GMT  
		Size: 3.4 MB (3369132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0e6af401a84e01daba730090001cbe22c6a0be1d7dbd3bd93ca35450cfb52e`  
		Last Modified: Thu, 23 Mar 2023 15:15:01 GMT  
		Size: 6.1 MB (6121790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.11-buster` - linux; 386

```console
$ docker pull hylang@sha256:d64f21c885b9cb12c5fd47f0790306a0990e4ec4ca83b065dd914086c44e6b01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52154322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a38abb112b4d0cdb47db87acc3f3fa0e8a327b8d7ddd8e50416ce9b963c1f37`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:40 GMT
ADD file:5743625b778ab9036f4eae3e44da6b59db355d7d6d7b8f42fbb71f2b8c428dd7 in / 
# Thu, 23 Mar 2023 00:39:40 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:39:40 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 00:39:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 23 Mar 2023 00:39:40 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PYTHON_VERSION=3.11.2
# Thu, 23 Mar 2023 00:39:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libdb-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version # buildkit
# Thu, 23 Mar 2023 00:39:40 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Thu, 23 Mar 2023 00:39:40 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Thu, 23 Mar 2023 00:39:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Thu, 23 Mar 2023 00:39:40 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 23:47:53 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 23:47:53 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 23:48:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 23:48:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:0a3d55947c3a2af51034409d456cfd83f620450381a4b036d86b0db1b8b0aaf8`  
		Last Modified: Thu, 23 Mar 2023 00:43:56 GMT  
		Size: 27.8 MB (27798660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c70637e20a88924d41c9d0cb225ed274b518f2fd1a4e3d798534f2f495b288`  
		Last Modified: Thu, 23 Mar 2023 08:25:10 GMT  
		Size: 2.8 MB (2790382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6906d94841776cc732b6f8c9e08e273b0607934c1dba725ce7af24dde3cc320`  
		Last Modified: Thu, 23 Mar 2023 08:26:43 GMT  
		Size: 12.1 MB (12074016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0ba7a729a7a40ddde5f447c7e0cd96dba659d98ba0adf0e7b4575979312170`  
		Last Modified: Thu, 23 Mar 2023 08:26:41 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d9f4eeb1b96dd338e89145a23407b71a31d5745b1b395f572effe6f816b93`  
		Last Modified: Thu, 23 Mar 2023 08:26:42 GMT  
		Size: 3.4 MB (3369197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b270148de8918cb322cbd87a70e4a0f1d278d913a55212ea092c2a50617fc7`  
		Last Modified: Thu, 23 Mar 2023 23:58:56 GMT  
		Size: 6.1 MB (6121824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
