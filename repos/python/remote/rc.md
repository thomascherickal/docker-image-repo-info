## `python:rc`

```console
$ docker pull python@sha256:35b1d8d839311181ac50d0aba830bd7a6a8e55b9234ce71be06ddd0b7576ce5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `python:rc` - linux; amd64

```console
$ docker pull python@sha256:01df9cee8c18899562e7c0cc3e194048cd362cd7fbaffdbb788254fb90c3f141
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.7 MB (350686117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e1f79c6b67b2c02686a6301cdab62c5ce08a13edf921b38068030b5dd8ed26`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:48:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:47:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:47:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 17:20:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 17:20:22 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 20:34:33 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 20:43:46 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 20:43:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 20:43:47 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 20:43:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 20:43:47 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 20:43:54 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 20:43:54 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a88e76431345b48525c4e4d58d497810019f4bafdb5e2bd56dc34a05e09cc3`  
		Last Modified: Tue, 09 Jun 2020 02:00:47 GMT  
		Size: 192.2 MB (192214313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776f0e36afc19d8b1cf242d59ec0e5950aac4e8a60868a266dbc9515ba06f2`  
		Last Modified: Tue, 09 Jun 2020 19:35:03 GMT  
		Size: 6.1 MB (6145050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907230f2e1f4e2242b0c24e41e5a38285a4b53483409ea6d60108b61bdd74677`  
		Last Modified: Mon, 06 Jul 2020 21:01:16 GMT  
		Size: 30.2 MB (30195003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eabc09271c232ac71583230878fc93e770f59a7aab998355a8ef70fa3aa7758`  
		Last Modified: Mon, 06 Jul 2020 21:01:08 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462f35d0bfa2979e2e8c7bc0898a1f0e1de58fd201402a93770635b3c609098a`  
		Last Modified: Mon, 06 Jul 2020 21:01:09 GMT  
		Size: 2.1 MB (2106642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm variant v5

```console
$ docker pull python@sha256:086922b7be5cfc4423559af5517af3d3f6994ae4dde30c9cb38d6a925e798d5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.6 MB (321618433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79431c1051108ed8ceac24ef18a88fd0688ca88cf120e77ba82ae17daed9f37`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:35 GMT
ADD file:2f1cc936406bc9d491f8bcacebb22061ff4c710311b85c5e852ce0d319421b68 in / 
# Tue, 09 Jun 2020 00:51:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:28:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:32:05 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:18:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 07:18:26 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 07:19:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:19:19 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 18:49:23 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 19:01:48 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 19:01:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 19:01:51 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 19:01:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 19:01:53 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 19:02:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 19:02:09 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:3e588deec0981579bbdb8fdc5c1dde7b354b6df6fe9aaca73c69aa0bc697d812`  
		Last Modified: Tue, 09 Jun 2020 00:59:03 GMT  
		Size: 48.1 MB (48107094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b72a58ca618497267d363d547aa0cac4e121092ef4d192f9cd40d48fbaa46c`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 7.4 MB (7360856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fb48ce42ec95f1caafdac679b5a64b2cd2863a624e7e3cad6d34546279f720`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 9.7 MB (9686959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b56b1fead8edb93db924ab12912143e0a0529ae8bfac7b332b343489ce954`  
		Last Modified: Tue, 09 Jun 2020 01:58:29 GMT  
		Size: 49.6 MB (49572262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d836c9d96b13362c3a8f180048a0ff785c5bc77374abd56ef435eb931af6b5c`  
		Last Modified: Tue, 09 Jun 2020 01:59:24 GMT  
		Size: 171.2 MB (171166479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d87d1dd691fb83514b127a0e82aecf9f3a6439e12cdff8200eb261ee1029f`  
		Last Modified: Tue, 09 Jun 2020 10:07:22 GMT  
		Size: 5.8 MB (5839976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c2d1f100cdbf595f9e201424525bf48ff803f6708baf36981e387de9d2240b`  
		Last Modified: Mon, 06 Jul 2020 19:04:16 GMT  
		Size: 27.8 MB (27777731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e71d037a2f2ab42836efbf2fc69aa718ca6537b299ea8f40f579305a7574194`  
		Last Modified: Mon, 06 Jul 2020 19:04:06 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57bfba8ece64c3168de919369624c9b482412e55c0436f87d0fa66d9f8625d`  
		Last Modified: Mon, 06 Jul 2020 19:04:07 GMT  
		Size: 2.1 MB (2106842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm variant v7

```console
$ docker pull python@sha256:f1b84ab3c6dc5e689ef9d3a2927e9139ad7fbe040d9e52abd24dc27eb3472279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.2 MB (313154956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a89060657984ce555545b62e0e8db5fd5c97cde9e3bcfef24b1ddae0a48e71`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:52:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 15:22:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 15:22:14 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 15:22:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 15:22:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 19:31:09 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 19:45:09 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 19:45:12 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 19:45:12 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 19:45:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 19:45:13 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 19:45:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 19:45:28 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d84f63917d0e3fb79c2b4c16f4595b8db444749589cfd28a57ef31188ab110`  
		Last Modified: Tue, 09 Jun 2020 02:12:32 GMT  
		Size: 168.4 MB (168420423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a9df87fb47437c180a0456208542e1900a98b934d3ed37b7e8093da9caed9f`  
		Last Modified: Tue, 09 Jun 2020 18:22:25 GMT  
		Size: 5.5 MB (5536240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b73f757417ef1cc14d541dfeac0d93e3d2b4102caf25d0a35511b4fcbc9b9e`  
		Last Modified: Mon, 06 Jul 2020 20:00:24 GMT  
		Size: 27.4 MB (27424400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320df2bfc328b50b49a500c1471bc676b5579c8111103f38958ff38c99957e13`  
		Last Modified: Mon, 06 Jul 2020 20:00:15 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4663bbf0b3e6504da50324fd27162c35734342b6d037d0540cb43b865b0d36c`  
		Last Modified: Mon, 06 Jul 2020 20:00:15 GMT  
		Size: 2.1 MB (2106859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; arm64 variant v8

```console
$ docker pull python@sha256:88203327e7c9c25e27542818d74aaaa670eca14ce534f5283631c5c5a003662d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.3 MB (340275288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6b4ece82f20f2c11603285cdf82f7653db9d5bef8d67b69d008b80a822eec8`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 04:11:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 04:11:27 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 14:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:08:37 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 20:56:09 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 21:05:59 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 21:06:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 21:06:04 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 21:06:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 21:06:06 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 21:06:20 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 21:06:21 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326561827fde74d56d06dce7035ef6653dbf62a27a5dc35416ba6f00293a09b8`  
		Last Modified: Tue, 09 Jun 2020 02:48:39 GMT  
		Size: 183.7 MB (183744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824604b39a2bb683a5c5e24f45cb35f2e372484dbd7a0a8584b76fe34a99437b`  
		Last Modified: Tue, 09 Jun 2020 16:48:54 GMT  
		Size: 6.3 MB (6259331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865cc25b00bf2c9a006bd970f40e39097529ecb2877d53a8a1d305f0f9f02750`  
		Last Modified: Mon, 06 Jul 2020 21:25:37 GMT  
		Size: 29.2 MB (29175278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909da1497610790c42c40e0dbe391bea00ca686aa81a0d603755307ecb4b0cd1`  
		Last Modified: Mon, 06 Jul 2020 21:25:27 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b6d6f71f3835d07fa2b8511c58622d1ea7dacc23ac53ba4ede73953c995d6a`  
		Last Modified: Mon, 06 Jul 2020 21:25:28 GMT  
		Size: 2.1 MB (2106845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; 386

```console
$ docker pull python@sha256:d78d2fa3a520ae59d1644e3923f65f061c262eea0aebca0e78bdba8631a5038c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358507718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12952e47fa931e5d0311f73a8183a8559a1176424391aa88fe683fe13d09043f`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 15:48:23 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 15:48:23 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:43:31 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 19:49:57 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 20:07:30 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 20:07:31 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 20:07:31 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 20:07:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 20:07:32 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 20:07:44 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 20:07:44 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e805e55983a46c901632f289542625edb04ff470dc6dd9217466a3788d608`  
		Last Modified: Tue, 09 Jun 2020 02:33:23 GMT  
		Size: 198.8 MB (198755099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c62fd4eb29b10c1fa4fb03b84e361acbb9f4039d3613d6699565c550723abb`  
		Last Modified: Tue, 09 Jun 2020 19:38:10 GMT  
		Size: 6.5 MB (6489009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4779db3fd5929240b35ed752463618044aa37eff42d2ba0f7c66737ae53903c`  
		Last Modified: Mon, 06 Jul 2020 20:31:23 GMT  
		Size: 28.3 MB (28251301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0c0a874cd07c8d6eefd42ff2e5f0a549d49bbabfaf33705f6e6e84d903d7be`  
		Last Modified: Mon, 06 Jul 2020 20:31:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5e062a7b183d9819f9c303ca18c31a26c1d4f57af012c0d6f2dc66b2483271`  
		Last Modified: Mon, 06 Jul 2020 20:31:15 GMT  
		Size: 2.1 MB (2106677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; mips64le

```console
$ docker pull python@sha256:1f55b10a4c562c914e51b705711a1420b1b6eeb4620d9b888139be986cce25dc
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.2 MB (335212359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb31ca8c7ea5a365f2a347f7274cdd50c15ba3679088a472045505e225a73899`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:09:44 GMT
ADD file:b51eae556569a7654c89a15b745fafdb0477ed08e8a06f7fcd6363145123d67f in / 
# Tue, 09 Jun 2020 01:09:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:51:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:55:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 11:00:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 11:00:45 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 11:01:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 11:01:08 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 19:11:09 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 19:59:27 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 19:59:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 19:59:29 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 19:59:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 19:59:30 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 19:59:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 19:59:55 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:8084fc3b4d2453eb8005c0b33e3c542e3615868e22652e74e19fec36df3c488e`  
		Last Modified: Tue, 09 Jun 2020 01:17:30 GMT  
		Size: 49.0 MB (49019818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df088964944d43608e89126d7ae55a47489499bad77148bac16c1593e8ff69a`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 7.2 MB (7231469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a34d1c06dc4557c94a0e8dc1d4f49ee8f512c443dea9748d2bb00fc4e1f6502`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 10.0 MB (10015784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaedff7ebdd283f729f3eb0635079193636dc776885aa0339370ed36edfbc2f`  
		Last Modified: Tue, 09 Jun 2020 02:11:18 GMT  
		Size: 50.8 MB (50838846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814cc59ed9a88b832e8d53df38caa9b76578203bea7cbfc5b7c03b6d842221e1`  
		Last Modified: Tue, 09 Jun 2020 02:13:43 GMT  
		Size: 179.7 MB (179749508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adea584f72a079f0e09d6d585b8bb7b7ec1b4a661db7f237337cdd5c8c2b188`  
		Last Modified: Tue, 09 Jun 2020 18:55:58 GMT  
		Size: 6.5 MB (6454880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f1ccb1951aea95e0034d40482ae8cb76a5311e347ee489fd85a51a559dcfab`  
		Last Modified: Mon, 06 Jul 2020 20:01:40 GMT  
		Size: 29.8 MB (29795092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d25d91577789fd152a3aa710399e68d2326e0006bccaa0a9947ba280902d06`  
		Last Modified: Mon, 06 Jul 2020 20:01:11 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bef6592cd7bd769d0081ee21ed88c18077a11235a8334f55d154baeb67e6683`  
		Last Modified: Mon, 06 Jul 2020 20:01:13 GMT  
		Size: 2.1 MB (2106728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; ppc64le

```console
$ docker pull python@sha256:7f0bde1271edf4ebdd216e537c91dba8be5743f3d79ae1383a4397bbe0d030e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.6 MB (373554522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b88d3af11711258d846551d3d92c2be85689f500306004b0dec90d8905b7cc1`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:01 GMT
ADD file:18a41180457a190a9dede1228479d2e332a348f22ac027c36e14d6d92e556f22 in / 
# Tue, 09 Jun 2020 01:22:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:58:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 03:00:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:11:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 13:57:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 13:58:11 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 18:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 18:02:26 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 19:36:14 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 19:47:48 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 19:48:05 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 19:48:11 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 19:48:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 19:48:18 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 19:48:40 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 19:48:44 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:0cad52b1770a1b4a84068be3efe78098837be582f5905e627b2cdba07e641fd1`  
		Last Modified: Tue, 09 Jun 2020 01:30:12 GMT  
		Size: 54.1 MB (54143376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0318f8e4196d9f742fcca63ed04f9c2cb14ac6541f33cd67dae342ef35845da`  
		Last Modified: Tue, 09 Jun 2020 03:43:38 GMT  
		Size: 8.3 MB (8254819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec302fe954105553bdc7cac9100b6bfd114d3b56ef94d850b0364da83650fc6`  
		Last Modified: Tue, 09 Jun 2020 03:43:37 GMT  
		Size: 10.7 MB (10727191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf65a8c1ffe0371d22a42dfd9c0b4ac2900e0ca4d9d12502c488c59d3aff6aee`  
		Last Modified: Tue, 09 Jun 2020 03:44:31 GMT  
		Size: 57.5 MB (57460152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aad1912038650766f7c3949e5b7084d257bdb77914a13f32fc7334f57b1ee68`  
		Last Modified: Tue, 09 Jun 2020 03:46:28 GMT  
		Size: 203.0 MB (203016516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed779f95fafb2a686209f8d45637bc8ae08766c136225f1c93e0f10815311223`  
		Last Modified: Tue, 09 Jun 2020 22:02:05 GMT  
		Size: 6.9 MB (6892317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb235c1d276a57b5285e2052acd9722dba4a89b83b83169698941960430a45`  
		Last Modified: Mon, 06 Jul 2020 20:13:32 GMT  
		Size: 31.0 MB (30953073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9291e86c2d26b7ed19afb3c4c9933964f84998f3197d3468e193d55dab1c17`  
		Last Modified: Mon, 06 Jul 2020 20:13:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c98977cbfe9fa16d96566e3b74100733bea6ffb81602399d5dad439ec7a23c`  
		Last Modified: Mon, 06 Jul 2020 20:13:24 GMT  
		Size: 2.1 MB (2106844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - linux; s390x

```console
$ docker pull python@sha256:2f1b45e60bf0d8aa09ff7f8871f5406497ae1aaf707bfe77994e7aa5f3e0500a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332552732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e70b0e6870de13a13a64bd5035386068e61c31cc89f455077a05260691c0418`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:21 GMT
ADD file:525b5566f1fb9dfef74a4f49170a50bba0f0ed22a8bd627a8f802803236f1db8 in / 
# Tue, 09 Jun 2020 01:42:23 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:09:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:09:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 08:26:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 08:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 09:28:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 09:28:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Mon, 06 Jul 2020 19:50:19 GMT
ENV PYTHON_VERSION=3.9.0b4
# Mon, 06 Jul 2020 19:55:20 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Mon, 06 Jul 2020 19:55:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 06 Jul 2020 19:55:23 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Mon, 06 Jul 2020 19:55:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Mon, 06 Jul 2020 19:55:23 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Mon, 06 Jul 2020 19:55:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 06 Jul 2020 19:55:30 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:76dae9e9a8f2b69403c29a068363410a0b491d889452a410e1a846db24918418`  
		Last Modified: Tue, 09 Jun 2020 01:46:14 GMT  
		Size: 49.0 MB (48965925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea4ddfd9cac861440dd774171c0df5d003bcf031cc856603f0dcc1a569a7614`  
		Last Modified: Tue, 09 Jun 2020 02:18:01 GMT  
		Size: 7.4 MB (7385198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4340e9fce6caba0ffebdee007c25f4ed849de61e56dcee1ed7e081edbcf1e5`  
		Last Modified: Tue, 09 Jun 2020 02:18:06 GMT  
		Size: 9.9 MB (9882055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89446217dee5ed85681993c919acbdf28494151380677fdefa88b6b5e481573c`  
		Last Modified: Tue, 09 Jun 2020 02:18:19 GMT  
		Size: 51.4 MB (51366573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61438bbb152f907aeaae3b74ab198003590836b10d32255683615a865a061c46`  
		Last Modified: Tue, 09 Jun 2020 02:18:46 GMT  
		Size: 176.8 MB (176764149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18bd1ddd205f062d03d6e54ca50e73aa4a03002602c0b8f13908d2c1afdea61`  
		Last Modified: Tue, 09 Jun 2020 11:03:38 GMT  
		Size: 6.1 MB (6057856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e23c3398a9c8148c2d56c869e2ea83577fa0f8a01d2ee8e747dcc2dc2ec2a1`  
		Last Modified: Mon, 06 Jul 2020 20:07:38 GMT  
		Size: 30.0 MB (30023877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae264e2088dee300e474267ec88fde26205b5916e4ed84bfbc7777754a9634`  
		Last Modified: Mon, 06 Jul 2020 20:07:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ff39fb86789f60d83c8358c33b1768e3d098cfa165e8a007990dbf82f1af76`  
		Last Modified: Mon, 06 Jul 2020 20:07:33 GMT  
		Size: 2.1 MB (2106865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - windows version 10.0.14393.3808; amd64

```console
$ docker pull python@sha256:5d6bb650f3daaaee022c3317f23b4f4ad1487a174574a50ff3555fa85abdc12f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5811323096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41eccf5eb74e647ae5fa864603b30eb806acf935b6ae4fdffd1a7155962fd0b`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 15:11:08 GMT
ENV PYTHON_VERSION=3.9.0b4
# Wed, 15 Jul 2020 15:11:08 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 15 Jul 2020 15:13:48 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:13:49 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 15 Jul 2020 15:13:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 15 Jul 2020 15:13:52 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 15 Jul 2020 15:15:50 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:15:51 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c092947b8e0a4b70ab2057dc4d839f279a3e97a44dbbd5cf1c6d78625d19706`  
		Last Modified: Wed, 15 Jul 2020 16:06:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e656db332a6c560d8c59bbca5791b50d32fd04f0d848f609cbfbc396103f0`  
		Last Modified: Wed, 15 Jul 2020 16:06:01 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd674549405d948fa68fc5e261c6a7cc39f0f2e978311a069b31768ea21af4c4`  
		Last Modified: Wed, 15 Jul 2020 16:06:11 GMT  
		Size: 58.5 MB (58460081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188c5057c62c16ebd66671dd8fa2f5ea5852b3ac6b228517ce774a4224a74c49`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16cbd68fc02b4db0e46b2447f1f621f9837378398fad7610d1722ac0450e46`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a62f921fdee54169f1144917e019deee414b1099f9356de34c2928dfedc7cac`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044a084f9497c4602cdb79648891a1ebdd0ce42cf242ebf248e198a68a217641`  
		Last Modified: Wed, 15 Jul 2020 16:06:03 GMT  
		Size: 15.4 MB (15392924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267879af5c9452d2fb96868b24e7aaa200c82fe7d9ac0d196f88461b6b85ecc3`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:rc` - windows version 10.0.17763.1339; amd64

```console
$ docker pull python@sha256:9bb8a7ba249ff5581fbc7936d88b35fd1153e63ab7c1c3aaf79f505d62a6ccc4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378278657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02c96b286e88da00a84f47d2d6f0aa60a1dd18b2cd1c360719b3e11b3adffe3`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 15:16:05 GMT
ENV PYTHON_VERSION=3.9.0b4
# Wed, 15 Jul 2020 15:16:05 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 15 Jul 2020 15:17:57 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:17:58 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 15 Jul 2020 15:18:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 15 Jul 2020 15:18:01 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 15 Jul 2020 15:18:57 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:18:58 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e31ac57da0b12a7b4205073fc685298f44fe244dc4fe01bea8995dfeaae5b7e`  
		Last Modified: Wed, 15 Jul 2020 16:06:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c206535bbe7125994f9d9b588516c5fcac3dc361c2c5e03f9fa9aaebc2d64b`  
		Last Modified: Wed, 15 Jul 2020 16:06:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf387c2fc343d6e89e88da38b5b0b2c1501eee1d3a5dba8e50cd07b51fc449df`  
		Last Modified: Wed, 15 Jul 2020 16:06:39 GMT  
		Size: 57.8 MB (57813903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94052a89523b8dab42fae81d4143328e603659fb32096b5f7ffce7d8e2692733`  
		Last Modified: Wed, 15 Jul 2020 16:06:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e69baedce2671e0627500667ac506f2a5c34a5021b4792d4c905e671852990d`  
		Last Modified: Wed, 15 Jul 2020 16:06:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceab9b21b17d53a3f644c0bf69f00f391ef552b71a9a68be3fd0c40fb4bb0a24`  
		Last Modified: Wed, 15 Jul 2020 16:06:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945f406bb2649596f4c01d274b1cf7956b47beafed7a77ca5ff7c6f19d180413`  
		Last Modified: Wed, 15 Jul 2020 16:06:35 GMT  
		Size: 10.3 MB (10264438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4875ad03aecb3ddb2962ba78e19d37cf95245d103d96a86b28d1866a5a33b68`  
		Last Modified: Wed, 15 Jul 2020 16:06:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
