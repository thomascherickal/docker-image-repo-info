## `python:bullseye`

```console
$ docker pull python@sha256:b09761ed21b1424218f3e996673cdbfbeed2af5804f7416afbfee0b37e898c2c
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

### `python:bullseye` - linux; amd64

```console
$ docker pull python@sha256:3d11a72c123ffc9326b86ad432480cef0ab73f02b7ed684873c2f8c35ce9a79f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.8 MB (349773811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246fb19839fd033a0dd925c1f89cd1ad482c6b703d56f34bf0d2808b076e132`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:43:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:30:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 08:30:57 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 08:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:31:03 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 13 Oct 2021 08:38:24 GMT
ENV PYTHON_VERSION=3.10.0
# Tue, 26 Oct 2021 22:23:27 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 26 Oct 2021 22:23:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 26 Oct 2021 22:23:28 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 26 Oct 2021 22:23:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 26 Oct 2021 22:23:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 26 Oct 2021 22:23:29 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 26 Oct 2021 22:23:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 22:23:35 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d2d81226a43a97871acd5afb7e8aabfad4d6b62ae1709c870df3ee230bc3f5`  
		Last Modified: Tue, 12 Oct 2021 15:53:13 GMT  
		Size: 54.6 MB (54567761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c24ae8b66041c09dabc913b6f16fb914d5640b53b10747a343ddc5bb5bd6769`  
		Last Modified: Tue, 12 Oct 2021 15:54:01 GMT  
		Size: 196.5 MB (196500090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4322d1621dec2def676639847e546c07a1da4ba0c035edb1036bf5fb45063b`  
		Last Modified: Wed, 13 Oct 2021 09:52:38 GMT  
		Size: 6.3 MB (6290839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777982287b6a9a7b6c2e8f090de34a1564abf3916be787cacd186d2b8605062`  
		Last Modified: Tue, 26 Oct 2021 23:56:11 GMT  
		Size: 19.1 MB (19122971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5fb32d4befd10c682ce3f658540f40db4ec2a0b03afa659bd64b98472b31c9`  
		Last Modified: Tue, 26 Oct 2021 23:56:07 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3be23cccd3f678e797eb2cab75749f8adffa7d3029f1de724f7d6c0755ce03`  
		Last Modified: Tue, 26 Oct 2021 23:56:09 GMT  
		Size: 2.3 MB (2349190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; arm variant v5

```console
$ docker pull python@sha256:aafa55ef3af4c6b2ba1b1267178318c7afd3602746864dd8b71b21e4a3da3c93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.7 MB (321709006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfcf4164e0d56e829ee6982e93ac5389f44850dfc510c2dfe60d45ca6e3eba5b`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:44:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 23:15:29 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 23:15:29 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 23:15:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 23:15:46 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 23:29:27 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 00:43:31 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 27 Oct 2021 00:43:33 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 00:43:33 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 00:43:34 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 00:43:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 00:43:34 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 00:43:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 00:43:48 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c918a5faa65bffd689b9869a942e77a3fbc7d89566be880da188d6050f4f627`  
		Last Modified: Tue, 12 Oct 2021 06:02:11 GMT  
		Size: 52.3 MB (52322898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127725d64ae6922801ff988a903c7db9c780283ffb0ed82afa5763076b47be7`  
		Last Modified: Tue, 12 Oct 2021 06:04:12 GMT  
		Size: 174.7 MB (174690436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a481b4a6314d423a2d363241fc5394aa4b348f2d362497f5b4089a877b048`  
		Last Modified: Wed, 13 Oct 2021 02:18:28 GMT  
		Size: 6.0 MB (6017779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ed9d669b719b2f6567333cc343e31f85ae96ba12a2f91dbbef810d16b6b36`  
		Last Modified: Wed, 27 Oct 2021 02:27:05 GMT  
		Size: 18.2 MB (18241410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288ac15a50d4dd0e225276e40cf43d3627592ace51b8a0b9dc2cb108fed051ff`  
		Last Modified: Wed, 27 Oct 2021 02:26:53 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1d572f50bf6231c7caadabd95d57a95a6bf665248f7dc0d1a72d2b6245e76e`  
		Last Modified: Wed, 27 Oct 2021 02:26:55 GMT  
		Size: 2.3 MB (2349241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; arm variant v7

```console
$ docker pull python@sha256:6ef63cdd93c6430f00f6119a11fd14d1a9a6e559f485e2d9672b5c530bf70708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.5 MB (308543588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd28a76e15751a83c564e5049b489223da7d54680c55fd951596d4be67f38e95`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:27:59 GMT
ADD file:d9f40ca54fb79741d1e76c7bca9250f78453d0b39fb6c921337f3071a79a55a9 in / 
# Tue, 12 Oct 2021 01:28:00 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:35:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 18:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:38:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 05:07:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:07:32 GMT
ENV LANG=C.UTF-8
# Thu, 14 Oct 2021 05:07:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 05:07:45 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 14 Oct 2021 05:28:50 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 00:58:01 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 27 Oct 2021 00:58:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 00:58:04 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 00:58:04 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 00:58:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 00:58:05 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 00:58:19 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 00:58:19 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:88ce59c3081c4041f41eb407032db40c207cc2d806ba0eb12e170b697db91e52`  
		Last Modified: Tue, 12 Oct 2021 01:43:42 GMT  
		Size: 50.1 MB (50118673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d212c40843ca0a1c4c7b2cd635c4801f93ea3c3470b17d99c403c0e065a8711`  
		Last Modified: Tue, 12 Oct 2021 18:57:54 GMT  
		Size: 4.9 MB (4922722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdffc4d771520b3975a2a5a85d9d8594ae6d055776a553760db80a5f8e7a279`  
		Last Modified: Tue, 12 Oct 2021 18:57:56 GMT  
		Size: 10.2 MB (10216977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ea64c0b77d8c40a4101ce92be9b38e5c45e0efe6b4e9c6712d624ba7438be`  
		Last Modified: Tue, 12 Oct 2021 18:58:42 GMT  
		Size: 50.3 MB (50327625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab447199c1569435d8bbc51243e55ea8347a655f0327b9d94e5b02fbe009a347`  
		Last Modified: Tue, 12 Oct 2021 19:00:29 GMT  
		Size: 166.9 MB (166944845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666cc9cc53a0a0a5ece346dbb947ae9201ebd524ee70cb71738d93c15442bd5`  
		Last Modified: Thu, 14 Oct 2021 08:55:27 GMT  
		Size: 5.7 MB (5702121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca4d87b8fd64adf6a96a6f132fca746b740a8ef3a6b9e0a228b3ef8fd051edb`  
		Last Modified: Wed, 27 Oct 2021 03:58:29 GMT  
		Size: 18.0 MB (17961045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf36fc76abfde3cf0d215946a2431d7595385cb22fe1bff1e2e6c8e387ebec69`  
		Last Modified: Wed, 27 Oct 2021 03:58:18 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd2cf5e03f3ddc6723ceeac0f57d82adfa203f863810001319dddb1120c34e1`  
		Last Modified: Wed, 27 Oct 2021 03:58:20 GMT  
		Size: 2.3 MB (2349348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; arm64 variant v8

```console
$ docker pull python@sha256:ea4ed6a876b7a93aa57aeb49eb8ec4bd34c8c1acb8c6149ebb83b4b379c42255
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.7 MB (340677395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b68fdbe2ef2ac6275c7c90cf038b8b677a9041d313d0c46c76e36888a15926b`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:04 GMT
ADD file:1529ae12e334fd992892d3fb97c103297cff7e0115b0475bec4c093939a2bff7 in / 
# Tue, 12 Oct 2021 01:41:04 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:58:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 02:58:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 09:55:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 09:55:37 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 09:55:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 09:55:45 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 16 Oct 2021 10:00:44 GMT
ENV PYTHON_VERSION=3.10.0
# Tue, 26 Oct 2021 23:05:21 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 26 Oct 2021 23:05:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 26 Oct 2021 23:05:23 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 26 Oct 2021 23:05:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 26 Oct 2021 23:05:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 26 Oct 2021 23:05:26 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 26 Oct 2021 23:05:32 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 23:05:33 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:1c47a423366578e5ce665d03788914bf0459485a627a27896fa9c5663ce55cdf`  
		Last Modified: Tue, 12 Oct 2021 01:47:41 GMT  
		Size: 53.6 MB (53603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b1f128be8ebd64f787c46418ffe34ce1096d1ccd6938924d7397713720758`  
		Last Modified: Sat, 16 Oct 2021 03:14:21 GMT  
		Size: 5.1 MB (5141861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c338d42ad921985fb8ebb6e2c48d381f6e03a91535eeffce7f08084b3dfbfdf4`  
		Last Modified: Sat, 16 Oct 2021 03:14:21 GMT  
		Size: 10.7 MB (10655847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27d3d9a061af78e3fcbefe5dbbe718db380687319e5ba8a7c9fd7ba55d16cc3`  
		Last Modified: Sat, 16 Oct 2021 03:14:43 GMT  
		Size: 54.7 MB (54669931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56467c8996a237c29310630374ed68e9883e8e7117197de0272f3275c9c6ce75`  
		Last Modified: Sat, 16 Oct 2021 03:15:20 GMT  
		Size: 189.4 MB (189385660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e0d7dd5fc0502520b41e6920dfbbc1cfb67281ff16e738d5a63051064298a`  
		Last Modified: Sat, 16 Oct 2021 10:59:46 GMT  
		Size: 6.2 MB (6162258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0128a085b8f46003e1c4a4d59fa5f19578a382598c218db6f57adda48a2c50e`  
		Last Modified: Wed, 27 Oct 2021 00:35:14 GMT  
		Size: 18.7 MB (18707705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285d7e5f2c7c8658a556c9baf4c1974d9179c72bb0e08afae04a9858692601c0`  
		Last Modified: Wed, 27 Oct 2021 00:35:11 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d58877f376caf993dc984c82ceda8f80a9015caf6455c7c76f8c1e4b8881b2a`  
		Last Modified: Wed, 27 Oct 2021 00:35:11 GMT  
		Size: 2.4 MB (2350885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; 386

```console
$ docker pull python@sha256:fba7d2d8371fbd2289f7580d1105bda5551a3787c487238a006a6869914fd145
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.2 MB (355202083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0379c46d88f4645d162c55c2b347d500d8e176f5149665ad13f7d81068f77912`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:37:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:10:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 10:10:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 10:10:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:10:19 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 10:42:54 GMT
ENV PYTHON_VERSION=3.10.0
# Tue, 26 Oct 2021 23:58:22 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 26 Oct 2021 23:58:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 26 Oct 2021 23:58:24 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 26 Oct 2021 23:58:24 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 26 Oct 2021 23:58:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 26 Oct 2021 23:58:24 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 26 Oct 2021 23:58:31 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 26 Oct 2021 23:58:31 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ceaeace1516b23dd6c26014f977ec910629b0f1e818efcba72285c444c745dc`  
		Last Modified: Tue, 12 Oct 2021 04:49:16 GMT  
		Size: 199.4 MB (199412262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8f4848838ec6e4b74c8f0c0abaa43b7f9d38872d82c8d5a419d5180aaed64`  
		Last Modified: Tue, 12 Oct 2021 15:16:16 GMT  
		Size: 6.7 MB (6679957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84df066eba12961ec52a112cd1d0c4edf03d4773d2ec3d73f03444a19851ad86`  
		Last Modified: Wed, 27 Oct 2021 01:41:05 GMT  
		Size: 18.4 MB (18385797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd3fa872c6b399eab2ae4ab595b9612e2ea7d67be29f766d6eda5c96532597c`  
		Last Modified: Wed, 27 Oct 2021 01:41:01 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2235e0b4ab3314433865bcb4e3fb6409822910c94ec83311ef442bc0c6857d64`  
		Last Modified: Wed, 27 Oct 2021 01:41:02 GMT  
		Size: 2.3 MB (2349164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; mips64le

```console
$ docker pull python@sha256:b80d9b8f3d4c69054b9ba38c6193db14f701b023398ee2d22bc4c0a1d87623ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329497995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713a3f73b246e3627b74cf7adf7e697fd37797135180d71a54b40b54c096e4a5`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:10:49 GMT
ADD file:856952232716a2e2d5069387a06a537937a1dec1bb75bc9519c60d6ad226bddb in / 
# Tue, 12 Oct 2021 01:10:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:49:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 01:50:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:53:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:17:34 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:17:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 02:18:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:18:14 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 03:49:24 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 01:17:17 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 27 Oct 2021 01:17:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 01:17:19 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 01:17:20 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 01:17:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 01:17:20 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 01:17:40 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 01:17:41 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:3d2cd78b9c44ce4eadbb0cc35b884bfd0dac51123f3c8c6645cb8dc9dc9c1512`  
		Last Modified: Tue, 12 Oct 2021 01:19:18 GMT  
		Size: 53.2 MB (53169836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc92c0f1b1ba16db081439cf0fe0ba300c5acb087b88f97abb47cd8aa1760d6`  
		Last Modified: Tue, 12 Oct 2021 02:04:54 GMT  
		Size: 5.1 MB (5114923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f090a91c9dcffdc8ccb3d0c43f49469a175e0c902bdae900df04c7afe0799f64`  
		Last Modified: Tue, 12 Oct 2021 02:04:56 GMT  
		Size: 10.9 MB (10873345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dca8dc314040adde734540d22d6ece8f751dd2fa78662083691ed36be6a2a8f`  
		Last Modified: Tue, 12 Oct 2021 02:05:49 GMT  
		Size: 53.3 MB (53296535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3cbd8a1740e3dd9cfc5bb50b5091d9750be6809c9404144caf76f9a1853815`  
		Last Modified: Tue, 12 Oct 2021 02:08:01 GMT  
		Size: 179.0 MB (178993465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f6369376b11da243b3fc6c413a52b5e21829ae059a0310972f6dc03370e506`  
		Last Modified: Tue, 12 Oct 2021 17:40:13 GMT  
		Size: 6.6 MB (6620612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6323328652edf00dee3eb6cf12b54857c8831241993f0486e1e1b96bba5cda`  
		Last Modified: Wed, 27 Oct 2021 04:53:27 GMT  
		Size: 19.1 MB (19079899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46354dad65af9e9df08cc8ac4150930c4bd0bed6bd88fb8578e775147abc9215`  
		Last Modified: Wed, 27 Oct 2021 04:53:12 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832fbfd3f73f09bac791c8cb1134ae4684fcbd18e00ff9ef8eaa86a88e8e9a6`  
		Last Modified: Wed, 27 Oct 2021 04:53:14 GMT  
		Size: 2.3 MB (2349147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; ppc64le

```console
$ docker pull python@sha256:45f65501c26fd73bcd930ff27e35eced1c06eec8ef5de09e0f775ae8bfa22183
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359084022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a258f06761b31cb2ae0a5995443aaab41589290cd5aabd75264a722b16261ae`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:04 GMT
ADD file:127b21494e1c790bdbb4c277638b3e16b25fbbcd1e0cdb52e60a4f55a57cd0f2 in / 
# Tue, 12 Oct 2021 01:25:10 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:46:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 03:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 19:34:46 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 19:34:49 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 19:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 19:35:38 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 12 Oct 2021 20:10:36 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 27 Oct 2021 01:49:40 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 27 Oct 2021 01:49:48 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 27 Oct 2021 01:49:50 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 27 Oct 2021 01:49:51 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 27 Oct 2021 01:49:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 27 Oct 2021 01:49:54 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 27 Oct 2021 01:50:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 27 Oct 2021 01:50:12 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c7e7ddcf3b3abfed2b7aab50c1b68bfdfc6fcffed2f4b93ebff4d6050b3d5e72`  
		Last Modified: Tue, 12 Oct 2021 01:36:12 GMT  
		Size: 58.8 MB (58808876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ad477ff0e1489411f419167095ae70f3711a8505b497821289b706b6117c86`  
		Last Modified: Tue, 12 Oct 2021 04:41:09 GMT  
		Size: 5.4 MB (5401977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110cf21b1de9b38b05498de988be3daa0d8ef99e8cb1ff84b5a3d01c61e9d831`  
		Last Modified: Tue, 12 Oct 2021 04:41:11 GMT  
		Size: 11.6 MB (11625975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384a9fb45c6c30c61d87780024c7b377d81b00dec3596a5222eb6e5687e131e`  
		Last Modified: Tue, 12 Oct 2021 04:41:52 GMT  
		Size: 58.9 MB (58851024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5604f798ed9b57b6774ef0752f22b0003715ee542cde915090a58ce1b733e9`  
		Last Modified: Tue, 12 Oct 2021 04:42:40 GMT  
		Size: 195.9 MB (195850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019ea474958b07ec279112b5e08bd1cfec52234b8fb86d489b66306aca1e767`  
		Last Modified: Wed, 13 Oct 2021 01:38:10 GMT  
		Size: 7.0 MB (7041856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3111a3c5dca5cce9d9dde59299071ef47104c7c9a441663344ef3f77d78958d`  
		Last Modified: Wed, 27 Oct 2021 03:59:31 GMT  
		Size: 19.2 MB (19154152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a708b39e5afffa026ea5af9659b0b54b09a5d04cca8166067a3de6a50b7c3ea2`  
		Last Modified: Wed, 27 Oct 2021 03:59:27 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee20aa3274f67c1620a3bd0dec2c15563e40f2b72899438cd65d0e7c361cd27b`  
		Last Modified: Wed, 27 Oct 2021 03:59:27 GMT  
		Size: 2.3 MB (2349227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:bullseye` - linux; s390x

```console
$ docker pull python@sha256:ac5a17f40a2cd32a22e989b8119b3daeca4e13bb12b921e9585511339cbd5f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.1 MB (323095887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b53db846d6d8ad7aabc374b2f3df3166da850966844e7ab4f9a9a09063b9947`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 06:41:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 06:41:08 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 06:41:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 06:41:13 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 17 Nov 2021 07:03:10 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 17 Nov 2021 07:11:00 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Wed, 17 Nov 2021 07:11:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 17 Nov 2021 07:11:01 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 17 Nov 2021 07:11:02 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 17 Nov 2021 07:11:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 17 Nov 2021 07:11:02 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 17 Nov 2021 07:11:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 17 Nov 2021 07:11:07 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bbc68017b41a8cc07b10d715e2a23108c5addefa80b01cac1a2ef075bb1acd`  
		Last Modified: Wed, 17 Nov 2021 03:17:36 GMT  
		Size: 54.0 MB (54041155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5890dc05b0932fa2fcd5ebf331e2dbb96bf6af4989173b3745e7228388fc8f0a`  
		Last Modified: Wed, 17 Nov 2021 03:18:03 GMT  
		Size: 172.5 MB (172490076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e94970c013972c9bb7215d74e2e631b6c95cb53ab2886a2eb2dc6bb0735c1a`  
		Last Modified: Wed, 17 Nov 2021 09:00:47 GMT  
		Size: 6.2 MB (6240897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f77eb758dd69c4bf0c75a7ce32ccb28879bbdfe307a73a2767a834439552f9`  
		Last Modified: Wed, 17 Nov 2021 09:01:15 GMT  
		Size: 18.9 MB (18868484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68335d0c6b6d91a92a72bced14c4429e3efd6a8dae57f09838e22f5082bfe572`  
		Last Modified: Wed, 17 Nov 2021 09:01:12 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b5a146d511f9a39b063f2a30deedb8d8b0c6cfd8324d84916c95c715caef02`  
		Last Modified: Wed, 17 Nov 2021 09:01:12 GMT  
		Size: 2.3 MB (2349166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
