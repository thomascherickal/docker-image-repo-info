## `hylang:python3.10-buster`

```console
$ docker pull hylang@sha256:fc4c91e07a5c3711d24ecfa57f54537a5c3f180cd5af6203c5b8b10d8a0f1ff4
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

### `hylang:python3.10-buster` - linux; amd64

```console
$ docker pull hylang@sha256:c51124e0107f6d99cf9b708854e872652e0541ce4175085dbed1e46cb0362a24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47873826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5220f83d66ab3882f1b91c12afe6366a1d0bb0a22b12a6c5d586bb10cc20c89e`
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
# Thu, 17 Mar 2022 04:33:44 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 05:26:27 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 05:38:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 05:38:33 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 05:38:33 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 05:38:33 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 05:38:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 05:38:33 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 05:38:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 05:38:45 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 07:07:29 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 07:07:29 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 07:07:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 07:07:32 GMT
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
	-	`sha256:664de1b4b763c99c50294f3ec811f94a5ec6f6eeac2370b3f688b9ea41658942`  
		Last Modified: Thu, 17 Mar 2022 07:02:47 GMT  
		Size: 11.7 MB (11668338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d2d88092f48ca5bf240b9f660ec4f5ec2af737657d9ebc85de8cba66b46ad5`  
		Last Modified: Thu, 17 Mar 2022 07:02:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32edb68a7223d212314f937b5419495b2d56a25d26f7eca1b98936848eb4d40`  
		Last Modified: Thu, 17 Mar 2022 07:02:46 GMT  
		Size: 3.2 MB (3163465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39c73756f113d62922e5a77229f768954e5e1ddd5a021b65296e788e4ebb112`  
		Last Modified: Thu, 17 Mar 2022 07:10:45 GMT  
		Size: 3.1 MB (3117800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:bd96b83ee4a61d095ed4bdd8a76719e274bb357fcc11baaf4a24e202ff8fcdd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44982947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b837d1ab7337b6ae989a4b8681a91d22c3b732d844beddd615a65b0f32689e`
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
# Thu, 17 Mar 2022 05:49:09 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 07:06:25 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 07:39:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 07:40:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 07:40:02 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 07:40:03 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 07:40:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 07:40:05 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 07:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 07:40:46 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 09:23:52 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 09:23:53 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 09:24:00 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 09:24:01 GMT
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
	-	`sha256:a62da156176df6968db5c0abbcadc8fc7cb9fd4cf640807ceafee3c8003381d7`  
		Last Modified: Thu, 17 Mar 2022 09:20:19 GMT  
		Size: 11.4 MB (11354727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd573826ee8653104b7afcaad9015947b9883a3fb5a479a9bbca3037c08eb07`  
		Last Modified: Thu, 17 Mar 2022 09:20:12 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c203dbdc422691f9d38d642867b053430dfd15034ea01e8c74fa7538d37dda`  
		Last Modified: Thu, 17 Mar 2022 09:20:15 GMT  
		Size: 3.2 MB (3163136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2827ad3f82c977df6efaa5535e1c683f1a3b5888377ca27f3d919616b8352eb2`  
		Last Modified: Thu, 17 Mar 2022 09:28:35 GMT  
		Size: 3.1 MB (3118029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:64606a615ec93d182ab538b89a536df4a44a869d044061eea8892388f50cd2e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42252570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b13d42574915c1bacf88a65f25c18470f47e5d9fa8a079de5496aae2272ca3`
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
# Thu, 17 Mar 2022 10:53:18 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 13:07:44 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 13:40:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 13:40:58 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 13:40:58 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 13:40:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 13:40:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 13:40:59 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 13:41:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 13:41:29 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 17:24:53 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 17:24:54 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 17:25:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 17:25:02 GMT
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
	-	`sha256:06204f77a27b8bc9371840a7d5934264e4730b7670c8e060603273c1ff538a52`  
		Last Modified: Thu, 17 Mar 2022 17:15:24 GMT  
		Size: 10.9 MB (10857795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5a308dbabdec94b2a86ac1cb33f4b437fe4846a99abf03ae0df4ea5e64799b`  
		Last Modified: Thu, 17 Mar 2022 17:15:18 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e62c7c296b53b9f510a05a4a1e0fb53602981fce55449a9865792ab53b3dc31`  
		Last Modified: Thu, 17 Mar 2022 17:15:21 GMT  
		Size: 3.2 MB (3163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff843359211bc953d6c1ccc06af019dd2d64df9fbae6789a88bc8ae4f5c97382`  
		Last Modified: Thu, 17 Mar 2022 17:34:47 GMT  
		Size: 3.1 MB (3118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:bf5fdb3f49a72d93beca04d3d1a459e1a9868b9b3359e9fd6f38df2cf3950dea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46281359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6dcd84c756cd2b19142a9c922dc94e0b059c72119138a7e5e279ce35ca6f0c4`
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
# Thu, 17 Mar 2022 03:50:50 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 04:30:13 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 04:40:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 04:40:09 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 04:40:10 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 04:40:11 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 04:40:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 04:40:13 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 04:40:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 04:40:31 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 05:52:52 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 05:52:53 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 05:52:57 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 05:52:57 GMT
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
	-	`sha256:e5e06520705927533f596ddec5e7da32822f5c967b17d3c7c8dbc8f6a94dee69`  
		Last Modified: Thu, 17 Mar 2022 05:47:54 GMT  
		Size: 11.7 MB (11658417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c86fa8ed079d6b5a85e5d70f9b646767a76093a1c9808b589cefba67b066eb`  
		Last Modified: Thu, 17 Mar 2022 05:47:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f1eacc22d6d77f1a18bd39e5c15cb3fe1734373a0c722dff0800771a5f9a4`  
		Last Modified: Thu, 17 Mar 2022 05:47:53 GMT  
		Size: 2.9 MB (2947265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c9f2f6307b6023a7f32712bc8bd1b9cd63b9149a28d51aa7dc60b78ddc0072`  
		Last Modified: Thu, 17 Mar 2022 05:58:44 GMT  
		Size: 3.1 MB (3116100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; 386

```console
$ docker pull hylang@sha256:5197cc7d603a7465fcab8c656e75b91491b8263f4a28d32fc3410093c616107d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48448557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b70ebc6bd372580ff324424159f44dd5995d89b02a15c50a76a21e17d9d7075`
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
# Thu, 24 Mar 2022 01:52:36 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 24 Mar 2022 03:25:46 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 24 Mar 2022 03:38:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 24 Mar 2022 03:38:46 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 24 Mar 2022 03:38:47 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 24 Mar 2022 03:38:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 24 Mar 2022 03:38:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 24 Mar 2022 03:38:50 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 24 Mar 2022 03:39:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 24 Mar 2022 03:39:05 GMT
CMD ["python3"]
# Thu, 24 Mar 2022 14:42:02 GMT
ENV HY_VERSION=1.0a4
# Thu, 24 Mar 2022 14:42:02 GMT
ENV HYRULE_VERSION=0.1
# Thu, 24 Mar 2022 14:42:06 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 24 Mar 2022 14:42:07 GMT
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
	-	`sha256:5722d3b2221dec54c902777eb063e2aa2c9ec0e8696ee3df464dd4770cbb69ce`  
		Last Modified: Thu, 24 Mar 2022 06:06:47 GMT  
		Size: 11.8 MB (11798942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc2ecd697a3df9959fdb035e8ed0334f778e0c5cf06a9403942fe6b562dd19`  
		Last Modified: Thu, 24 Mar 2022 06:06:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5603c434663023e5de439242eae22a6c06998ae529823cda85bb8cb86fd4690e`  
		Last Modified: Thu, 24 Mar 2022 06:06:46 GMT  
		Size: 2.9 MB (2947305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b68a57bc3c2ef7cdcf0678b70a26027cdd42c10c61d2b05d1015bcdd9e81e44`  
		Last Modified: Thu, 24 Mar 2022 14:49:12 GMT  
		Size: 3.1 MB (3116293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:25d147c5d3d837df9f5901076b4ba2e4583c84d6111821e4dc027b4c5dae71d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52213363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a0539b7dd065899b751cf01a53ae41735cf9729a3cdf78461657dc4f5f98242`
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
# Thu, 17 Mar 2022 12:45:34 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 14:29:02 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 14:57:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 14:57:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 14:57:32 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 14:57:35 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 14:57:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 14:57:42 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 14:58:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 14:58:29 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 18:22:37 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 18:22:45 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 18:23:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 18:23:27 GMT
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
	-	`sha256:77f1d18912fe0e5741c5e5a4f819a57fa77c8ab5b0281fcb7f5bbe14b2f62ecd`  
		Last Modified: Thu, 17 Mar 2022 18:12:43 GMT  
		Size: 12.5 MB (12479849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b724cecd529ab0e9ad7db96190d91ed7da8945cf3767491121114709d6428b8`  
		Last Modified: Thu, 17 Mar 2022 18:12:40 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823afb80fadefb6cc30e28b3abdcdc67ad35518527daa622b7e144141ae62076`  
		Last Modified: Thu, 17 Mar 2022 18:12:42 GMT  
		Size: 3.2 MB (3165054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e1d0301a847d8f6f30f3715b6f995c094caf425b3741c78143ef8cd5b382b5`  
		Last Modified: Thu, 17 Mar 2022 18:40:13 GMT  
		Size: 3.1 MB (3118206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:python3.10-buster` - linux; s390x

```console
$ docker pull hylang@sha256:0d32e3c33c3dd934a821dab332436746102b691cd3555ef658c5991bc7107877
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45981123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d58a22d6deaa5ddaafc51acee2ab8bb5a7f6a5fed131705236523fec39736a9e`
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
# Thu, 17 Mar 2022 03:28:13 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 17 Mar 2022 03:56:08 GMT
ENV PYTHON_VERSION=3.10.3
# Thu, 17 Mar 2022 04:04:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 17 Mar 2022 04:04:29 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "/usr/local/bin/$src" "/usr/local/bin/$dst"; 	done
# Thu, 17 Mar 2022 04:04:29 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 17 Mar 2022 04:04:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 17 Mar 2022 04:04:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 17 Mar 2022 04:04:29 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 17 Mar 2022 04:04:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 17 Mar 2022 04:04:39 GMT
CMD ["python3"]
# Thu, 17 Mar 2022 05:12:13 GMT
ENV HY_VERSION=1.0a4
# Thu, 17 Mar 2022 05:12:13 GMT
ENV HYRULE_VERSION=0.1
# Thu, 17 Mar 2022 05:12:16 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 17 Mar 2022 05:12:17 GMT
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
	-	`sha256:aac00e4e3208741af5592ab43e2f9a13bef281b846e2975ddf6a2fc328dc79f7`  
		Last Modified: Thu, 17 Mar 2022 05:09:10 GMT  
		Size: 11.5 MB (11471763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7124c56c0fb12d55fa2dedf1875e3e3beb443feee7f20e3a373d58f917b76a3`  
		Last Modified: Thu, 17 Mar 2022 05:09:09 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df37fb8a41bc6875e3d85283a11b7b820fc3d88715af8ddbf5fe3269feb940e2`  
		Last Modified: Thu, 17 Mar 2022 05:09:09 GMT  
		Size: 3.2 MB (3162814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb40e18a15de7ebc0dea491d81f53418ab3eb06d3b1fded2c6a9cf910840ecb`  
		Last Modified: Thu, 17 Mar 2022 05:17:18 GMT  
		Size: 3.1 MB (3117707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
