## `pypy:2-jessie`

```console
$ docker pull pypy@sha256:1c744532725f0b831ac691071bb675ea89e7837842dabdfe0160003c9a9bdd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `pypy:2-jessie` - linux; amd64

```console
$ docker pull pypy@sha256:8a25f32d099da879e52e251a60a3c0cc56a92769d5539b4e419dc3c75df2229e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282716542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efc90a235f1098321e7da6a3f5219325b7ac48e664d27938fb399fe78739e605`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:15 GMT
ADD file:00e3c0ca649cf82da02cd7fec7b3121205c2c54c4569209a2212c4924c73d5a9 in / 
# Tue, 31 Mar 2020 01:21:15 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:00:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 02:02:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:04:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:16:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 04:16:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 04:17:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:17:52 GMT
ENV PYPY_VERSION=7.3.0
# Tue, 31 Mar 2020 04:18:13 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f4950a54378ac637da2a6defa52d6ffed96af12fcd5d74e1182fb834883c9826' ;; 		arm64) pypyArch='aarch64'; sha256='a3dd8d5e2a656849fa344dce4679d854a19bc4a096a0cf62b46a1be127a5d56c' ;; 		i386) pypyArch='linux32'; sha256='eac1308b7d523003a5f6d20f58406d52ab14611bcec750122ae513a5a35110db' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		cd /usr/local/lib_pypy; 		pypy _ssl_build.py; 	fi; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 31 Mar 2020 04:18:13 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 04:18:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 04:18:14 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 04:18:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 04:18:27 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f27d6ed8cebc4be4a992767cb74cd433e5e145ae55c57e9e913e47d315b1dbdf`  
		Last Modified: Tue, 31 Mar 2020 01:26:56 GMT  
		Size: 54.4 MB (54389951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2886394fe026f40712d4f22ecfe40e26911d758627d04e684d9d5ff5637296`  
		Last Modified: Tue, 31 Mar 2020 02:10:58 GMT  
		Size: 17.5 MB (17545721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79486f9007497ffa7c18e154e42d395db78950bb662ad3788d208c2b7b9599`  
		Last Modified: Tue, 31 Mar 2020 02:11:11 GMT  
		Size: 43.3 MB (43333264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2071d428ba7a22c15ddc433fcb14a7bc30e7990695c11886519abb304c6b97b7`  
		Last Modified: Tue, 31 Mar 2020 02:11:35 GMT  
		Size: 131.9 MB (131895348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c52ae1e6cc070086b62318610341036a8512a77b6bb5baaea9c54f8b115a625`  
		Last Modified: Tue, 31 Mar 2020 04:30:58 GMT  
		Size: 3.2 MB (3168433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef3eb421c8c6506113f48b9f2364c6fcc9854d9bf2230fe3ae55b9cce2a863b`  
		Last Modified: Tue, 31 Mar 2020 04:31:05 GMT  
		Size: 30.5 MB (30495950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68555a2ab14beeb590b33df42a2aed8bcfc56157355fdf7900d8ad3e2c3274b`  
		Last Modified: Tue, 31 Mar 2020 04:30:57 GMT  
		Size: 1.9 MB (1887875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-jessie` - linux; 386

```console
$ docker pull pypy@sha256:4e40d678fdb9d7d520d9749fccd391f495545640c36b935e34f919d4c7da83ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.4 MB (287445425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890f36c5e1c7eac561758bbb42fa7a979c7adbd53e7c7bc12e011a1a613b50d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:59 GMT
ADD file:ee61b11b0132f3aa493c1fe2d59c8c7225e31b99c52f87f49a49512a80a203ae in / 
# Tue, 31 Mar 2020 00:39:59 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 01:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:22:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:04:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 02:04:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 02:06:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:06:40 GMT
ENV PYPY_VERSION=7.3.0
# Tue, 31 Mar 2020 02:06:57 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='f4950a54378ac637da2a6defa52d6ffed96af12fcd5d74e1182fb834883c9826' ;; 		arm64) pypyArch='aarch64'; sha256='a3dd8d5e2a656849fa344dce4679d854a19bc4a096a0cf62b46a1be127a5d56c' ;; 		i386) pypyArch='linux32'; sha256='eac1308b7d523003a5f6d20f58406d52ab14611bcec750122ae513a5a35110db' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2.7-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		cd /usr/local/lib_pypy; 		pypy _ssl_build.py; 	fi; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 31 Mar 2020 02:06:58 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 31 Mar 2020 02:06:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 31 Mar 2020 02:06:58 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 31 Mar 2020 02:07:11 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Mar 2020 02:07:11 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f263b30518dd64881c8ace989042a8efd1273a1175e0dc751ca62444e9f2ff81`  
		Last Modified: Tue, 31 Mar 2020 00:45:52 GMT  
		Size: 54.6 MB (54607453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f5a9dd559c3a0035cf2826e46fcddd2f78535e67543e52c97156d68f2b89b6`  
		Last Modified: Tue, 31 Mar 2020 01:30:29 GMT  
		Size: 19.9 MB (19855790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54e4a737961a715ee92034bb56cf77c442fa2e42a168bbdea4cdf47ae036de6`  
		Last Modified: Tue, 31 Mar 2020 01:30:46 GMT  
		Size: 44.0 MB (43976045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7728564dbb10e1d2b344529700b32e3d00bd06e7ab0eba73435a5c188448417f`  
		Last Modified: Tue, 31 Mar 2020 01:31:28 GMT  
		Size: 135.9 MB (135875385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337b60dc8f676e206045b284a2ae0aac95a47755ae0a81be3cd0a814cab6fe41`  
		Last Modified: Tue, 31 Mar 2020 02:22:08 GMT  
		Size: 3.3 MB (3272177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e4fb21b7fb431ac482ad2792e31d54519558c9ab25e2e1ac567380ed40cc2e`  
		Last Modified: Tue, 31 Mar 2020 02:22:17 GMT  
		Size: 28.0 MB (27970706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2f5403f3c75a9c5fbfc37a5c16c7acaf2423c6db1a4209cd351424a665556b`  
		Last Modified: Tue, 31 Mar 2020 02:22:08 GMT  
		Size: 1.9 MB (1887869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
