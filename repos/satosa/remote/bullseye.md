## `satosa:bullseye`

```console
$ docker pull satosa@sha256:b2ead7d73de69e81ae1a2a2f52d2da56c40cf38f4fc7e40dd34b87376e301d70
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

### `satosa:bullseye` - linux; amd64

```console
$ docker pull satosa@sha256:4950b9d5259dc004f395b4d3ce755c24ce74e2927fbf4932ae23295b011f145f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82835727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd991f722e8b69b9303d112a0778505af47c34eac32a9fd648ed9643d96dd31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:41:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:41:52 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:41:57 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 14:36:15 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 14:46:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 14:46:46 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 14:46:46 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 14:46:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 14:46:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 14:46:46 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 14:46:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 14:46:58 GMT
CMD ["python3"]
# Thu, 06 Oct 2022 03:39:18 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Thu, 06 Oct 2022 03:39:18 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 06 Oct 2022 03:40:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 06 Oct 2022 03:40:21 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 06 Oct 2022 03:40:21 GMT
WORKDIR /etc/satosa
# Thu, 06 Oct 2022 03:40:21 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 06 Oct 2022 03:40:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 03:40:22 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 03:40:22 GMT
USER satosa:satosa
# Thu, 06 Oct 2022 03:40:22 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08aeb7fd50562d57cef1a49d6197d619df0b4ce52e4caeba2402c27c6e536b`  
		Last Modified: Wed, 05 Oct 2022 16:33:56 GMT  
		Size: 1.1 MB (1076333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30527e10f55af538c1464ce755f9e9fceae68bb639f9b8211cfaf3c11e83ba42`  
		Last Modified: Wed, 05 Oct 2022 16:35:00 GMT  
		Size: 12.1 MB (12108136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693e7a5ba2a8a42880d04042159d67aa9ebb2d67864b7b419fe2847294c080a2`  
		Last Modified: Wed, 05 Oct 2022 16:34:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b6f7685fa51adb5da18c9a4fd647bc9cb24af571c32a824206e8a9277d7b09`  
		Last Modified: Wed, 05 Oct 2022 16:34:59 GMT  
		Size: 3.3 MB (3336145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5da338bab701b4cc39b4904cc4f88b9b9f8fb5fe46eb139f181c8376744651`  
		Last Modified: Thu, 06 Oct 2022 03:40:56 GMT  
		Size: 19.6 MB (19588779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87760b871691aafb645a03796037a67e78b5d95c73022972eef55d8d8ae8de5f`  
		Last Modified: Thu, 06 Oct 2022 03:40:56 GMT  
		Size: 15.3 MB (15294443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5cab8f7e45b29bdabd4abe2472c0e0ac66512c16d66554860253d2d7469435`  
		Last Modified: Thu, 06 Oct 2022 03:40:53 GMT  
		Size: 9.4 KB (9441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8792810adeced91dfe1d4feaf1939f5c231a83334264c73d1ddaadc85e60ace1`  
		Last Modified: Thu, 06 Oct 2022 03:40:52 GMT  
		Size: 2.1 KB (2114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; arm variant v5

```console
$ docker pull satosa@sha256:171d8cae1705b40d0bca7392711073bc204a5556b2a78e16f9bf3ccfc9a65157
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191863034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d51ce9209abeeec0fb5f679b04d79796aa0a30a3707c783daa94319b6a98887`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:05:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 12:05:50 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 12:06:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:06:00 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 13 Sep 2022 13:02:13 GMT
ENV PYTHON_VERSION=3.10.7
# Tue, 13 Sep 2022 13:26:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Tue, 13 Sep 2022 13:26:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 13 Sep 2022 13:26:31 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Tue, 13 Sep 2022 13:26:31 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 13 Sep 2022 13:26:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Tue, 13 Sep 2022 13:26:31 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Tue, 13 Sep 2022 13:26:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 13 Sep 2022 13:26:49 GMT
CMD ["python3"]
# Tue, 13 Sep 2022 19:56:33 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Tue, 13 Sep 2022 19:56:33 GMT
ENV SATOSA_VERSION=8.1.1
# Tue, 13 Sep 2022 20:03:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Tue, 13 Sep 2022 20:03:58 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Tue, 13 Sep 2022 20:03:58 GMT
WORKDIR /etc/satosa
# Tue, 13 Sep 2022 20:03:58 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Tue, 13 Sep 2022 20:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 20:03:58 GMT
EXPOSE 8080
# Tue, 13 Sep 2022 20:03:58 GMT
USER satosa:satosa
# Tue, 13 Sep 2022 20:03:59 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34e46f8b0011c17d76258124294fbd3b83ccc08b49bd5ba31077d0409c1a5d`  
		Last Modified: Tue, 13 Sep 2022 14:47:49 GMT  
		Size: 1.1 MB (1059688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bdd65de5710dfc2501f893f3233d49521392638b4a3b2ae84366ff4c86056c`  
		Last Modified: Tue, 13 Sep 2022 14:48:41 GMT  
		Size: 11.7 MB (11686263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358951f041e406933698d182eb2b9a911cd5b92eaf1016b8e4309d96c7407772`  
		Last Modified: Tue, 13 Sep 2022 14:48:37 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41065f57acef74f68f1a86ef17b8c01933dcb21364f69d26d8267b3884996472`  
		Last Modified: Tue, 13 Sep 2022 14:48:39 GMT  
		Size: 3.3 MB (3335652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca267a55d1107a4db9587ad0de566898103674ab57b8a8cbccb439ee04ec91`  
		Last Modified: Tue, 13 Sep 2022 20:04:37 GMT  
		Size: 21.2 MB (21231162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a8c6daf99168e9657e4fb6171951b8b07d4d6192949e1f92097b05f3160be4`  
		Last Modified: Tue, 13 Sep 2022 20:04:50 GMT  
		Size: 125.6 MB (125633187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc1d927ae599ba332225b5305154ed8271b2701ffc605ffc72eb29aaa0f5022`  
		Last Modified: Tue, 13 Sep 2022 20:04:29 GMT  
		Size: 9.4 KB (9445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ff7f03cfe2bd5aeddd462908b5b4a1b7ef004c20072d910df4313925fc9d61`  
		Last Modified: Tue, 13 Sep 2022 20:04:29 GMT  
		Size: 2.1 KB (2116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; arm variant v7

```console
$ docker pull satosa@sha256:2bb77ab086fe1eb94551d47b9c2f22bf04c36cefba061310143076b4e569d08b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251790531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34998988c63f40abdd303119344ef2f589df76cd163a7595eb44885366b9d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 23:26:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 23:26:23 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 23:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 23:26:29 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 06 Oct 2022 01:09:13 GMT
ENV PYTHON_VERSION=3.10.7
# Thu, 06 Oct 2022 01:25:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Thu, 06 Oct 2022 01:25:14 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 06 Oct 2022 01:25:14 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Thu, 06 Oct 2022 01:25:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Thu, 06 Oct 2022 01:25:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Thu, 06 Oct 2022 01:25:15 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Thu, 06 Oct 2022 01:25:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 06 Oct 2022 01:25:27 GMT
CMD ["python3"]
# Fri, 07 Oct 2022 03:35:26 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Fri, 07 Oct 2022 03:35:26 GMT
ENV SATOSA_VERSION=8.1.1
# Fri, 07 Oct 2022 03:43:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Fri, 07 Oct 2022 03:43:26 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Fri, 07 Oct 2022 03:43:26 GMT
WORKDIR /etc/satosa
# Fri, 07 Oct 2022 03:43:27 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 03:43:27 GMT
EXPOSE 8080
# Fri, 07 Oct 2022 03:43:27 GMT
USER satosa:satosa
# Fri, 07 Oct 2022 03:43:27 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f5ae95fa5f771d4156b88644cb100d08cf8b431fb078c59871220f226a6fe9`  
		Last Modified: Thu, 06 Oct 2022 03:57:25 GMT  
		Size: 1.0 MB (1041608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028449ad44dfe50a3ab6cb3ec0c675ae38ef08d3513dc26922471bd610e7d185`  
		Last Modified: Thu, 06 Oct 2022 03:58:44 GMT  
		Size: 11.2 MB (11205291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff29165ae8b3d5b1d18d752f6ecf14b05eaae12fcfa9b20ace63026773eab8ac`  
		Last Modified: Thu, 06 Oct 2022 03:58:42 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f920d3aa94f9e8646adf10f3ae1265e2ea06d76b06d7238b1ea1491881c3e082`  
		Last Modified: Thu, 06 Oct 2022 03:58:43 GMT  
		Size: 3.3 MB (3335682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa6103a3af68ef515876198148030d3df493c93b1e11b7a18af20238f0b9519`  
		Last Modified: Fri, 07 Oct 2022 03:50:21 GMT  
		Size: 21.0 MB (20961380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578240c43eebc7b306800815f96d206aa4fa66604145044ec388ebf8ba2656a`  
		Last Modified: Fri, 07 Oct 2022 03:50:43 GMT  
		Size: 188.7 MB (188655581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040a195fdbea96bd078e908f3911816178f987b6ec8ef2008f75666cdd37b1d1`  
		Last Modified: Fri, 07 Oct 2022 03:50:14 GMT  
		Size: 9.4 KB (9442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3e0c7bce8839c5175b7299c46340652c3bd456db7b5e6a21a80ce0185250ae`  
		Last Modified: Fri, 07 Oct 2022 03:50:13 GMT  
		Size: 2.1 KB (2115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; arm64 variant v8

```console
$ docker pull satosa@sha256:f21a660311d694040b3a9ffed676beb69acf8df1d6872e511a300c45a53987ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (79983656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4196584ba1382e4f2a15f1633a2c903b6332eb083a726d52748ee18ce8dba5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:45:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 09:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:45:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:45:55 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 10:44:21 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 10:54:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 10:54:28 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 10:54:29 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 10:54:30 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 10:54:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 10:54:32 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 10:54:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 10:54:44 GMT
CMD ["python3"]
# Thu, 06 Oct 2022 02:00:04 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Thu, 06 Oct 2022 02:00:05 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 06 Oct 2022 02:00:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 06 Oct 2022 02:00:56 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 06 Oct 2022 02:00:57 GMT
WORKDIR /etc/satosa
# Thu, 06 Oct 2022 02:00:59 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 06 Oct 2022 02:00:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 02:01:00 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 02:01:01 GMT
USER satosa:satosa
# Thu, 06 Oct 2022 02:01:02 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61358e3667e2d11218ffd1160790a79eb2f7cd1fa39485e1de62d4f5e8eb72b0`  
		Last Modified: Wed, 05 Oct 2022 12:30:12 GMT  
		Size: 858.9 KB (858913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be44f5cc50304dbffaf2be8a96f8f2bfe3e4d560151ce2218f872fb2fc5284c6`  
		Last Modified: Wed, 05 Oct 2022 12:31:24 GMT  
		Size: 12.2 MB (12153497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240534457965c86613e0b1d2a79deb50de07039ba4c573caefa67baf8cb3e6a3`  
		Last Modified: Wed, 05 Oct 2022 12:31:22 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a1e1f631d1fdf7200955ac719bcd9f9b4d28e18e4b9d3f9241bfbe724a232`  
		Last Modified: Wed, 05 Oct 2022 12:31:23 GMT  
		Size: 3.1 MB (3119912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0feebdcf2d431a4b5ffbbb0164d31cd64098833886c44a200e567098189b0f5`  
		Last Modified: Thu, 06 Oct 2022 02:01:48 GMT  
		Size: 19.3 MB (19325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a67709009848a5c2c453aba179a08fed1ad162b2e0f910385107c867d2a73d`  
		Last Modified: Thu, 06 Oct 2022 02:01:48 GMT  
		Size: 14.4 MB (14449456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dc1ea77aeaf9d1f48a73b3f746337d2c940cad671f290cfafaaf6b8d2fe3aa`  
		Last Modified: Thu, 06 Oct 2022 02:01:45 GMT  
		Size: 9.4 KB (9394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8deaf951386b463d3af0fdcb77576ba191e69fdaa099e149a05e96705b43d6fc`  
		Last Modified: Thu, 06 Oct 2022 02:01:45 GMT  
		Size: 2.1 KB (2114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; 386

```console
$ docker pull satosa@sha256:cd048e10b45d8236322e6d36620253e4507fbfc52003a4eb56d60d073e451c76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.6 MB (255582289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb42f375b52a74784a07b3c97a0885c23430b86fcfe436b031b10c141f1e49b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:27:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 09:27:32 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:27:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 10:40:52 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 10:52:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 10:52:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 10:52:59 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 10:53:00 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 10:53:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 10:53:02 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 10:53:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 10:53:16 GMT
CMD ["python3"]
# Wed, 05 Oct 2022 18:41:42 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Wed, 05 Oct 2022 18:41:42 GMT
ENV SATOSA_VERSION=8.1.1
# Wed, 05 Oct 2022 18:45:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Wed, 05 Oct 2022 18:45:08 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Wed, 05 Oct 2022 18:45:08 GMT
WORKDIR /etc/satosa
# Wed, 05 Oct 2022 18:45:10 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Wed, 05 Oct 2022 18:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:45:11 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:45:12 GMT
USER satosa:satosa
# Wed, 05 Oct 2022 18:45:13 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f28a2a1499f025201f7bd6169c4443f9c6aca750e71b6d10a78c59ec0c05c08`  
		Last Modified: Wed, 05 Oct 2022 12:51:40 GMT  
		Size: 883.6 KB (883620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dcf5f62d9fa77cf6c19d4b29a8919833ec065e2a36489730035d59aee4345b`  
		Last Modified: Wed, 05 Oct 2022 12:52:52 GMT  
		Size: 12.2 MB (12216448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56352ae122508146f12dd55f58aa182b6fba5e7f8b9b37035d47814f0be31b80`  
		Last Modified: Wed, 05 Oct 2022 12:52:50 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b8f463ee39e1cb071311eda2cd1869dd8d4fb5d1de2a01c769ad74de44b582`  
		Last Modified: Wed, 05 Oct 2022 12:52:51 GMT  
		Size: 3.1 MB (3119783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad10d6fe8971411b9a5dd60e58b80ce162c28e84ff15fe612e09df31ab46cfe`  
		Last Modified: Wed, 05 Oct 2022 18:46:09 GMT  
		Size: 22.6 MB (22587844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a393fca2d7f6e41d7eb5cae123556ad65ddc3033fb54f6d6647eb5215ecf16a2`  
		Last Modified: Wed, 05 Oct 2022 18:46:19 GMT  
		Size: 184.4 MB (184366561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d3694be03514c51e796d860b47adddf04ac40e7bb21310cfffe3b8ded0078`  
		Last Modified: Wed, 05 Oct 2022 18:46:06 GMT  
		Size: 9.4 KB (9395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f2863c24becc534b1571a89fcd9df7855b29e56f15f2d1e185438cc82b7c70`  
		Last Modified: Wed, 05 Oct 2022 18:46:06 GMT  
		Size: 2.1 KB (2116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; mips64le

```console
$ docker pull satosa@sha256:7869114653c49b63541c0e430b330627147440822937087bba1344a692d88ebc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253413661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4bb2b8153f13789e26b42f14845177a46c476553ffd828a51c1b8ee7ce7a5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 21:09:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 21:09:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 21:09:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 21:10:02 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 21:10:04 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 22:27:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 22:27:11 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 22:27:14 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 22:27:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 22:27:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 22:27:21 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 22:28:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 22:28:15 GMT
CMD ["python3"]
# Thu, 06 Oct 2022 12:34:29 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Thu, 06 Oct 2022 12:34:32 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 06 Oct 2022 12:53:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 06 Oct 2022 12:53:49 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 06 Oct 2022 12:53:54 GMT
WORKDIR /etc/satosa
# Thu, 06 Oct 2022 12:53:58 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 06 Oct 2022 12:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 12:54:07 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 12:54:12 GMT
USER satosa:satosa
# Thu, 06 Oct 2022 12:54:17 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c6f8738cd8363c688712476db560fa00fcbfaa51a29dbb3a7cd1f1782329f`  
		Last Modified: Thu, 06 Oct 2022 03:23:26 GMT  
		Size: 844.7 KB (844732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195b2826bc5f1f586d795b8e465e1c89a74db72d4e75288d5083032b99985c1`  
		Last Modified: Thu, 06 Oct 2022 03:23:33 GMT  
		Size: 12.1 MB (12130312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aa2f3e0c90384683db52cffe856f42f45ef87a4315dfbb1d8f9b82c78eb445`  
		Last Modified: Thu, 06 Oct 2022 03:23:25 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e3b3be68722d076acf8e7917c82f88268041920ea92773e8d6fcb7287a0512`  
		Last Modified: Thu, 06 Oct 2022 03:23:29 GMT  
		Size: 3.1 MB (3120628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2938a5686126063a6a7856be8916b4c1cbdeed51a060815141236a5b97c99f4c`  
		Last Modified: Thu, 06 Oct 2022 12:54:46 GMT  
		Size: 21.3 MB (21288961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c871cc11157054ce27021ed1d95438e7b4c3f4c6e171f7f3cf40d26ce38946b0`  
		Last Modified: Thu, 06 Oct 2022 12:55:38 GMT  
		Size: 186.4 MB (186376435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229885e6381952e964f7f628300949bbbd21c68cbd9986c751c9b88f241c0e45`  
		Last Modified: Thu, 06 Oct 2022 12:54:33 GMT  
		Size: 9.4 KB (9395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9dbad4fcdd1421cec7d108f0c86747c2608f8bddc9f321fdbda532971a6711`  
		Last Modified: Thu, 06 Oct 2022 12:54:33 GMT  
		Size: 2.1 KB (2115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; ppc64le

```console
$ docker pull satosa@sha256:621066f458e74d1c7a732b038ac3cbbaff7592fd97bef9d811dbef5ec4c8dd4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258063839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29ab51bb9ebeebd48c1e5cb9e12d903958ba369a27f62ab6d62f7724497ec2f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:14:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 04:14:42 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:14:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:14:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 05:34:53 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 06:07:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 06:07:54 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 06:07:55 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 06:07:55 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 06:07:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 06:07:56 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 06:08:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 06:08:18 GMT
CMD ["python3"]
# Wed, 05 Oct 2022 18:06:22 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Wed, 05 Oct 2022 18:06:24 GMT
ENV SATOSA_VERSION=8.1.1
# Wed, 05 Oct 2022 20:47:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Wed, 05 Oct 2022 20:47:08 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Wed, 05 Oct 2022 20:47:09 GMT
WORKDIR /etc/satosa
# Wed, 05 Oct 2022 20:47:09 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Wed, 05 Oct 2022 20:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 20:47:10 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 20:47:10 GMT
USER satosa:satosa
# Wed, 05 Oct 2022 20:47:10 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d33f116fa83a9fe13ff78c6d4d38481a145985cb05da3b2eb81d3360803b9e`  
		Last Modified: Wed, 05 Oct 2022 07:33:48 GMT  
		Size: 1.1 MB (1094693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cc8907b973c6335ba66c47f29f31c03f214d150a0a7c8f7ea10f56f08df5cb`  
		Last Modified: Wed, 05 Oct 2022 07:34:43 GMT  
		Size: 12.5 MB (12467137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f0ee33a9cc2b5580ebdfeb9d3e5cc6b281af333fdbd839f5b5457e3ded26d5`  
		Last Modified: Wed, 05 Oct 2022 07:34:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ef474fd45a54b20a9e3bb6734240d1be6ad601286de7a1207e17896114f21c`  
		Last Modified: Wed, 05 Oct 2022 07:34:40 GMT  
		Size: 3.3 MB (3336393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777fd0421f723d142b74666e4b7150b6d75fc85c2bec05703363b45f0c826e52`  
		Last Modified: Wed, 05 Oct 2022 20:48:16 GMT  
		Size: 22.2 MB (22157531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2636525afa3305b149289cc53cdc37062a0e49178ed3dc685e7b46515fd65082`  
		Last Modified: Wed, 05 Oct 2022 20:48:32 GMT  
		Size: 183.7 MB (183705715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3cf4d4dbd82f2ce324e9c89facbd5942eacce47a62dc99d9c1f5fb5bb9b37f`  
		Last Modified: Wed, 05 Oct 2022 20:48:11 GMT  
		Size: 9.4 KB (9440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7a2a71a2873423ea4392d40fae28a28b9e6d9d73ba54a6cb29146b876586f3`  
		Last Modified: Wed, 05 Oct 2022 20:48:11 GMT  
		Size: 2.1 KB (2113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:bullseye` - linux; s390x

```console
$ docker pull satosa@sha256:b14365e13c43c487d595d125e1d947e43beed488be99114ca02a3d7a1c4f4939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.7 MB (250673923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067055d0735521050cc614760913cff0dacfa97c019ffedb1c0922151311fcc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 06:05:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 06:05:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 06:05:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 06:05:43 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 05 Oct 2022 06:27:10 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 05 Oct 2022 06:35:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python3 --version
# Wed, 05 Oct 2022 06:35:37 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 05 Oct 2022 06:35:38 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 05 Oct 2022 06:35:38 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 05 Oct 2022 06:35:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 05 Oct 2022 06:35:38 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 05 Oct 2022 06:35:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 05 Oct 2022 06:35:47 GMT
CMD ["python3"]
# Wed, 05 Oct 2022 15:57:00 GMT
RUN set -eux; 	groupadd -g 1000 satosa; 	useradd -g 1000 -u 1000 satosa; 	apt-get update; 	apt-get install -y --no-install-recommends 		jq 		libxml2-utils 		xmlsec1 	; 	rm -rf /var/lib/apt/lists/*; 	pip install --no-cache-dir 		yq 	;
# Wed, 05 Oct 2022 15:57:01 GMT
ENV SATOSA_VERSION=8.1.1
# Wed, 05 Oct 2022 18:39:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		cargo 		dpkg-dev 		gcc 		gnupg dirmngr 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		python3-dev 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Wed, 05 Oct 2022 18:39:59 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Wed, 05 Oct 2022 18:39:59 GMT
WORKDIR /etc/satosa
# Wed, 05 Oct 2022 18:39:59 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Wed, 05 Oct 2022 18:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:40:00 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:40:00 GMT
USER satosa:satosa
# Wed, 05 Oct 2022 18:40:00 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a9e2861e3cb29f36d2532da3b7e12fced4bc6185bf88795f47bd2b43f3706`  
		Last Modified: Wed, 05 Oct 2022 07:04:02 GMT  
		Size: 1.1 MB (1075836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6887f28282f09984d977a6f2e0c71b94f4470a7f9ff4b96fbcd54aad7f31f77`  
		Last Modified: Wed, 05 Oct 2022 07:04:36 GMT  
		Size: 11.9 MB (11904504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f77ea15a6a68073cbdb5abdd9946f642d5ee8ba221231aca54fcf7ed01b68ca`  
		Last Modified: Wed, 05 Oct 2022 07:04:35 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fcc6a3e689d4829f63548781a3888e2d036de80f4e131de51e79ddae40527`  
		Last Modified: Wed, 05 Oct 2022 07:04:35 GMT  
		Size: 3.3 MB (3335736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84923a50c5bc4a4f3af964e5cbc9c5f564ec6d2049914c63d52f7f05269170f8`  
		Last Modified: Wed, 05 Oct 2022 18:40:40 GMT  
		Size: 19.6 MB (19580640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8399de9904ea0fe9969106194cad373216176bac4d71a6a9b3ad4f4a05a64b66`  
		Last Modified: Wed, 05 Oct 2022 18:40:47 GMT  
		Size: 185.1 MB (185114699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d98c580b0489aced3401033fcdc672c7e9e048d3c3faa92d559049ab7d98`  
		Last Modified: Wed, 05 Oct 2022 18:40:37 GMT  
		Size: 9.4 KB (9441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007f31d4d5c2496a3f904d57d0ebc35471ea70d4ffb2199b7145100c0c46d916`  
		Last Modified: Wed, 05 Oct 2022 18:40:39 GMT  
		Size: 2.1 KB (2115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
