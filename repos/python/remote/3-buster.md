## `python:3-buster`

```console
$ docker pull python@sha256:9632dcfc08257c69ade5eec76970a9d4ae39926b456ed7a5b7a078881dbf30c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `python:3-buster` - linux; amd64

```console
$ docker pull python@sha256:eeec995b11398c350fbd86be8e2442d6695fa6d46bd5b08900072beb91135dcd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.9 MB (342920047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef07326642ffc2bef8022d338d20215048dffce365c3dd5944e2853a1d11edfc`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:44:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:45:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:45:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:09:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 14:09:14 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 14:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:09:21 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 13 Sep 2022 14:33:55 GMT
ENV PYTHON_VERSION=3.10.7
# Tue, 13 Sep 2022 14:44:17 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Tue, 13 Sep 2022 14:44:18 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 13 Sep 2022 14:44:18 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Tue, 13 Sep 2022 14:44:18 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 13 Sep 2022 14:44:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Tue, 13 Sep 2022 14:44:18 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Tue, 13 Sep 2022 14:44:24 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 13 Sep 2022 14:44:24 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b34aaa3cba7676359d4f9d29333c92bd9f448969b07f56bb8482398a5dc53c6`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 7.9 MB (7857266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a443ab54eaa5455912b469fb6d8b621ade658cd0afef9c706b7e37085004b25`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 10.0 MB (9998148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cacf42b5677aa20eb8fff5102f7482828f27555a167f49da0597869f91002f`  
		Last Modified: Tue, 13 Sep 2022 03:51:39 GMT  
		Size: 51.8 MB (51844022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2334d631be5e1dc71eaed4b65f73ba5378f40a7bcf7e474645e9523cf494451c`  
		Last Modified: Tue, 13 Sep 2022 03:52:15 GMT  
		Size: 192.6 MB (192593709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b7372a07981d30a2709fc23db3c92d6e790a962a140121174524c86ea1af60`  
		Last Modified: Tue, 13 Sep 2022 15:26:28 GMT  
		Size: 6.1 MB (6146355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ac4c9d0d30b3d1e902f6af9981bef02a9e4072fc146a640761047aab30012e`  
		Last Modified: Tue, 13 Sep 2022 15:27:12 GMT  
		Size: 21.0 MB (20996023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e49764c5f834e2deebb568528e97abd0fed10b09cbe2257a3e03895cbe4aa58`  
		Last Modified: Tue, 13 Sep 2022 15:27:09 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d3625321d55fa66019d0ab2bb7afbfa3db19c17b379fe7c1d7bb83029e40af`  
		Last Modified: Tue, 13 Sep 2022 15:27:10 GMT  
		Size: 3.0 MB (3043916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; arm variant v7

```console
$ docker pull python@sha256:a6797e9fc64ff392f51fd358a63a183a1335b4ab91934c9456ab424e2d9a5395
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.9 MB (306941157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad9938ae25ad0fd3c125b755a652a431cf26cfc5a0709cf32f86123ecfa7c46`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:03:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 08:13:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 08:13:14 GMT
ENV LANG=C.UTF-8
# Wed, 24 Aug 2022 08:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 08:13:21 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:54:00 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 23:26:00 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 07 Sep 2022 23:26:01 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 23:26:01 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 23:26:01 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 23:26:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 23:26:01 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 23:26:15 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 23:26:16 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b803711841bad336591ae6cde869b0acee5e53607ac006c3205ce3f2594f71`  
		Last Modified: Tue, 23 Aug 2022 13:14:52 GMT  
		Size: 168.7 MB (168701019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be825887562d3aeb37c06f5712f7c867cccc2f8132f698d8276d38e5475cc7c`  
		Last Modified: Wed, 24 Aug 2022 12:01:13 GMT  
		Size: 5.5 MB (5536440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88953c2dec0641b24fcad04c19bf25db086998ed2b2f0217e77b56b31397578f`  
		Last Modified: Thu, 08 Sep 2022 03:35:15 GMT  
		Size: 19.9 MB (19895269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0605f7e1e448571f22062e2dafc621b86a362899bef29dfe2f597da78b54d78c`  
		Last Modified: Thu, 08 Sep 2022 03:35:11 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb7249b46e94853b53c1f125cfd0dcc85bc3fc97a8c880742708c149c340d5a`  
		Last Modified: Thu, 08 Sep 2022 03:35:12 GMT  
		Size: 3.0 MB (3043949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:32929ba4895b7eb82205f2e99c93d945aace883374736efeba00bc17dd903d2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.5 MB (332478216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c9d35415f4468ddc0b223ec8b3f4517bc50a572e720eb025f070c7b74e8194`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 08:37:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 08:37:07 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 08:37:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 08:37:16 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:01:39 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 22:11:22 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 07 Sep 2022 22:11:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 22:11:25 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 22:11:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 22:11:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 22:11:28 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 22:11:34 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 22:11:35 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34806818c453e9a369973b475f26ada73304ea74e3ae1860af58abbe6872a7c`  
		Last Modified: Tue, 23 Aug 2022 02:38:56 GMT  
		Size: 184.1 MB (184087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60c6448c2ed3436d80dfc7ea0076b662bfbde08a3af07f348f1963c37616aab`  
		Last Modified: Tue, 23 Aug 2022 11:04:38 GMT  
		Size: 6.0 MB (6017659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f872275687e699cd0e260227e6bf9b08b915476117bde67aa6a5a1828c575`  
		Last Modified: Thu, 08 Sep 2022 00:42:37 GMT  
		Size: 20.4 MB (20435951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918aff0809820ad64c8f39f7d590590c6e000c6a6457be32cc46c4779dde23e`  
		Last Modified: Thu, 08 Sep 2022 00:42:33 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3836b11b1f1788f459bfc62fe8b206e8ae8056e944b06d548073e4e5b8a7f71f`  
		Last Modified: Thu, 08 Sep 2022 00:42:34 GMT  
		Size: 3.0 MB (3044883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; 386

```console
$ docker pull python@sha256:ec22f776cecbaa42d303bc8e92f1ca69c262316f57fae0b11cb6c70d057c2102
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351620157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215dc063cb61f805583c6e7c12cb595e26f0eea99317ebd02fce07433ae76bb8`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:56 GMT
ADD file:abd47beae46939f6ebc8cc566b1f23f170bd1b9318b1ef10dd16ea4209140bd0 in / 
# Tue, 13 Sep 2022 01:39:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 04:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:52:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:37:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 14:37:42 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 14:37:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:37:50 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Tue, 13 Sep 2022 15:10:41 GMT
ENV PYTHON_VERSION=3.10.7
# Tue, 13 Sep 2022 15:23:23 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Tue, 13 Sep 2022 15:23:24 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 13 Sep 2022 15:23:25 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Tue, 13 Sep 2022 15:23:26 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 13 Sep 2022 15:23:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Tue, 13 Sep 2022 15:23:27 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Tue, 13 Sep 2022 15:23:35 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 13 Sep 2022 15:23:36 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:a0702c36e95be838f5e174ceb286969e8527f17111141f2c8a8ecda44d0a14d4`  
		Last Modified: Tue, 13 Sep 2022 01:45:44 GMT  
		Size: 51.2 MB (51202973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be8b5f305f5479b300e03b1ee4b19b0008833df2d269be3dcb6caff4e790abb`  
		Last Modified: Tue, 13 Sep 2022 04:58:21 GMT  
		Size: 8.0 MB (8024065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2875198ef388281cfb712c18bf183cea7a0597a6b05b7894e9e91d2a585e1d`  
		Last Modified: Tue, 13 Sep 2022 04:58:21 GMT  
		Size: 10.1 MB (10123769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19d1325da1b59cc6eae7d3e5a5bf3488a953a4ba0e68c14fc76c0fd31ebe91f`  
		Last Modified: Tue, 13 Sep 2022 04:58:39 GMT  
		Size: 53.4 MB (53447031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f345acca58a9abc499b31bb97db4ded802e9f498023efcd5c7ecd007f2e608a4`  
		Last Modified: Tue, 13 Sep 2022 04:59:13 GMT  
		Size: 199.1 MB (199082132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0773130626e68b30a5f165297af23fe515ae7dd0b6e8c6586a6716bb9b19d1e`  
		Last Modified: Tue, 13 Sep 2022 16:10:39 GMT  
		Size: 6.2 MB (6249485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca0b9e0daa09e9c120c36fea301d3985d8b2dc37ec91a60643437846f9d662`  
		Last Modified: Tue, 13 Sep 2022 16:11:27 GMT  
		Size: 20.4 MB (20445550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5e74f713c83c838401eea028c93c7baa7a05f3d7cde303ec3c9345dea039`  
		Last Modified: Tue, 13 Sep 2022 16:11:24 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99525c8f5c46abe8f8b9c909d454035588cca0b0c45f97bb63acec39dad7c109`  
		Last Modified: Tue, 13 Sep 2022 16:11:25 GMT  
		Size: 3.0 MB (3044919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
