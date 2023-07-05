## `pypy:2-bullseye`

```console
$ docker pull pypy@sha256:713df40c55a49dffe8dba227d30027184f0ec7a3498c6661cf5fdd58b3253076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:78d6604997c44a40f7c64e39ad3af8da6c08752187e8b8ddecfabb11ea4bb04c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.6 MB (358596038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c104a0cf75963f2105e10aa8f7156127c0d8745266f8d662bdc6422e406e1ba9`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:31:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:52 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 04:25:52 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:25:52 GMT
ENV PYPY_VERSION=7.3.12
# Tue, 04 Jul 2023 04:31:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 04 Jul 2023 04:31:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 04 Jul 2023 04:31:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 04 Jul 2023 04:31:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 04 Jul 2023 04:31:30 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f8721393bc605f2b915d80eb2ad6d5219db374f36bbd1fee99b99174a0a4ca`  
		Last Modified: Tue, 04 Jul 2023 03:53:17 GMT  
		Size: 196.9 MB (196850887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57e27e92fed5af76e0cf12cd70b4e2d4a3d0228ff060abb8056fcc7dcb8ff05`  
		Last Modified: Tue, 04 Jul 2023 04:33:45 GMT  
		Size: 3.2 MB (3210875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e8d30b10e4ff0ee4c9feb1830f7b43f070780acf81584c4755d97a329018a6`  
		Last Modified: Tue, 04 Jul 2023 04:37:02 GMT  
		Size: 31.2 MB (31237041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693498974dae01028946688c80ddee4c391f93cec6714719c5ef1a92fb8fd1ea`  
		Last Modified: Tue, 04 Jul 2023 04:36:57 GMT  
		Size: 1.9 MB (1896562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:4446345d4c7d6be89b29840004e3c7450d062d92c13203d3daa8936c29ce0117
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.2 MB (348224146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75710ab8f9ce32b24d4af3aaa928ebed64d21b97fbb2534bf02ce6a8cd399ec8`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 21:26:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 21:26:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 21:26:19 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 21:26:19 GMT
ENV PYPY_VERSION=7.3.12
# Tue, 04 Jul 2023 21:28:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 04 Jul 2023 21:28:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 04 Jul 2023 21:28:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 04 Jul 2023 21:28:24 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 04 Jul 2023 21:28:24 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5fa66dbb545c6ff93c768ac595d874b2f22053e8d2f842f4b6ccc310ebfe0c`  
		Last Modified: Tue, 04 Jul 2023 06:22:15 GMT  
		Size: 54.7 MB (54676075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790673d5b08f786a9f9e0a1db5dd3941e80d10bde172f69852e2c405b2eb3ad3`  
		Last Modified: Tue, 04 Jul 2023 06:22:40 GMT  
		Size: 189.8 MB (189777942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf9ecfbbb01f1ad8608730438c757ed1c342a552d8bf79ae5a59f2f424a1291`  
		Last Modified: Tue, 04 Jul 2023 21:29:47 GMT  
		Size: 3.2 MB (3214899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d352e252887ffb59fa597702d53aa7bb095381ee6694cf21c550db4f4a10c2c`  
		Last Modified: Tue, 04 Jul 2023 21:31:29 GMT  
		Size: 29.2 MB (29207873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78522710d9762045d3bef287a0b5c57a34eff88687438ca1b2db7741a1d20a9b`  
		Last Modified: Tue, 04 Jul 2023 21:31:25 GMT  
		Size: 1.9 MB (1896631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:467c9804b12a9fd4008d4d1b5eed145708404ce8d89152a0ebc98b882cd384a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360544578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce06665db9d1adaf935a96c7724908fd085252887b303def90a893d34cb96e2a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:31:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:32:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:39:04 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 23:39:04 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 23:39:04 GMT
ENV PYPY_VERSION=7.3.12
# Tue, 04 Jul 2023 23:45:14 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux64.tar.bz2'; 			sha256='1a61a2574b79466f606010f2999a2b995bd96cd085f91a78ebdd3d5c2c40e81d'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-aarch64.tar.bz2'; 			sha256='e04dcb6286a7b4724ec3f0e50d3cc1ba8583301dd1658c06d7f37599e4201c59'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-linux32.tar.bz2'; 			sha256='abf3ae477bd0e526ac6dcefe0bfa845e1535aa053342c0d641219bfcde4b9b56'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.12-s390x.tar.bz2'; 			sha256='80c0154d8b0949f9dc6a227c322abbc9590c8ae4c9f11c13bf4022aa38b82064'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 04 Jul 2023 23:45:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 04 Jul 2023 23:45:15 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 04 Jul 2023 23:45:20 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 04 Jul 2023 23:45:21 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee301eb66e57dfaf79983158c75b77a7775e1b6216c45ce247c6fac3786a46`  
		Last Modified: Tue, 04 Jul 2023 05:39:53 GMT  
		Size: 55.9 MB (55922990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28c7ac3e45d13ee62a7daff4eb413a3752789ab4b5620de47a04abff3a358cc`  
		Last Modified: Tue, 04 Jul 2023 05:40:36 GMT  
		Size: 199.8 MB (199766345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e104c0712e116cd7a7f1d7ba99b401e99936cee5abaeb1210c6248337f047a`  
		Last Modified: Tue, 04 Jul 2023 23:47:45 GMT  
		Size: 3.4 MB (3360923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f2d213b2fb870d32a136d1ff21df12904398831f74dcd538cadfcccd4cba5`  
		Last Modified: Tue, 04 Jul 2023 23:51:23 GMT  
		Size: 27.3 MB (27293307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f798c8ae50f99f2f6b3b0c95648577304c7b72649498640c0ac3890c44e60b`  
		Last Modified: Tue, 04 Jul 2023 23:51:17 GMT  
		Size: 1.9 MB (1896652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
