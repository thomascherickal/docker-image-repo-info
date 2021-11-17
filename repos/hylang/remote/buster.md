## `hylang:buster`

```console
$ docker pull hylang@sha256:e758d89e8a3eca02228ae1002966675148cb46c0bcff311df154af7b168331e1
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

### `hylang:buster` - linux; amd64

```console
$ docker pull hylang@sha256:ef0e1b256804ae05a0d8d5b411ce3480b5b2081ea7c58f694d93a8b334034154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46894067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265803a6f0c553ccdcd17b32131c43302c65d0cafbc0fb52cf10ac56ccef6532`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:27:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:27:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 02:27:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:27:16 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 02:27:16 GMT
ENV PYTHON_VERSION=3.10.0
# Tue, 26 Oct 2021 23:07:39 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Tue, 26 Oct 2021 23:07:40 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 26 Oct 2021 23:07:40 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 26 Oct 2021 23:07:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 26 Oct 2021 23:07:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 26 Oct 2021 23:07:41 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 26 Oct 2021 23:07:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 23:07:53 GMT
CMD ["python3"]
# Wed, 27 Oct 2021 00:39:54 GMT
ENV HY_VERSION=1.0a3
# Wed, 27 Oct 2021 00:39:58 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 27 Oct 2021 00:39:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14063a2781d6ddd50c6afb4a9e22cccf2205cb04a72caff066c71cf3e4d19c76`  
		Last Modified: Tue, 12 Oct 2021 03:59:20 GMT  
		Size: 2.8 MB (2770128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40db430947f5f02010fded48c025a40ac4676ad54930881bc13045d759be1ec2`  
		Last Modified: Tue, 26 Oct 2021 23:57:12 GMT  
		Size: 11.1 MB (11082445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4651afaed6a4448b243533bb08e0769b3e71630f1444c059aee6addac8ed5`  
		Last Modified: Tue, 26 Oct 2021 23:57:10 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca213099b1138b10b8df21bf74c486bb43968f83f5559ac13c345e27fb35b46`  
		Last Modified: Tue, 26 Oct 2021 23:57:11 GMT  
		Size: 2.6 MB (2637127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c868081071a370eb954d125f58c700259319caa83f1f9b1341ff45332c9883e`  
		Last Modified: Wed, 27 Oct 2021 00:45:11 GMT  
		Size: 3.3 MB (3264624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; arm variant v5

```console
$ docker pull hylang@sha256:8057b6df7d376c589755b62db6fbc0b894443ba16e7cd4367c3f6512872e4350
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44001094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b14df7ef5ab16113dcbee2e37ffd73f01f3aedfb25ccbba8b1dd8001d8ed25`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:55:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 02:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:09 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 02:56:10 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 02:09:39 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 27 Oct 2021 02:09:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 02:09:41 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 02:09:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 02:09:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 02:09:43 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 02:10:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 02:10:15 GMT
CMD ["python3"]
# Thu, 28 Oct 2021 01:06:59 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 01:07:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 01:07:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2ee7823be7344428bdf9697ac7c13298b13a28b90bd26806a94dd54150bfb2`  
		Last Modified: Tue, 12 Oct 2021 05:30:01 GMT  
		Size: 2.5 MB (2460705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c018832869efa05eb73a1f7a0c17b8fe92e7bf1c467e9fa662c428800d300d`  
		Last Modified: Wed, 27 Oct 2021 02:28:51 GMT  
		Size: 10.8 MB (10765547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8284d46f33730728d8b248fc2a1d2a658c34adc647d7687b5780f09c17e9c61c`  
		Last Modified: Wed, 27 Oct 2021 02:28:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abe600152051059bb6dea464fc617766e2b22ea0f69e3aa942c43101a1fc13d`  
		Last Modified: Wed, 27 Oct 2021 02:28:46 GMT  
		Size: 2.6 MB (2636807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3269909ef671fb7d20ac5983484a849e058e0ae1cafded22168d8e2bcea4187d`  
		Last Modified: Thu, 28 Oct 2021 01:13:20 GMT  
		Size: 3.3 MB (3265098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; arm variant v7

```console
$ docker pull hylang@sha256:fc2ab20d7c289e95759d3ea4558c75b62bc7c8a0b108c4f9209009e69720587e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ed4c6e0ac89e4f10145f39c0b47f4795c8c4580a69aa5480090154107bf10c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 14:38:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 14:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 14:38:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 14:38:51 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 14:38:52 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 02:36:09 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 27 Oct 2021 02:36:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 02:36:11 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 02:36:12 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 02:36:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 02:36:13 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 02:36:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 02:36:41 GMT
CMD ["python3"]
# Thu, 28 Oct 2021 02:58:08 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 02:58:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 02:58:19 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e86b879c212e1c8855b9dae8245a789a3d7b33e8eaab89770fd329ea85471f`  
		Last Modified: Tue, 12 Oct 2021 17:57:16 GMT  
		Size: 2.4 MB (2359007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411b3de1e57d86c84cfb92495f810b7b742c74f9c1b829c3f67aaa963e315662`  
		Last Modified: Wed, 27 Oct 2021 04:00:12 GMT  
		Size: 10.3 MB (10273413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06ed47e77d8a33170cd0216e5036a2ede2ac63d167dc12b0b21d026c77f0b04`  
		Last Modified: Wed, 27 Oct 2021 04:00:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4c814ca09c6e8472ed26b076f5ed4a6680f3950afec6e8e10c1f694e5051b2`  
		Last Modified: Wed, 27 Oct 2021 04:00:07 GMT  
		Size: 2.6 MB (2636831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e920ba4cbb3c7f11e3d2000630147083f4e011d683bd2b4a336027ce6afbb2a8`  
		Last Modified: Thu, 28 Oct 2021 03:11:13 GMT  
		Size: 3.3 MB (3265034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:cd62c6b281e4c236fbe2b22bee011919210b42ca892d51e0b28907d4ad891631
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45317935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c544734dbc6ec70c1c111ed2f569e34fe8bf1c7ba9141df6f1cdc7109bf613`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:08:47 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 12:08:48 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 12:08:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 12:08:57 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 17 Nov 2021 12:08:58 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 17 Nov 2021 12:19:38 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 12:19:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 12:19:40 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 12:19:41 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 12:19:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 12:19:43 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 12:19:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 12:19:58 GMT
CMD ["python3"]
# Wed, 17 Nov 2021 19:35:13 GMT
ENV HY_VERSION=1.0a3
# Wed, 17 Nov 2021 19:35:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 17 Nov 2021 19:35:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f4dbfdbaf408c653fc8669bf567279ddade82816852723ec56e4a2104973b7`  
		Last Modified: Wed, 17 Nov 2021 13:16:56 GMT  
		Size: 2.6 MB (2636095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb80c86664a6749145db1d3e3319d89c39fe8c94aefb3284263e5322da61d34`  
		Last Modified: Wed, 17 Nov 2021 13:16:57 GMT  
		Size: 11.1 MB (11068060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0753761b971edcbd68685c6b5713a021eded809e196cc069048cefd0ad0b7423`  
		Last Modified: Wed, 17 Nov 2021 13:16:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f29097f98178fb7a3fe298e345b6ca63119cde89e68bd83933542ea0f6af51`  
		Last Modified: Wed, 17 Nov 2021 13:16:55 GMT  
		Size: 2.4 MB (2426997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feee9879224e6ffc193ea9302be8c28229a19df402461987a59d516288858f53`  
		Last Modified: Wed, 17 Nov 2021 19:42:01 GMT  
		Size: 3.3 MB (3263433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; 386

```console
$ docker pull hylang@sha256:b4710734643089116c9a59c92f8193c324d77615783015bdd230b824086c7e42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47692462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18f6a535624eacf121644eafcf0a94d02bc395d219756d5cbe685d715868df9`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:34:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 11:34:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 11:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:35:11 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 11:35:11 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 00:54:31 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 27 Oct 2021 00:54:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 00:54:32 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 00:54:32 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 00:54:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 00:54:33 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 00:54:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 00:54:47 GMT
CMD ["python3"]
# Wed, 27 Oct 2021 02:27:33 GMT
ENV HY_VERSION=1.0a3
# Wed, 27 Oct 2021 02:27:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 27 Oct 2021 02:27:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72cdbfcb8f2cd5644506ac0cd5090947f6d31a35726a79f886a5934303675d7`  
		Last Modified: Tue, 12 Oct 2021 15:18:28 GMT  
		Size: 2.8 MB (2781645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507e751f3d0d26e9f98afe1dde353924256121151ec61ab6f293fd4e84d07722`  
		Last Modified: Wed, 27 Oct 2021 01:42:19 GMT  
		Size: 11.2 MB (11217346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca139493e28d0214c4c20ac3aa3b1ecbc7cad00d235a49abdbb509f3df398f13`  
		Last Modified: Wed, 27 Oct 2021 01:42:17 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1d1d05c7a350530a0aaa4bafb0a5e53b163ffb509c653efee588f2f7f048d5`  
		Last Modified: Wed, 27 Oct 2021 01:42:21 GMT  
		Size: 2.6 MB (2636889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9709bad2e1b62759b65aec13c811688d70a5c631e577442b618603ee9913e66`  
		Last Modified: Wed, 27 Oct 2021 02:34:37 GMT  
		Size: 3.3 MB (3264905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; mips64le

```console
$ docker pull hylang@sha256:71c7dcab5a66514670d26a24e1bba0d3b3fec1dcb5e3aff952bf843230edc59f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45098463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8056299b613550180ebf2e32e4dddce6ce12b2ce79b980786f5ab47434c3ee33`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:12:07 GMT
ADD file:a467fbf2015350da455cad98b5f5f247d88749cf317062ca09c466c27d53f87b in / 
# Tue, 12 Oct 2021 01:12:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:09:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 06:09:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 06:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:10:12 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 06:10:12 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 04:39:33 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 27 Oct 2021 04:39:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 04:39:36 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 04:39:36 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 04:39:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 04:39:37 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 04:40:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 04:40:20 GMT
CMD ["python3"]
# Thu, 28 Oct 2021 00:15:00 GMT
ENV HY_VERSION=1.0a3
# Thu, 28 Oct 2021 00:15:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 28 Oct 2021 00:15:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4d8cdee9d607e77b6f8c2203cc9cc02b38004def2b7fe162538c1538da10c870`  
		Last Modified: Tue, 12 Oct 2021 01:21:36 GMT  
		Size: 25.8 MB (25806535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8c46d02e2dc030abf8220908837c8ce7237c6cfe76ea97d5613d0cb7902a5`  
		Last Modified: Tue, 12 Oct 2021 17:42:27 GMT  
		Size: 2.3 MB (2321370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5268f9476c5c3efb91534742257fb761257226accb78d302d215679c3da0be5`  
		Last Modified: Wed, 27 Oct 2021 04:54:59 GMT  
		Size: 11.1 MB (11068868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f033051f15d5cd398b22c0dd56d05b86b31e42d7e45bf80619b91979dd22c8`  
		Last Modified: Wed, 27 Oct 2021 04:54:51 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6679f894bde519d3a6e083366ab6eb3209524ad9be66ba539e0a7b2bce84bec`  
		Last Modified: Wed, 27 Oct 2021 04:54:54 GMT  
		Size: 2.6 MB (2636575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4391bb42f99cad9a384e60806a28b07ee5d156615160b5de1304dee15c31143d`  
		Last Modified: Thu, 28 Oct 2021 00:18:58 GMT  
		Size: 3.3 MB (3264882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; ppc64le

```console
$ docker pull hylang@sha256:05d6289e448a49fcbca6fa005421eae28b8c6863c5352e1d27dac3fb39500eb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51227183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61281967258dee7e58be14af5afbf765bfd80db479c6594c97360301be55d40`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 20:53:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 20:53:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 20:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:54:31 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 20:54:38 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 02:53:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 27 Oct 2021 02:53:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 02:53:09 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 02:53:10 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 02:53:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 02:53:15 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 02:53:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 02:53:49 GMT
CMD ["python3"]
# Wed, 27 Oct 2021 07:33:24 GMT
ENV HY_VERSION=1.0a3
# Wed, 27 Oct 2021 07:33:51 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 27 Oct 2021 07:33:57 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95ee29a374c3f95ac300b0a2569816c6b15c1ba36cf90137267578c6ced2935`  
		Last Modified: Wed, 13 Oct 2021 01:40:02 GMT  
		Size: 2.9 MB (2887525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408195271bce9c23b989e1db6e3610efbf68f52ca3a6cf8f89fd050896a12d5f`  
		Last Modified: Wed, 27 Oct 2021 04:00:45 GMT  
		Size: 11.9 MB (11888811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d42452174707456c77746282953721fd1e82e5810b61b61f404e76d47103283`  
		Last Modified: Wed, 27 Oct 2021 04:00:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd17984e062983f0145b77dac4ed5158def6c86177ed774c58ffa8c48f3d2760`  
		Last Modified: Wed, 27 Oct 2021 04:00:44 GMT  
		Size: 2.6 MB (2638089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789017ba366d7e6eb0ce5e816f3ff2ce0784e99ea25310af00edf40672c8d909`  
		Last Modified: Wed, 27 Oct 2021 07:48:58 GMT  
		Size: 3.3 MB (3265328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:buster` - linux; s390x

```console
$ docker pull hylang@sha256:fe86e12743fc154cfdaf6b2a9907be99e9b4c01f95e4f4fa9d6c3cad480cbac0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45022821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:445ded141ac350c237c932c7a6dd01064e9253ebcdfa90391ac5b046f6b4363b`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:3ff5fbc9c53cf76aad0fe0e1a525cb0bc0d70e8f2a3d5741dfb8b3b8a9448ffd in / 
# Wed, 17 Nov 2021 02:43:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:28:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 07:28:30 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 07:28:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		netbase 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:28:34 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 17 Nov 2021 07:28:35 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 17 Nov 2021 07:36:47 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Wed, 17 Nov 2021 07:36:48 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 07:36:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 07:36:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 07:36:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 07:36:48 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 07:36:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 07:36:58 GMT
CMD ["python3"]
# Wed, 17 Nov 2021 20:17:03 GMT
ENV HY_VERSION=1.0a3
# Wed, 17 Nov 2021 20:17:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 17 Nov 2021 20:17:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b8b917e61b3be882db10e68210f73caf5cc788bfb07aec0a659e30f4796b476b`  
		Last Modified: Wed, 17 Nov 2021 02:49:01 GMT  
		Size: 25.8 MB (25769063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cf7e45aa9b0f16d7e11c2b6ff20b0d3e1ae55510baf86a136a1e9cf14a23ce`  
		Last Modified: Wed, 17 Nov 2021 09:01:58 GMT  
		Size: 2.5 MB (2459494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070d93fa33294230536a806472b83930f9a67b0453f0b9791307e2c822590f83`  
		Last Modified: Wed, 17 Nov 2021 09:01:59 GMT  
		Size: 10.9 MB (10892956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f61fa2ff0829e333be4ef1ff25c95a12803c61dc27fa7dbfa6e2666b807038`  
		Last Modified: Wed, 17 Nov 2021 09:01:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29e20cb9a35f89a291d780ae213cfe629065c42a8798314b82aec345dade475`  
		Last Modified: Wed, 17 Nov 2021 09:01:58 GMT  
		Size: 2.6 MB (2636437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8212ed7faef240aa3c37c0ab18b3e533b7203f3dee353175f296e84500e2ee`  
		Last Modified: Wed, 17 Nov 2021 20:23:01 GMT  
		Size: 3.3 MB (3264639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
