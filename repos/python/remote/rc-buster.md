## `python:rc-buster`

```console
$ docker pull python@sha256:94fe7cf402628b73dea2d086c3845223fafea32abdcdaa01127ace38ebc49cfd
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

### `python:rc-buster` - linux; amd64

```console
$ docker pull python@sha256:2a1c9fccfa45013c7e71d8948066950458f2f5587b993e951596e1224b4f2504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.3 MB (341258630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0377856e82525f2bf517f5129ad024f39433670bd4a07cd6199359eab75799`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:34:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 19:53:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 19:53:16 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 19:53:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 19:53:23 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 19:53:23 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 20:01:59 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 20:02:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 20:02:00 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 20:02:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 20:02:01 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 20:02:07 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 20:02:07 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e5f66f5d0e1c97622f33d44fb04efb42bd3562bdc3482537d121040c789f9a`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 7.8 MB (7833606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c8f1c77d6674046d7deb41be1ca07f25cb43fd67f87e879ee79cc6586087f0`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 10.0 MB (9997249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5095cab277710f0c2883844158323ad986c763ffc37353ddff874dd85585d9b6`  
		Last Modified: Fri, 03 Sep 2021 06:40:55 GMT  
		Size: 51.8 MB (51840968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7fe362a971515971cf53613a30cc824f94d544272a5e061eb6365923ccbc11`  
		Last Modified: Fri, 03 Sep 2021 06:41:32 GMT  
		Size: 192.4 MB (192394977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d8710b0a9c611ad4a36359868daba091097621da798df7144ccf4bacdf81c`  
		Last Modified: Fri, 03 Sep 2021 21:13:10 GMT  
		Size: 6.1 MB (6146094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e333b4fe4558aa0870cd975ef87a27aea584540e71a73de91945e6b4afca0b1`  
		Last Modified: Fri, 03 Sep 2021 21:13:12 GMT  
		Size: 20.3 MB (20260663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd5864773249d66b93f15a14b668a40918032260420d4c6c84dfb78efc96114`  
		Last Modified: Fri, 03 Sep 2021 21:13:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6723857b6c582212ba428cd162b25b62e485acdec8853a5591dca85a75cae79`  
		Last Modified: Fri, 03 Sep 2021 21:13:09 GMT  
		Size: 2.3 MB (2348948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v5

```console
$ docker pull python@sha256:2aef9ee1a46866492489a6fdefe1a641969b39f2df829f7c636ebfcd94fdd10c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313571563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b69ff00c485e48b847aa8d4beb58fee3945270c04b80c27f3b221597ae5d1b`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:39:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:57:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:57:20 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:57:37 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 12:57:37 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 13:11:56 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 13:11:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 13:11:58 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 13:11:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 13:11:59 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 13:12:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 13:12:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df658833310cf636515e182b07f0f757747de5e7bf7cb2d5798c438dffe9a962`  
		Last Modified: Fri, 03 Sep 2021 02:55:13 GMT  
		Size: 49.6 MB (49574916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c5eacbd1943e12eba81a033914a38c27e596c6baab6126ef425dcec1b36a99`  
		Last Modified: Fri, 03 Sep 2021 02:57:09 GMT  
		Size: 171.3 MB (171331569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3498a5688ab8ffb7812387173c2764838c50d74fbb8e6151cc23de59a5ae54`  
		Last Modified: Fri, 03 Sep 2021 16:42:00 GMT  
		Size: 5.8 MB (5840761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34597cfac6761fe9f508482a60b25e5b599a88db337707f3185971939c640214`  
		Last Modified: Fri, 03 Sep 2021 16:42:10 GMT  
		Size: 19.3 MB (19256828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42410edbd58094dd029e81d477a410e6a06b480251fcdfeff0b73759dda7c5`  
		Last Modified: Fri, 03 Sep 2021 16:41:56 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de5eaab6aac87d03af781ed30599c8fa7cd3ef0427c0b69c530891b47ff7304`  
		Last Modified: Fri, 03 Sep 2021 16:41:58 GMT  
		Size: 2.3 MB (2349012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm variant v7

```console
$ docker pull python@sha256:bdb58a446f3001cc67f87b1067d7d88b55ecd75ffcbcd4f01b4b13645a6af574
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305213416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bcf4c8594d83888ad89bc327f2119e758af378ab684867b3bf8fc258090cc82`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:07 GMT
ADD file:7d9f257bd092a8a471b2e30445e24ebcdd04fe5eb33221ef4cb542c51cd67634 in / 
# Fri, 03 Sep 2021 01:00:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:55:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:56:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:56:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:58:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:42:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:42:05 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:42:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:42:19 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 17:42:19 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 18:01:26 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 18:01:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 18:01:29 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 18:01:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 18:01:29 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 18:01:45 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 18:01:45 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:31da451bd6969464c4b47947ee26596591a377c63a0e72516d2f30ee57e2b208`  
		Last Modified: Fri, 03 Sep 2021 01:15:39 GMT  
		Size: 45.9 MB (45917540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87adc3bfcca5fb7687b4659aa5234d7129c257bee13db9fc2023182221c8f9`  
		Last Modified: Fri, 03 Sep 2021 03:16:21 GMT  
		Size: 7.1 MB (7124882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839b23a1c23903dc0f3dd12042eba74f3c52eb0f7f6bcccb387bc1a9fd6a7e94`  
		Last Modified: Fri, 03 Sep 2021 03:16:21 GMT  
		Size: 9.3 MB (9343846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bdddceb233fa2c9e12d0ca171371ccf6ae0dbcbac996eceeb26801c852951b`  
		Last Modified: Fri, 03 Sep 2021 03:17:06 GMT  
		Size: 47.4 MB (47357010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ebd1bb2ec4f281d5f384fc44745d27c7d77e05a61c18e48e002a258b5e7ebb`  
		Last Modified: Fri, 03 Sep 2021 03:18:52 GMT  
		Size: 168.6 MB (168592215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1712088d03454a1aca9e6da348245b284f6a8e79282cac7682bae2520cdcc103`  
		Last Modified: Fri, 03 Sep 2021 23:56:47 GMT  
		Size: 5.5 MB (5536658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56822f84636fa4183ef5c43582b1e61d6f8f0fc2fd04a0d5828c57e438f253b`  
		Last Modified: Fri, 03 Sep 2021 23:56:56 GMT  
		Size: 19.0 MB (18992013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bab83b2d32d6f73feb7aa1e4dd3ca59dee6a56dd482812909b15361d0e0dce`  
		Last Modified: Fri, 03 Sep 2021 23:56:43 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dcc2d556bb4197435ab9fffeb74b8f5c905481b13b0c1cbffa17fb5fc20c95`  
		Last Modified: Fri, 03 Sep 2021 23:56:45 GMT  
		Size: 2.3 MB (2349021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:86701cbb73143f1ede2ce03dba4a938e43667ef4b3813eabb0a8ca1752912610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.3 MB (331334166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef6f0b52e287642e011a55da8505300f7149d8ea5e3a70f546cb43bc41ae4e6`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:34:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:00:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 05:00:34 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 05:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:00:40 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 05:00:40 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 05:06:58 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 05:06:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 05:06:59 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 05:06:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 05:07:00 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 05:07:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 05:07:06 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a277fe22c4aa02638e00e9df995f81fc80e44710768e66b1067d15d6ebfb117d`  
		Last Modified: Fri, 03 Sep 2021 04:43:16 GMT  
		Size: 184.0 MB (183974353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a05e58b4dbdc9ce1bb6bc758ba09207088932561c2c9e2145529af33d498f4b`  
		Last Modified: Fri, 03 Sep 2021 07:08:14 GMT  
		Size: 6.3 MB (6259474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bda1ff47291267d9f5b65557979ae6ae0d9706f8200def49802df6262820cb`  
		Last Modified: Fri, 03 Sep 2021 07:08:16 GMT  
		Size: 19.7 MB (19681157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d07a1ed3f3d59bc26f3f3d133bdca9de6ffd84aa9d828edb6aff6edd82eeed`  
		Last Modified: Fri, 03 Sep 2021 07:08:12 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00006ef67d3e5d9aec9f91af5f0bf3ff0afb03815b2ddb4ded126a323058b9`  
		Last Modified: Fri, 03 Sep 2021 07:08:13 GMT  
		Size: 2.3 MB (2348911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; 386

```console
$ docker pull python@sha256:05bc1ba233a7671749f60db3d18fa5871edca8de0f29670c54a86d398f8087b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.3 MB (350257434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:458482a3938e48812d08333b016f8038dae5f278e8ca3f8393f41115a7351458`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:19:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:19:07 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:19:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:19:18 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 17:19:18 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 17:33:10 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 17:33:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 17:33:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 17:33:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 17:33:13 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 17:33:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 17:33:25 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076e49e31f46f892cc53ebc742d6b7aac932b484254aa2eebc010ca0de90549`  
		Last Modified: Fri, 03 Sep 2021 01:22:43 GMT  
		Size: 198.9 MB (198931128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7fd42169baed4401d459521099caaaac715d68e28c1b177fdbc33a574d8a7e`  
		Last Modified: Fri, 03 Sep 2021 21:14:11 GMT  
		Size: 6.5 MB (6490415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3964bd02c04d08bbc36e9847e1743ebd416915449fe49299a412d07f14ece88`  
		Last Modified: Fri, 03 Sep 2021 21:14:14 GMT  
		Size: 19.5 MB (19501502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a203273fbcccd4370691d7f86b6fb449329e5f66068e8b45fdf5a7f5d1215a`  
		Last Modified: Fri, 03 Sep 2021 21:14:09 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ae62d3995a6c60f9d80b4ede55dfaf411a791e10c25e0e0c3e4ae89931df06`  
		Last Modified: Fri, 03 Sep 2021 21:14:10 GMT  
		Size: 2.3 MB (2348996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; mips64le

```console
$ docker pull python@sha256:b8b201a654bd4e3902e4c5b91acba53f04084ab2755eb0ebb3cf25ae762bb129
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325716913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce35b595480bd0af2cb3276cb6d59491b163be8ed6f56d3c86f89f64c92d5a52`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:49:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:44:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 05:44:38 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 05:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:44:55 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 18 Aug 2021 05:44:55 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Wed, 18 Aug 2021 06:26:53 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 18 Aug 2021 06:26:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 18 Aug 2021 06:26:56 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 18 Aug 2021 06:26:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 18 Aug 2021 06:26:56 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 18 Aug 2021 06:27:20 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 18 Aug 2021 06:27:21 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a254e959b3e0b79e2ecebd56f2318cd2299b7983a3afc46b2ccf4c7400d3cb`  
		Last Modified: Tue, 17 Aug 2021 21:00:16 GMT  
		Size: 179.9 MB (179911997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1219e2a7b715b79d76b028f03f306e8c68823374e6ed7396c056127cb05d615d`  
		Last Modified: Wed, 18 Aug 2021 11:44:36 GMT  
		Size: 6.5 MB (6455424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138acd2420f0c9cc01d3ff7887432a8e32d0d8451f2f0a5203b8edcdbc4dad0a`  
		Last Modified: Wed, 18 Aug 2021 11:44:45 GMT  
		Size: 19.8 MB (19808440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e7d9cef86b609675f838a70b6dc52902e6f122aa2e73158b69e44728b9f22`  
		Last Modified: Wed, 18 Aug 2021 11:44:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9436ada8282587b4fa2754d67aa141b16666e7684fe7ced966375413baf21`  
		Last Modified: Wed, 18 Aug 2021 11:44:33 GMT  
		Size: 2.3 MB (2348793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; ppc64le

```console
$ docker pull python@sha256:08c5d978dbab233dd2e5c009041b253332070bd64c674bfb35a0ebcec5f10c2f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.9 MB (363937952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c97c86d61a4e22dfe041096a369465243ed3ffb1214f0dfeaf1ff6197469fe`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:42:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 21:59:33 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 21:59:38 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 22:00:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 22:00:44 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 22:00:50 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 22:10:40 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 22:10:54 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 22:11:00 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 22:11:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 22:11:10 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 22:11:36 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 22:11:44 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0210891d190261ad1963160b64e1e7e13a3b1e4b1ac8f297c5280432fa730`  
		Last Modified: Fri, 03 Sep 2021 07:13:03 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a2531ea29e5d6a6e910840570189332f132c3c99c3ca0ce21f40c4311be87`  
		Last Modified: Fri, 03 Sep 2021 07:13:52 GMT  
		Size: 203.3 MB (203284346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136b36b93dd4ab4e74a5da0264447f26030e26214fde7ee48c4d62d6ebf2c468`  
		Last Modified: Fri, 03 Sep 2021 23:54:31 GMT  
		Size: 6.9 MB (6893725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c72b2f17a87e73234611e75afda6d3b7beef1e0d633f29bfa56f894ec81295`  
		Last Modified: Fri, 03 Sep 2021 23:54:37 GMT  
		Size: 20.8 MB (20770196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4709a30938e977b6d270c058ea35833d4b8d3b7b0ee3874edcf8202f3d5e43f2`  
		Last Modified: Fri, 03 Sep 2021 23:54:30 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2611afcb0ef431e934d265bedd5f2337ce01765dcc7c1ed2e06545504056fd71`  
		Last Modified: Fri, 03 Sep 2021 23:54:31 GMT  
		Size: 2.3 MB (2348983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc-buster` - linux; s390x

```console
$ docker pull python@sha256:50f91b5213311309cba98b62d7733445a1881afcd0e7e99fe3d4df3ac58e56b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322840924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb9314e2b959078fc1b84963846dc11e786cd66a4a1e51b5b12cfe1577605f9`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:11:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:34:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:34:39 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:34:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:34:44 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 03 Sep 2021 06:34:44 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Fri, 03 Sep 2021 06:40:38 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 03 Sep 2021 06:40:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 03 Sep 2021 06:40:43 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 03 Sep 2021 06:40:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 03 Sep 2021 06:40:44 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 03 Sep 2021 06:40:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 03 Sep 2021 06:40:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492849c87aa7918355ea3ddd15023d5192779474cd1ad01937363046cd5ed777`  
		Last Modified: Fri, 03 Sep 2021 02:20:59 GMT  
		Size: 51.4 MB (51380450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f583bcb6e3e69399c59333e43ffaa7efcf40301ec6fec56dcecb4f1ee5b35be1`  
		Last Modified: Fri, 03 Sep 2021 02:21:28 GMT  
		Size: 176.9 MB (176880284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6ab9fbf1e4e06be1abc8fe68c61f2c4c7edb787ebf5723ad0bb7477223eb40`  
		Last Modified: Fri, 03 Sep 2021 08:42:39 GMT  
		Size: 6.1 MB (6059120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4731baa82c418b885fdc76d1244e09c2149fff1ea3caeb250dc87efcd90b1af1`  
		Last Modified: Fri, 03 Sep 2021 08:42:42 GMT  
		Size: 19.9 MB (19883513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afe2a22de58187b0576ac80e071b6eb31b960cc10d9ba44890f99d7a86a2559`  
		Last Modified: Fri, 03 Sep 2021 08:42:38 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e930ad16e3c0d930efc54f2e74f1ee84ed2164f3e00f7b0a4ed497605c7780`  
		Last Modified: Fri, 03 Sep 2021 08:42:38 GMT  
		Size: 2.3 MB (2348994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
