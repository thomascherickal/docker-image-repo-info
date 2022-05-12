## `python:buster`

```console
$ docker pull python@sha256:71568c9d50183ac4682a38f9d29d71c66c528172f0312c6f31319a822d6a0fa5
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

### `python:buster` - linux; amd64

```console
$ docker pull python@sha256:c11dac2b90849202cd16083010483af6528e4f085ef3249aaeed27e7fee9d86d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.3 MB (342267788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e347508141d07578de92da0715eea757ab36b79340771e2b8787a236481dc96`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:51:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:39:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 06:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 06:39:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:39:44 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 07:28:45 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 07:38:58 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 07:38:59 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 07:38:59 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 07:38:59 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 07:38:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 07:38:59 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 07:39:06 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 07:39:06 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0162432a49c07aa492d3e1031af58a9a9f9b22acde859829434e5a54d019aa1c`  
		Last Modified: Wed, 11 May 2022 01:58:46 GMT  
		Size: 51.8 MB (51843657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee8ddc463fd0224112f41976e81d15dd46444f93185d9cde6203a0185857be2`  
		Last Modified: Wed, 11 May 2022 01:59:19 GMT  
		Size: 192.5 MB (192482405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80df26a7220cfa0df39e96a639f1d09d2525776e51087ffa7129624a0523f76`  
		Last Modified: Wed, 11 May 2022 09:14:35 GMT  
		Size: 6.1 MB (6146217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1651b2cc50ad3b2f74b71e8f2142567e7a0b0ca27b2c9f417cdc60eb8a2b1c5c`  
		Last Modified: Wed, 11 May 2022 09:15:48 GMT  
		Size: 20.6 MB (20631316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cbffa5fb894011e894dc54a77a0b192cd696b3481c7afffa54745c752826df`  
		Last Modified: Wed, 11 May 2022 09:15:44 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdbe0d5142634578a7bf8339a0826dd2fb07592ffc20ba9d850059759166b15`  
		Last Modified: Wed, 11 May 2022 09:15:45 GMT  
		Size: 2.9 MB (2872300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; arm variant v5

```console
$ docker pull python@sha256:27f7d1344fc3e6e9b8dfa5fd734711d66fb2f2ba33df380ae7622aba1b71af3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314772286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee26d4310edb54fe1ac191c810c3d9a78f49d678edaeb6c7d7395bd6e52737c2`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 00:51:01 GMT
ADD file:8292d961a3aa3c4584c010be23306dbea6f52d4f69fe30d2b3ae6d2f8cb91f98 in / 
# Wed, 11 May 2022 00:51:02 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:11:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:14:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:11:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:11:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:11:36 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 16:09:20 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 16:37:51 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 16:37:53 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 16:37:53 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 16:37:54 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 16:37:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 16:37:54 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 16:38:09 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 16:38:09 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:c49f9a696043c9b0e9c645a07e1bd105d319cdcc2a580c36b676431549349006`  
		Last Modified: Wed, 11 May 2022 01:06:38 GMT  
		Size: 48.2 MB (48157520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e1558e9432b31779c9f8031852fa3d04976b885da3cb16b17df0306315d71a`  
		Last Modified: Wed, 11 May 2022 02:33:16 GMT  
		Size: 7.4 MB (7400470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a934c6b94649dc17b407a076ca8c0c7bcec34754b3ebb8a184af9bdd71a7b51`  
		Last Modified: Wed, 11 May 2022 02:33:16 GMT  
		Size: 9.7 MB (9687677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaace8b36f9b1d3eb3b5996d8ce055793ead0ddf31c444be7594a8310b7860c`  
		Last Modified: Wed, 11 May 2022 02:34:03 GMT  
		Size: 49.6 MB (49583813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2909bfcbc90f525736b507b38e7ace65dbf74990a4e5e8455d45544ee9f097`  
		Last Modified: Wed, 11 May 2022 02:35:58 GMT  
		Size: 171.4 MB (171420596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14804c490dbaf4a277c7ed63ecb7175c06b600a2c73e603f30d45aac159446ac`  
		Last Modified: Wed, 11 May 2022 19:40:38 GMT  
		Size: 5.8 MB (5840777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcf5d6d9cbbbbbd0fa4f77a77b70cc95c643391ef5492e95111d6d6d5f372dc`  
		Last Modified: Wed, 11 May 2022 19:42:06 GMT  
		Size: 19.8 MB (19808897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867b245319d1664333bf79e66a8ac6f6da4734623a14196631dc1323e38070b0`  
		Last Modified: Wed, 11 May 2022 19:41:53 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a76a7f72c7177b2116ad83fd3963d1745ad57dea34a9250219db153fdc8b83d`  
		Last Modified: Wed, 11 May 2022 19:41:55 GMT  
		Size: 2.9 MB (2872303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; arm variant v7

```console
$ docker pull python@sha256:68cb3adb1555e60acb1ffe4e91819e87d4540e25f1e81e08df06aaf734f2d351
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.4 MB (306374883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f85b42be325b870bcbdf4035f61ca125ce95331ea140db5c206ee52c68518e`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 23:33:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 23:33:15 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 23:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 23:33:31 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 12 May 2022 02:27:52 GMT
ENV PYTHON_VERSION=3.10.4
# Thu, 12 May 2022 02:59:43 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Thu, 12 May 2022 02:59:46 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 02:59:46 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 02:59:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 12 May 2022 02:59:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 02:59:48 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 03:00:02 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 03:00:03 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f12fd5e3b5778467cb9879a44c76a2061dc01bd3fdbf773a2aaaaa384784222`  
		Last Modified: Thu, 12 May 2022 07:42:24 GMT  
		Size: 5.5 MB (5536768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802a6ef56c40f808fd118922e1aacdf3df65e08a1c1e87a8d7a6ec5fd1ab18de`  
		Last Modified: Thu, 12 May 2022 07:44:27 GMT  
		Size: 19.5 MB (19527119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850d8c7f161134fa063bb4e1d15e9bcd8e6b51258a056427d3281b027f1b4bfa`  
		Last Modified: Thu, 12 May 2022 07:44:14 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cade681f66755fbb6fcba27a7b3246166f5c50b91869779b97eb74b06bccdc2`  
		Last Modified: Thu, 12 May 2022 07:44:16 GMT  
		Size: 2.9 MB (2872389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:5bafba3844e6584625ab6d348c817fdcc9c23ca813bdf56b9df2925683cd8e31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331891949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8083b7abbc7adb52b95e6ce05e4a9aedc53b9c3738ebe088012fb2c2a6acf54d`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:21:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 09:21:20 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 09:21:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:21:27 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 10:14:05 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 10:23:53 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 10:23:54 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 10:23:55 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 10:23:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 10:23:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 10:23:58 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 10:24:05 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 10:24:06 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de10266dfd463bca117813d26548c5d6779bb7828b6fbbfd2b3fba2a0c33925`  
		Last Modified: Wed, 11 May 2022 11:49:20 GMT  
		Size: 6.0 MB (6017658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25106c7d297e9b441ea5ca8663e18be4f10280304ec10fa4d1618fe5725f3fb`  
		Last Modified: Wed, 11 May 2022 11:50:43 GMT  
		Size: 20.1 MB (20058035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a062a8fed5125056c1266e2f54650d15a6cc18c0aefee2a6048e649a4514ca`  
		Last Modified: Wed, 11 May 2022 11:50:40 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40049b41ab365d7931896588f06574a87394c3f1c21807fedfc6221e3e678cf4`  
		Last Modified: Wed, 11 May 2022 11:50:40 GMT  
		Size: 2.9 MB (2871810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; 386

```console
$ docker pull python@sha256:d867c62f2c1636779944765d6eac0f38464ff0723a9d468bba22c497a50d1715
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350993906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655fbdad08ae652c365b193a6bfa82e5aeae48cdf4f13ff12bc191ea6bd39029`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 01:39:25 GMT
ADD file:03855eb19b36aa184d26264c1416a11ac7661faddae3436aad12661bb4c6e656 in / 
# Wed, 11 May 2022 01:39:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:13:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:14:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 11:48:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 11:48:27 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 11:48:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 11:48:35 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 12:54:32 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 13:07:05 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 13:07:07 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 13:07:07 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 13:07:08 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 13:07:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 13:07:10 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 13:07:18 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 13:07:19 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:5b096db137216fbea3d646b6cad3959b69b6a1d27ff5f31bd01048df4a7e6c0a`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 51.2 MB (51199249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea31d1a573a95302db6857fc201016b7c6b8f21d0f56e011ec26f49e9d36b6`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 8.0 MB (8022259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1841293ac8ab91433085e85c8c899e4324ca8f84a2cf4300cb5410542e39f4`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 10.1 MB (10121987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c221acbd6711627d003a42bc75312b3994313814f1ba7a82f10f1e0e37b30b8`  
		Last Modified: Wed, 11 May 2022 02:23:28 GMT  
		Size: 53.4 MB (53442818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d4335971c3c6abcc0cee05c5dc4d86bb28ee87ad0592c808e4454c0579e3ce`  
		Last Modified: Wed, 11 May 2022 02:24:03 GMT  
		Size: 199.0 MB (199011140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeaa59cd603a4610a9b126e662a27305fe571e798aac418a5f71933c9168dac`  
		Last Modified: Wed, 11 May 2022 14:44:37 GMT  
		Size: 6.2 MB (6249277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ad7c9a004e263bb286802912f676680c6ead7509859105361764bdf2dd84d5`  
		Last Modified: Wed, 11 May 2022 14:46:04 GMT  
		Size: 20.1 MB (20075124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1e7fac6db7b4fd12ddef77e5c2e6a369ac1d8d889b47d7366fc24b10385f9c`  
		Last Modified: Wed, 11 May 2022 14:46:00 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c12416563608b1fbf46304fc85f9e44d8023e5d8bdbc7b469492a299307edd`  
		Last Modified: Wed, 11 May 2022 14:46:01 GMT  
		Size: 2.9 MB (2871819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; mips64le

```console
$ docker pull python@sha256:9acda31841d1c1baa2a811ccd1c23ec624fb271219346fcd814c7f92c7e1059a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.5 MB (326501322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa8518fee803ff39d0da0bc7b3ffdffd2c5a6c92ec4828abd17c5e74b0b9c447`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 02:24:09 GMT
ADD file:8196bde1e8989094969bcfd079f2fceac263a32d24556ea55bb20a53b915b112 in / 
# Wed, 11 May 2022 02:24:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:16:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 07:46:42 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 07:46:48 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 07:47:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 07:47:31 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Thu, 12 May 2022 10:48:52 GMT
ENV PYTHON_VERSION=3.10.4
# Thu, 12 May 2022 11:58:21 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Thu, 12 May 2022 11:58:30 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Thu, 12 May 2022 11:58:37 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Thu, 12 May 2022 11:58:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Thu, 12 May 2022 11:58:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Thu, 12 May 2022 11:58:55 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 11:59:26 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 11:59:33 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:737cd4f99975def8d1d06011f9f8adfb43e6149a232c24f0bcfac82bbb3d809c`  
		Last Modified: Wed, 11 May 2022 02:34:25 GMT  
		Size: 49.1 MB (49073768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5aa50fe74813ad1c212b9d93aaec284182c36ee0a9c1396c829c0cb4a914c3`  
		Last Modified: Wed, 11 May 2022 03:40:26 GMT  
		Size: 7.3 MB (7272760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e33346bc90837c57612ab94c57f4ada05199130494a326a1c665e9d38811a8d`  
		Last Modified: Wed, 11 May 2022 03:40:26 GMT  
		Size: 9.8 MB (9800318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e4fc355d43116148b88c95ecf294b953540521f03ba2ff14441034f5a10b6`  
		Last Modified: Wed, 11 May 2022 03:41:12 GMT  
		Size: 50.9 MB (50861425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc41e98cd28410a3e7f8c02632f783533e8863c3c4a7a65be309420c276522`  
		Last Modified: Wed, 11 May 2022 03:43:14 GMT  
		Size: 180.0 MB (180011027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ed25ce727115b4e611355b80a9ae80c65deaaf5f66cdcaac5a37ecbf76f096`  
		Last Modified: Thu, 12 May 2022 22:47:52 GMT  
		Size: 6.2 MB (6214323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf2895f00f33e0adca738037308832c1799be017dfc593e211133664373f0f`  
		Last Modified: Thu, 12 May 2022 22:48:02 GMT  
		Size: 20.4 MB (20395655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87879f2dab54c793c03c5d80da9a19e0a311b5a9e7acbaa68c7825d8d71db23`  
		Last Modified: Thu, 12 May 2022 22:47:47 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b81697ef52bb38938a72b0155e8a574bd930f398c0963a5792a5fc2ab2fcf`  
		Last Modified: Thu, 12 May 2022 22:47:50 GMT  
		Size: 2.9 MB (2871812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; ppc64le

```console
$ docker pull python@sha256:c66020f2f224aef4b8ffd3c1f47f73c097b4eab76c56f01d21e7a22cf9ce8f8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.9 MB (364932079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9b1b8f58ae2ee3d7b9d76f5ede2f150ce3ec1498a03e09da6645f47b09bf4f`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 01:32:53 GMT
ADD file:73ff2a18e50b226a862b74c50f091d80ddcd29f404879c4937887c560fdf624d in / 
# Wed, 11 May 2022 01:33:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:55:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:20:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 21:40:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 21:41:02 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 21:42:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 21:42:16 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 23:40:45 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 23:58:58 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 23:59:09 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 23:59:13 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 23:59:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 23:59:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 23:59:29 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Thu, 12 May 2022 00:00:10 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Thu, 12 May 2022 00:00:26 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:88d357d3afb8b0de721a4298ddb31fe73077663376e53d241a3d5217080e1f73`  
		Last Modified: Wed, 11 May 2022 01:43:32 GMT  
		Size: 54.2 MB (54170196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad446f507e97c97d9b6d29a8cd467c962ad6b7baa48356927e7afec937107eb`  
		Last Modified: Wed, 11 May 2022 03:49:39 GMT  
		Size: 8.3 MB (8293358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8784653a0c174d00c413056e723bd1a8692a8c27bfbe6508e37152d86bb395f4`  
		Last Modified: Wed, 11 May 2022 03:49:39 GMT  
		Size: 10.7 MB (10727832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8e974e0992db0fc98b88da2883b630af2407799183b4fe45d51e044b60ccf7`  
		Last Modified: Wed, 11 May 2022 03:50:04 GMT  
		Size: 57.5 MB (57458396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32fe3cc75c4624247cf639de03bd8d25c55a40ee6f9c3c999ec982a16043e11`  
		Last Modified: Wed, 11 May 2022 03:50:50 GMT  
		Size: 203.4 MB (203371891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649679d72d9b08e30465da30cad39f47171a755c3023473e4df645b6c0da46ae`  
		Last Modified: Thu, 12 May 2022 04:11:02 GMT  
		Size: 6.9 MB (6893681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf4fb92f181e9afab884894f314f14a3f7c7e46e90ea0bac8fd34cf3e641d93`  
		Last Modified: Thu, 12 May 2022 04:12:47 GMT  
		Size: 21.1 MB (21144135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d67f4c4f05e5d8d5fc0af3b728dca38aa22afbff817213f0c95f97ac8b2d0f`  
		Last Modified: Thu, 12 May 2022 04:12:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5027bc522049250760530641fef56226623f3ee98e83e0cb940e8e1b2f4ed9`  
		Last Modified: Thu, 12 May 2022 04:12:44 GMT  
		Size: 2.9 MB (2872357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:buster` - linux; s390x

```console
$ docker pull python@sha256:74cf32ad11ac14f9481fcd31fb4f58c99433ca81dd8e5753cd11fdcf6a9e3bc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.8 MB (323815249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a651905ca8817ee0391bf87e06a985ecd4d45b97d3a5070435d9668c22099e`
-	Default Command: `["python3"]`

```dockerfile
# Wed, 11 May 2022 00:44:30 GMT
ADD file:07d3aef2824f4da48dcf6a17e3ce265bea63e6140027ebee5f70b13eecd9a5fd in / 
# Wed, 11 May 2022 00:44:32 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:16:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:17:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:51:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 06:51:56 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 06:52:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libbluetooth-dev 		tk-dev 		uuid-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:52:01 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 11 May 2022 07:32:45 GMT
ENV PYTHON_VERSION=3.10.4
# Wed, 11 May 2022 07:40:54 GMT
RUN set -eux; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 	; 	make install; 		bin="$(readlink -ve /usr/local/bin/python3)"; 	dir="$(dirname "$bin")"; 	mkdir -p "/usr/share/gdb/auto-load/$dir"; 	cp -vL Tools/gdb/libpython.py "/usr/share/gdb/auto-load/$bin-gdb.py"; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		ldconfig; 		python3 --version
# Wed, 11 May 2022 07:40:55 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 11 May 2022 07:40:56 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 11 May 2022 07:40:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 11 May 2022 07:40:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/38e54e5de07c66e875c11a1ebbdb938854625dd8/public/get-pip.py
# Wed, 11 May 2022 07:40:56 GMT
ENV PYTHON_GET_PIP_SHA256=e235c437e5c7d7524fbce3880ca39b917a73dc565e0c813465b7a7a329bb279a
# Wed, 11 May 2022 07:41:01 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 11 May 2022 07:41:01 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:af98d4d7820a7b3b0a2afec4a171d8071d01877d1ce618b888a5a3c404ee8648`  
		Last Modified: Wed, 11 May 2022 00:50:25 GMT  
		Size: 49.0 MB (49000380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0761beea0e804b4a5a7dd37c5da5cffa31a45f325fe7c770cc1c3715ae3276`  
		Last Modified: Wed, 11 May 2022 01:25:43 GMT  
		Size: 7.4 MB (7423580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a570562b6ab9a24ab0bb1315e332237b14913dcc94de19fdf130826c8f5fb5a`  
		Last Modified: Wed, 11 May 2022 01:25:43 GMT  
		Size: 9.9 MB (9883171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d536289d3aa14d9486b1863430b9752f3884a4ed0dc74f4e73ce7355514e43d`  
		Last Modified: Wed, 11 May 2022 01:25:57 GMT  
		Size: 51.4 MB (51382023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d011b6ca25acd6dc401817177e6000cfe8ea9d25a715781c81a70150cbd61b0`  
		Last Modified: Wed, 11 May 2022 01:26:23 GMT  
		Size: 177.0 MB (176960767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fd0d0c7478019cd2659cd9f00362972c91ba17a0b0561d72b670d4f93b164d`  
		Last Modified: Wed, 11 May 2022 08:56:04 GMT  
		Size: 6.1 MB (6058668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2cffe80cbaae3376bb2e9e8b15869cc498c3de351ddd57401148fd54f059e8`  
		Last Modified: Wed, 11 May 2022 08:56:59 GMT  
		Size: 20.2 MB (20234091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e252975d0c7c54d86279f06d91bf00aefd3ae3b854fe95af28e52731732f97`  
		Last Modified: Wed, 11 May 2022 08:56:56 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3490bd6af7b85fdd24311fcdb732bd73189f60ca11f75a9f9a8a0f61187bc36`  
		Last Modified: Wed, 11 May 2022 08:56:56 GMT  
		Size: 2.9 MB (2872336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
