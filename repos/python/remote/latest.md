## `python:latest`

```console
$ docker pull python@sha256:d1f4c247976c0c19dd7749d61cc99c59bc5a22c4dff482624d78aa28a8a34e52
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
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `python:latest` - linux; amd64

```console
$ docker pull python@sha256:7988e94d90e711d3da1a279712484878f36513b64a4934cdf3a09f7f5725cec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339765098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0611cf846c85aac44ceca0952a02c6202b3ab6561e51c6d00ac15f981aed2732`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:37:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:37:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 20:37:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:38:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 12:59:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 12:59:04 GMT
ENV LANG=C.UTF-8
# Sat, 12 Dec 2020 12:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 13:07:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 12 Dec 2020 13:07:49 GMT
ENV PYTHON_VERSION=3.9.1
# Sat, 12 Dec 2020 13:16:05 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Sat, 12 Dec 2020 13:16:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 12 Dec 2020 13:16:06 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Sat, 12 Dec 2020 13:16:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Sat, 12 Dec 2020 13:16:06 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Sat, 12 Dec 2020 13:16:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 12 Dec 2020 13:16:13 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87cd3c61e278307eaa282fdbb51a5e2415cda64999c70a381ed6c5c724d370a`  
		Last Modified: Fri, 11 Dec 2020 20:44:17 GMT  
		Size: 7.8 MB (7811925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a3c799ec372b93b6dbd4b270effd9f36444dc164e8827ea9ab7aa0d1ef87da`  
		Last Modified: Fri, 11 Dec 2020 20:44:17 GMT  
		Size: 10.0 MB (9996419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c38f966ac77bd84d7866db24e1f7611b158e51e10e2e73ce009c3ad73f472`  
		Last Modified: Fri, 11 Dec 2020 20:44:36 GMT  
		Size: 51.8 MB (51830085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd6d195b6814bc0fc1eb872f13330e352cd881fc3dda45997e398aadfde685`  
		Last Modified: Fri, 11 Dec 2020 20:45:20 GMT  
		Size: 192.3 MB (192314183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b9446ae7bd8b2d803bace97990a5778ca8fc94a98bb372819e39ad08b5188d`  
		Last Modified: Sat, 12 Dec 2020 14:03:26 GMT  
		Size: 6.1 MB (6145367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cf96c794f990b91261a4562d89886838f6d3f4a9d9116c03daf2b3a3f1b65d`  
		Last Modified: Sat, 12 Dec 2020 14:03:47 GMT  
		Size: 19.1 MB (19133022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f674fd97fba7e780aca677b340a94f0bd86b13bf92148d77df53f142dc1c12d4`  
		Last Modified: Sat, 12 Dec 2020 14:03:42 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc24df6b7b87db1c6e705ea19ec51574a6ed300acb20852a193dd81ac17df94`  
		Last Modified: Sat, 12 Dec 2020 14:03:43 GMT  
		Size: 2.1 MB (2136137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm variant v5

```console
$ docker pull python@sha256:61abbec7611f8196902bf6661d8d92f584c133093dd52ba222e2c1d4c441efa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.2 MB (312221727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362296d681a2b86ddcabf65b7dcdedf118723d416cf195620c70b933365c41f9`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:16 GMT
ADD file:955829a14d270d20f9903754a57858fd2dbe3bcf8845491c1cdccae1e4896249 in / 
# Fri, 11 Dec 2020 02:04:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:45:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:46:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:49:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 09:24:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 09:24:58 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 09:25:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 09:52:50 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 09:52:52 GMT
ENV PYTHON_VERSION=3.9.1
# Fri, 11 Dec 2020 10:05:04 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 11 Dec 2020 10:05:07 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 10:05:08 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 10:05:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 10:05:10 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 10:05:23 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 10:05:24 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d0f09cc3b3e26671eb372263913148f5c37e856980aa747129a90a3e14610461`  
		Last Modified: Fri, 11 Dec 2020 02:14:15 GMT  
		Size: 48.1 MB (48110951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6dfd2752660733cb28140557883aebafb300f8d5feb54cd866371882826509`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 7.4 MB (7362304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70af9e49905885803a3a9fb626687874b912388320ca5bc2ab1f9ee2576787f1`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 9.7 MB (9687464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7a4c35c3d9812b61f1c67d568bd52e4772ae28fe061416d94a4f1fe75c4e8e`  
		Last Modified: Fri, 11 Dec 2020 03:07:26 GMT  
		Size: 49.6 MB (49571487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3473743862d30ca1914ad83b028434bdc4bd69ff5603cf69aa7d61e80f07d03`  
		Last Modified: Fri, 11 Dec 2020 03:08:26 GMT  
		Size: 171.3 MB (171273716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f03e9523072ae79de2125fa7c6f5a6f1e23a1a32ea5d09d0365bb5cd68619a`  
		Last Modified: Fri, 11 Dec 2020 12:13:19 GMT  
		Size: 5.8 MB (5840426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8a89507a783b1cb6b896d87d02366187e7d88d5c70d212eba5c0c16b6e775d`  
		Last Modified: Fri, 11 Dec 2020 12:13:56 GMT  
		Size: 18.2 MB (18238729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3373df98dea38973ac0cddb58ccf4fd2b2d2e231fbb5797d0c0d68553023df6c`  
		Last Modified: Fri, 11 Dec 2020 12:13:50 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a0759223420e3e5f94b20bdf2beaf61b7743d11c9e971704fb1f9ec30ec76a`  
		Last Modified: Fri, 11 Dec 2020 12:13:51 GMT  
		Size: 2.1 MB (2136418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm variant v7

```console
$ docker pull python@sha256:7313f44e112a2f5873f5635f1a848a2b93356f6c6946340b4c384672b1cac943
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303868535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a830011d15c9adaf66005a8c55290a7578f80547f381d0a8257d6ea65ae8fc2a`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:24:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:24:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:28:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 03:54:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 03:54:43 GMT
ENV LANG=C.UTF-8
# Sat, 12 Dec 2020 03:54:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 04:07:57 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 12 Dec 2020 04:07:58 GMT
ENV PYTHON_VERSION=3.9.1
# Sat, 12 Dec 2020 04:21:11 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Sat, 12 Dec 2020 04:21:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 12 Dec 2020 04:21:20 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Sat, 12 Dec 2020 04:21:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Sat, 12 Dec 2020 04:21:21 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Sat, 12 Dec 2020 04:21:34 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 12 Dec 2020 04:21:36 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ebb34ef82f207f1fe2804f394d61205a909e4ec6256fc1aa3a30b484c3176f`  
		Last Modified: Fri, 11 Dec 2020 16:43:39 GMT  
		Size: 7.1 MB (7099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc4c14c5eea8f2b3009ee1de8df43fcf61c0a0d73af4efa97923119eae19bf`  
		Last Modified: Fri, 11 Dec 2020 16:43:38 GMT  
		Size: 9.3 MB (9343469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d9bc5b9d534ac062b6fe74080e2674bdd0caef2d6c12cd1018d79ad0b02a`  
		Last Modified: Fri, 11 Dec 2020 16:44:04 GMT  
		Size: 47.4 MB (47356031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464e679b47b4193d41aa104658d18c56764a55280587949d2c6906ad683c3f91`  
		Last Modified: Fri, 11 Dec 2020 16:44:59 GMT  
		Size: 168.5 MB (168533599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485601594c4b92dee5a1993d590a78e66f51ddc97b8983720ca4b20a166de40c`  
		Last Modified: Sat, 12 Dec 2020 05:22:33 GMT  
		Size: 5.5 MB (5536528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8161ea2d2c11d604ef4782581da0a5680813d1d2e87111205256cbf04b06c52`  
		Last Modified: Sat, 12 Dec 2020 05:22:59 GMT  
		Size: 18.0 MB (17995149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08155e195101048b0e2fd8c699fe1fa8dabd9af0b081d72eb9002aeffc71928`  
		Last Modified: Sat, 12 Dec 2020 05:22:53 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bd84f3918a4935c1289ac7e5a504a179e1f1e09b292ba6554dc58c3bf17c39`  
		Last Modified: Sat, 12 Dec 2020 05:22:53 GMT  
		Size: 2.1 MB (2136386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; arm64 variant v8

```console
$ docker pull python@sha256:f36aa1fb2f7d90308325412b555bb7007dbf6a07280009d2b46b3245b60c9517
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329880887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976dbb5dd9d465c8503572aadf62b8ea8ea34fa7eb7ca2c7de18d235290b6874`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 18:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:53:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 18:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:55:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 08:28:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 08:28:57 GMT
ENV LANG=C.UTF-8
# Sat, 12 Dec 2020 08:29:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 08:38:34 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 12 Dec 2020 08:38:35 GMT
ENV PYTHON_VERSION=3.9.1
# Sat, 12 Dec 2020 08:47:28 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Sat, 12 Dec 2020 08:47:31 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 12 Dec 2020 08:47:31 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Sat, 12 Dec 2020 08:47:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Sat, 12 Dec 2020 08:47:33 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Sat, 12 Dec 2020 08:47:45 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 12 Dec 2020 08:47:46 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c9f56ed15888e5a0a9a8738d53044b1d62ff9f3c8c2857e5cebf782039305`  
		Last Modified: Fri, 11 Dec 2020 19:07:21 GMT  
		Size: 7.7 MB (7682310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33292316eac7d9491a0980a8cc9ba5f3e9cde7e2af0014f8dc10cdae5706b9d8`  
		Last Modified: Fri, 11 Dec 2020 19:07:22 GMT  
		Size: 10.0 MB (9984305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3287f43f5d44b20fe250f2683c57f0330bb0451261ad1d0c3eab9b116b0da52b`  
		Last Modified: Fri, 11 Dec 2020 19:07:44 GMT  
		Size: 52.2 MB (52164628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c6f771d62b3aeedaea9b8db36abed7da0bc14a0ed5e98935de87a1feaeb843`  
		Last Modified: Fri, 11 Dec 2020 19:08:42 GMT  
		Size: 183.9 MB (183870732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b024bfc9f5cc422807713cce155b02540f763743100f4ab299331d8ba2cc1dee`  
		Last Modified: Sat, 12 Dec 2020 09:40:37 GMT  
		Size: 6.3 MB (6259580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01348a7731720fcd655a09f4fc0df92a1701d5321f11fde8ff5d03dbfa84769`  
		Last Modified: Sat, 12 Dec 2020 09:41:02 GMT  
		Size: 18.6 MB (18602372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa06dc4ca3be4d361c7d26ec2118aa5b99e86fcb4f7e96f8ea027c4f9eafeff`  
		Last Modified: Sat, 12 Dec 2020 09:40:57 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbc47cb99870d20f5491ac8af156bb06984a1ee5b3b2879b6f5a08a053f4bb4`  
		Last Modified: Sat, 12 Dec 2020 09:40:57 GMT  
		Size: 2.1 MB (2136411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; 386

```console
$ docker pull python@sha256:9ab438120a1b3a48ab0fbbb897b689c1a79b03dc1a8899231d5ed55dee28b102
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348810239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de93727de36c4f045e4ec542b2897649d8a8d8943849310d4aff06c46b349a22`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:51 GMT
ADD file:5131dbfe4d05a72c50b47e4ee936290486446a3a4dfe832240dd270b0f563542 in / 
# Fri, 11 Dec 2020 02:02:51 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 21:53:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:54:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 08:48:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 08:48:13 GMT
ENV LANG=C.UTF-8
# Sat, 12 Dec 2020 08:48:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 09:08:16 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 12 Dec 2020 09:08:17 GMT
ENV PYTHON_VERSION=3.9.1
# Sat, 12 Dec 2020 09:28:57 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Sat, 12 Dec 2020 09:28:58 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 12 Dec 2020 09:28:59 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Sat, 12 Dec 2020 09:28:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Sat, 12 Dec 2020 09:29:00 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Sat, 12 Dec 2020 09:29:15 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 12 Dec 2020 09:29:15 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d18c9b676b719f51a76e9b6c9cb0781fbe5c36a18cfdcdac473acae10efbb381`  
		Last Modified: Fri, 11 Dec 2020 02:09:16 GMT  
		Size: 51.2 MB (51161209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f6b8ae81f7c117e14ce493f06a12caf05381e28e3e49377f9a8df8faec23`  
		Last Modified: Fri, 11 Dec 2020 22:01:23 GMT  
		Size: 8.0 MB (7981643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550bb3e6c2957b203bf8dd84e95fbae17705a07e090d1494aa9320dec6fae226`  
		Last Modified: Fri, 11 Dec 2020 22:01:23 GMT  
		Size: 10.3 MB (10338820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d57d09060e8546e1c094e2f365eae9cd2fbc6636eb4fa9981b7066d3a3f1400`  
		Last Modified: Fri, 11 Dec 2020 22:01:48 GMT  
		Size: 53.4 MB (53432037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ddf79278d52d7a566157e88a46bea5b94913cc3d89103617609e99376ae5c`  
		Last Modified: Fri, 11 Dec 2020 22:02:48 GMT  
		Size: 198.9 MB (198860674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e32c32e9c5c250f27301cccb58feb2ef67bda334443c3a0cb44fbccbe42c63a`  
		Last Modified: Sat, 12 Dec 2020 13:55:10 GMT  
		Size: 6.5 MB (6489258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05753483868c03fcb7e0d215a92259a3a4628734e6e7b45b4ffd96ed86daae7`  
		Last Modified: Sat, 12 Dec 2020 13:55:43 GMT  
		Size: 18.4 MB (18410190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de256e73cbb65262dfd93be3a80b1bedb776a09f820450961b7f6a7c635beadd`  
		Last Modified: Sat, 12 Dec 2020 13:55:33 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932483b5d649a89a6dc1a8f21bbdd8f0e7231c1555f4c88775bc271b7af199e4`  
		Last Modified: Sat, 12 Dec 2020 13:55:36 GMT  
		Size: 2.1 MB (2136175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; mips64le

```console
$ docker pull python@sha256:6b90c4f33a04bac4495df2163a2341e2ba4de3aff816a736fbeb7dc2e115e789
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.3 MB (324283135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1682915f97de076649fb22fc94362433136f5d8c9e6d3ce90a16b7e6d3fd14c`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:06 GMT
ADD file:de28e706af92bb73003a6ea1969c51666f52e0cd0286cbd99c624f3bc49e4666 in / 
# Fri, 11 Dec 2020 02:03:07 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:54:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 07:09:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 07:09:55 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 07:10:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 08:33:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 11 Dec 2020 08:33:01 GMT
ENV PYTHON_VERSION=3.9.1
# Fri, 11 Dec 2020 09:13:46 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Fri, 11 Dec 2020 09:13:48 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 11 Dec 2020 09:13:48 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Fri, 11 Dec 2020 09:13:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Fri, 11 Dec 2020 09:13:49 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Fri, 11 Dec 2020 09:14:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 11 Dec 2020 09:14:11 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6057d98f1b0dc943648ced0ad33983792fadf9f1b0eaac90fd62165829122340`  
		Last Modified: Fri, 11 Dec 2020 02:09:27 GMT  
		Size: 49.0 MB (49022625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e90ff301a3d0d856fb4e7e6911036aa68b68b2c71f3be423ef654b42f0be98`  
		Last Modified: Fri, 11 Dec 2020 03:02:19 GMT  
		Size: 7.2 MB (7232151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9b5cb9bd92be17ad45be69b85a627b3fc368a8486765bd25f83e7916c0484`  
		Last Modified: Fri, 11 Dec 2020 03:02:18 GMT  
		Size: 10.0 MB (10016229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576e15dbb62b557fb4030dd6fbc86324c2c98d2409f9b1fe6409accacd47f6a`  
		Last Modified: Fri, 11 Dec 2020 03:03:10 GMT  
		Size: 50.8 MB (50842772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b741f56358a0d13dd0e3f805c58d4bf51981ad3724b1096ab7a52575b0aa00`  
		Last Modified: Fri, 11 Dec 2020 03:05:24 GMT  
		Size: 179.8 MB (179823383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1898aaf3c579332781a853cd9c462c757bb08e2e4e6d71bd6166be5c1657e1f6`  
		Last Modified: Fri, 11 Dec 2020 13:38:50 GMT  
		Size: 6.5 MB (6455165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d767225e6bd7b657c094c4664be27476b3e1dd4aa5823f651d52d135605c44a`  
		Last Modified: Fri, 11 Dec 2020 13:40:01 GMT  
		Size: 18.8 MB (18754346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037231469b638539c7ee6dfaf41ca888e2b4e820016bb099e18d3b74bc84e747`  
		Last Modified: Fri, 11 Dec 2020 13:39:48 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955d24d774926fb25abe2778f1a6f44bff0a87bb784466ed1d40810fd2c3be8f`  
		Last Modified: Fri, 11 Dec 2020 13:39:49 GMT  
		Size: 2.1 MB (2136232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; ppc64le

```console
$ docker pull python@sha256:95a9d9f3e6b7f9f9715fe3264181f400d3db4fa7691b621d14152992725c399c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362352434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de4c0fb3f60e346c642ee6278f8c4edfc84972c187ab7407e8fb5c2f5e980ad0`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 17 Nov 2020 23:22:28 GMT
ADD file:b5112ae3b22de1d8a373191ad01151a6c1cdde605887b1836672be39787e2213 in / 
# Tue, 17 Nov 2020 23:22:37 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:55:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:57:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:59:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:20:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:26:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:27:03 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:28:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:59:11 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 08 Dec 2020 01:43:46 GMT
ENV PYTHON_VERSION=3.9.1
# Tue, 08 Dec 2020 01:54:14 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Tue, 08 Dec 2020 01:54:30 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Dec 2020 01:54:36 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Tue, 08 Dec 2020 01:54:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Tue, 08 Dec 2020 01:54:43 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Tue, 08 Dec 2020 01:55:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Dec 2020 01:55:16 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:94e00adb98ff1f971add74025ff2a8ca87e003568d828bdb0df26ecd46c269a2`  
		Last Modified: Tue, 17 Nov 2020 23:31:43 GMT  
		Size: 54.1 MB (54143125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46d858a6e31a5aa25fd9c527cdee95fe08fc11f45038212d1c5c7e52dc7b40`  
		Last Modified: Wed, 18 Nov 2020 01:53:05 GMT  
		Size: 8.3 MB (8255326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfab907b4d9fde9fb35f17a366b653e709c31cbce8602a2ae23c23d39524820`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 10.7 MB (10727375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157cce210a3874859c02d469911ddfc967ed435c3c04ebf12cdad81fe199cef0`  
		Last Modified: Wed, 18 Nov 2020 01:54:24 GMT  
		Size: 57.5 MB (57455140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c205957dfc9cb35b737f51ec6985e8bbfa793cabfde43085a053e7f5cf44ac`  
		Last Modified: Wed, 18 Nov 2020 01:57:37 GMT  
		Size: 203.1 MB (203086260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d76ab441741175eaddd328ea78d468be8bed8c957c980bc8dc7c25468b7639e`  
		Last Modified: Wed, 18 Nov 2020 10:02:18 GMT  
		Size: 6.9 MB (6893018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138953bd3f86ea1f4c5c5ec59d467184bd9845b2f30d06f99307873990ef399`  
		Last Modified: Tue, 08 Dec 2020 02:28:38 GMT  
		Size: 19.7 MB (19655516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf906535542d96a5ed71d7a65b35136b828a94157f1c9b6d509971839195adf`  
		Last Modified: Tue, 08 Dec 2020 02:28:34 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bc77a4cabfb0a7427f8d815a02f15d0b05511574b17a8efc59b9349a211fa5`  
		Last Modified: Tue, 08 Dec 2020 02:28:35 GMT  
		Size: 2.1 MB (2136440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - linux; s390x

```console
$ docker pull python@sha256:9326223a196411929d6edd76eb49df935c8933c194244bfa27ba78698650a6c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321446632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6221bb08adfc9f5a14334933a59ffb6693182252f808bfafb8a2d7175b4343d`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:47 GMT
ADD file:b48379f9d2c111607924e8c59c2769c735341a59df0d6819d8a4b3e44f5457b0 in / 
# Fri, 11 Dec 2020 02:11:54 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:03:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:06:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 02:18:02 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 02:18:03 GMT
ENV LANG=C.UTF-8
# Sat, 12 Dec 2020 02:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 02:24:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 12 Dec 2020 02:24:53 GMT
ENV PYTHON_VERSION=3.9.1
# Sat, 12 Dec 2020 02:31:21 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& python3 --version
# Sat, 12 Dec 2020 02:31:25 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 12 Dec 2020 02:31:26 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Sat, 12 Dec 2020 02:31:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Sat, 12 Dec 2020 02:31:27 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Sat, 12 Dec 2020 02:31:38 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 12 Dec 2020 02:31:39 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:b8cd59e115fe85cdffdb9750beb150c189e768249dc100d22cab4733fb0c7247`  
		Last Modified: Fri, 11 Dec 2020 02:16:44 GMT  
		Size: 49.0 MB (48968242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0eb33d878287686bed77cfef9cecb3fd540caf075a646ed34afdb64288ae74`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 7.4 MB (7386652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7571827f1162945abd5d70aa40ae2489e866f25a600c027f482c4dbd5bfc88`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 9.9 MB (9883064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9e36ebe77bd8ffdf1d40b3ce51f765116b1fdc5aa75b3bd774c9388233fc72`  
		Last Modified: Fri, 11 Dec 2020 16:16:04 GMT  
		Size: 51.4 MB (51379787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01320660a363425b4f9f32a4b413821e56ab6777e437330fb62f29ef4ddca113`  
		Last Modified: Fri, 11 Dec 2020 16:16:38 GMT  
		Size: 176.8 MB (176832403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b27ff98927ade867dbc1a73b0d1413d268df3879bcb7b56f82897b0d34efbe`  
		Last Modified: Sat, 12 Dec 2020 03:02:00 GMT  
		Size: 6.1 MB (6058810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e126e77d6b9f93d1f62a8067939430e566ebd7a23558d82ac9880f808d2467`  
		Last Modified: Sat, 12 Dec 2020 03:02:23 GMT  
		Size: 18.8 MB (18801042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4829cb4e93c3479f188f5639d4f2ea62a250502aa4a8a7491f94b256dec9b7ab`  
		Last Modified: Sat, 12 Dec 2020 03:02:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b85402277a67582c11dc599f3aadcc7307bb73250c2e0ad16228a1ae1f4e8`  
		Last Modified: Sat, 12 Dec 2020 03:02:20 GMT  
		Size: 2.1 MB (2136398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull python@sha256:4d6ad94e94ebf0ee499d3e50c8bac18bd2200d38f351576fc9851a27434c438a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459984427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b74f2e28c3ce4c4bc7d69af6706f80e7f5ef0b5dad8173bf16125219d4a3ef`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 17:43:53 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Dec 2020 17:50:46 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 09 Dec 2020 17:50:47 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 09 Dec 2020 17:52:27 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:52:28 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Wed, 09 Dec 2020 17:52:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Wed, 09 Dec 2020 17:52:30 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Wed, 09 Dec 2020 17:53:17 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:53:17 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94dd2e25fa016037458dfad84ce68c5f51c1d9a517cbb1d6a9d9037fb27a47b`  
		Last Modified: Wed, 09 Dec 2020 18:12:33 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43c1e1f0964479f228315ffd503fded10414f92c67f89d956a85cd6afbb593e`  
		Last Modified: Wed, 09 Dec 2020 18:13:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4905032a1c78aca05b445c178cfb9f2b232e664998995eec7a7ec6c5e9c0a11`  
		Last Modified: Wed, 09 Dec 2020 18:13:35 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c025c30481676471955858b2228cc152047dd812f258db8bb69da882bdfc85d`  
		Last Modified: Wed, 09 Dec 2020 18:13:44 GMT  
		Size: 58.8 MB (58753562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897c43b058d364c0cfe42936994f818c9a8b09b0ea08bb55aa6fc819d1ed2166`  
		Last Modified: Wed, 09 Dec 2020 18:13:33 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f8f24f052dc99033501acebee22fac2231edee372a691b66e128b885d2486d`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ab626fe701f307562f1e26401acffce062852c9f94f8594c06bee4ce07f9e8`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b216f88a03dd996b4d093e4bd48c81c3228f56ecb408ca5474a05f3ff2f68026`  
		Last Modified: Wed, 09 Dec 2020 18:13:50 GMT  
		Size: 10.3 MB (10347266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2d6922b1ca8f13967e7ed7af3f36f964f09aa3fa5fe8e15e7570cb232bf81`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:latest` - windows version 10.0.14393.4104; amd64

```console
$ docker pull python@sha256:9ce7afa14a81778ee17773f926931b87da7e3985a393c5bf49c80a4c4289d036
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5844029938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d866ede06291b789f8dfdf8aa3b0986295b32cf13902094bde50accd98f1fcbf`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 17:46:34 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Dec 2020 17:53:27 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 09 Dec 2020 17:53:28 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 09 Dec 2020 17:55:43 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:55:44 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Wed, 09 Dec 2020 17:55:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Wed, 09 Dec 2020 17:55:45 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Wed, 09 Dec 2020 17:57:28 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:57:29 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18db14afcdaf52f01f53af42090925b5c891dfe60bedf017c011f3a9f08413b`  
		Last Modified: Wed, 09 Dec 2020 18:13:02 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ca29429f89cd854a8f504abd4eab2422cc201417b761cb25739da44e3d8f17`  
		Last Modified: Wed, 09 Dec 2020 18:14:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1653b9b41b03210c8d1c3c8e78f6f3b736d190f1e837b58e198b57564904287e`  
		Last Modified: Wed, 09 Dec 2020 18:14:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfda6dd459e164fb22907204f47203086a18db50ac0fc85c2332ece599eb7b`  
		Last Modified: Wed, 09 Dec 2020 18:15:21 GMT  
		Size: 59.5 MB (59511092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffe81a4096bff4d1bf0523da2616ea9b1f60e9a4f2ea316062cca468f359bd6`  
		Last Modified: Wed, 09 Dec 2020 18:14:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2885308362db6236732ab5d3c4b08585b50ba5c271b2962981d7260d4dce0a5f`  
		Last Modified: Wed, 09 Dec 2020 18:14:10 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582349fec9eadd94781cd3719864cc1329516eb1c5acaad75a5468241f656041`  
		Last Modified: Wed, 09 Dec 2020 18:14:11 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d5ce8d444da26a15b607a6da87306131802e476db2b93eec8f33b96a36aa28`  
		Last Modified: Wed, 09 Dec 2020 18:14:14 GMT  
		Size: 15.7 MB (15665700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d9625bb9cca0bf263ae33004e926769ccd433ef06a9d2c36df018cd0bdeac0`  
		Last Modified: Wed, 09 Dec 2020 18:14:09 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
