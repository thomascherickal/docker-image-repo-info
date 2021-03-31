## `pypy:2-buster`

```console
$ docker pull pypy@sha256:1a0988a0e9bc4bf783a8435bf17f9e6d5d6b06e7e884c23be4f356b358baebd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-buster` - linux; amd64

```console
$ docker pull pypy@sha256:6ca09fdd960e0927041a31ce5112635aa1bb14e3c4aa30ec339f151dc1e4730f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.2 MB (350240356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19366199e53ac55ed80644723a3102c9190d14345c1bab0cae132f1ad011e4c`
-	Default Command: `["pypy"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:53:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 05:53:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:54:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 17:54:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 17:54:53 GMT
ENV LANG=C.UTF-8
# Sat, 27 Mar 2021 17:54:53 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 27 Mar 2021 17:54:53 GMT
ENV PYPY_VERSION=7.3.3
# Sat, 27 Mar 2021 17:57:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux64.tar.bz2'; 			sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-aarch64.tar.bz2'; 			sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux32.tar.bz2'; 			sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 27 Mar 2021 17:57:45 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 27 Mar 2021 17:57:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 27 Mar 2021 17:57:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 27 Mar 2021 17:57:55 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 27 Mar 2021 17:57:55 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c70e46d8b5f0e1d77797b7a0565b7a316bd8c7c024f5cca82592128af142dac`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 7.8 MB (7832558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea848ad42f0d1676b3a0ce709208ba3fa154cd53370c50e7cf8e580c63d96ae0`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 10.0 MB (9997159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fe137f8d2641315dd2f93c46dfdb671ce7399edc1f44f10cc68984f2809d8e`  
		Last Modified: Sat, 27 Mar 2021 06:04:05 GMT  
		Size: 51.8 MB (51839972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13f6ed9b0cab6a0e5a875bd6ecb04c0b0bc1cd98a1600fbaf5b2f49a4c7190`  
		Last Modified: Sat, 27 Mar 2021 06:05:00 GMT  
		Size: 192.3 MB (192343172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be727aa92d898b75c8a269e3513b6e9eee04df2de15e1f035e8a921a96013b8`  
		Last Modified: Sat, 27 Mar 2021 17:58:38 GMT  
		Size: 3.2 MB (3189178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64da3ab009844055dfb621d13bc330fa0b48145e10e89a9c0c13297f4a892a75`  
		Last Modified: Sat, 27 Mar 2021 17:58:44 GMT  
		Size: 32.7 MB (32670578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ec1123ea5a180045d16b764f152a026b386235bdacc77388efc00c9b1feca6`  
		Last Modified: Sat, 27 Mar 2021 17:58:38 GMT  
		Size: 2.0 MB (1967461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-buster` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:b9595f4ff311a41653d19b7324e4b616f4e562aae86f85d2b8673f3ef92e3ac5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333978701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50fc4c92733243a582b6c0b14670b1db962fe3e9eecc61db72dad292af1a5347`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:18:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:57:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:57:54 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 09:57:55 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 09:57:56 GMT
ENV PYPY_VERSION=7.3.3
# Wed, 31 Mar 2021 10:03:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux64.tar.bz2'; 			sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-aarch64.tar.bz2'; 			sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux32.tar.bz2'; 			sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 31 Mar 2021 10:03:53 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 31 Mar 2021 10:03:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 31 Mar 2021 10:03:55 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 31 Mar 2021 10:04:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 31 Mar 2021 10:04:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70c372ae296f23e908bf1e1ed9f4c0c81a8a6d7fc48c0e2db16035bb9b7a54`  
		Last Modified: Wed, 31 Mar 2021 00:30:24 GMT  
		Size: 52.2 MB (52165620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc089388c7ca4407aec7247a44601b896e57e96d53a858fb0e8c6f2f94ab8da`  
		Last Modified: Wed, 31 Mar 2021 00:31:19 GMT  
		Size: 183.9 MB (183900636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40acefb3e513f4c89a0bf52c9ea4625b27730761d86abc17a48649223240a81e`  
		Last Modified: Wed, 31 Mar 2021 10:06:21 GMT  
		Size: 3.2 MB (3196054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eeaaf95a9677928747774df7d3539b72fbc0789fc8c22ce920f364c3924f84`  
		Last Modified: Wed, 31 Mar 2021 10:06:31 GMT  
		Size: 25.8 MB (25844143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdbda599a7443ac30d9d9c5f7aaa09668e676ad3a8981d82bef7613505a0ec1`  
		Last Modified: Wed, 31 Mar 2021 10:06:21 GMT  
		Size: 2.0 MB (1967519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-buster` - linux; 386

```console
$ docker pull pypy@sha256:1fee0406cd318d3667e526e8e013df8b27d277cf216f9c70ddcbaee786dff114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.3 MB (357327893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a72741737ad6d63f9e58cd0192f0a101c1730eb8c1031abc6baba7e00f37787a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:30 GMT
ADD file:a2981af3d3aa369b11e802f23b175abfdb0f7636cdeec3aed67488d7a1f28a19 in / 
# Tue, 30 Mar 2021 21:39:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:56:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:58:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 07:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 07:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 07:59:17 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 07:59:17 GMT
ENV PYPY_VERSION=7.3.3
# Wed, 31 Mar 2021 08:04:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux64.tar.bz2'; 			sha256='f412b602ccd6912ddee0e7523e0e38f4b2c7a144449c2cad078cffbdb66fd7b1'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-aarch64.tar.bz2'; 			sha256='23b145b7cfbaeefb6ee76fc8216c83b652ab1daffac490558718edbbd60082d8'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.3-linux32.tar.bz2'; 			sha256='bfbc81874b137837a8ba8c517b97de29f5a336f7ec500c52f2bfdbd3580d1703'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 31 Mar 2021 08:04:23 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 31 Mar 2021 08:04:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 31 Mar 2021 08:04:23 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 31 Mar 2021 08:04:34 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 31 Mar 2021 08:04:34 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:a3a3dbaddd2d56d7418508211551c461f826d1cae349d39a355a1c22fe140b36`  
		Last Modified: Tue, 30 Mar 2021 21:46:05 GMT  
		Size: 51.2 MB (51198756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de970e2d41035ffe1a656cc3d1f8e17bc7b8539b23745405b8fccf25d10fd312`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 8.0 MB (7997659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27a2cf0e2e609cc89ee5b623626f822424bdc818ac5eab541a7a7b158ef0c01`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 10.3 MB (10340050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a5ef36d45f69154fe2b83a8e658d4f08c45428493e8e1cc74a8b03b3c4799`  
		Last Modified: Wed, 31 Mar 2021 00:08:31 GMT  
		Size: 53.4 MB (53438017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e4b62cf2ad846ba0bec17add38106ebdfbe771009574c1a033f9698ba80e36`  
		Last Modified: Wed, 31 Mar 2021 00:09:26 GMT  
		Size: 198.9 MB (198898090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4beecde3b6464ecdc496d7d1aba80aec687289086e4fa9881bdb774d80e02c0`  
		Last Modified: Wed, 31 Mar 2021 08:07:29 GMT  
		Size: 3.3 MB (3329325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92e2d75278766b65ab2adae73ac447f4f34afc7f1fc35fa3dd9855a0fb67da4`  
		Last Modified: Wed, 31 Mar 2021 08:07:38 GMT  
		Size: 30.2 MB (30158564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175501514d114c81e4b6805bd5dc1da58cfd12e8ba5c3311120d3b8e4c36430`  
		Last Modified: Wed, 31 Mar 2021 08:07:30 GMT  
		Size: 2.0 MB (1967432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
