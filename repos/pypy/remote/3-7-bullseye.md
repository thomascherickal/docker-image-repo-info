## `pypy:3-7-bullseye`

```console
$ docker pull pypy@sha256:496d7939a2cfde1cc8d6a8b85e51bf0bd69aa80992b9465e1454c1d03e251775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:3-7-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:e0d3b6ba36e65c2ed36b052fdb99d688756c86ccad925e841a47a0d944e6cc92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.4 MB (358357126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b4d981404e19236f913b1a465aba511aceacb5f3c6613351a24801edb8690a`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:33:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:33:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:34:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 15:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 15:55:45 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 15:55:45 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 15:55:45 GMT
ENV PYPY_VERSION=7.3.13
# Tue, 19 Dec 2023 15:56:04 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 19 Dec 2023 15:56:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 19 Dec 2023 15:56:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 19 Dec 2023 15:56:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 19 Dec 2023 15:56:14 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8988ac7a69cc18b80883227d1cddd6babff98a5fce88b591500f8727dd26ff0d`  
		Last Modified: Tue, 19 Dec 2023 04:42:17 GMT  
		Size: 15.8 MB (15764812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d278fc41a93b35689afe55f7bbeda81194c3ed9d7162d8adf2ed2af1e042ea`  
		Last Modified: Tue, 19 Dec 2023 04:42:32 GMT  
		Size: 54.6 MB (54595440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e04794082b8082ce8c158a02cb11d1d737d6c0cd1542062514b3e2a93f6c70`  
		Last Modified: Tue, 19 Dec 2023 04:43:04 GMT  
		Size: 196.9 MB (196880584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d9f2c1a5dce0f4979f3ff6f50c3a750a63cd8ccc552865e3617168a283b8b6`  
		Last Modified: Tue, 19 Dec 2023 16:03:43 GMT  
		Size: 3.2 MB (3211864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d6d1b2dc873155c0da350320c1c5c6c6e208f37f04cdb7af8825c23b58f861`  
		Last Modified: Tue, 19 Dec 2023 16:03:48 GMT  
		Size: 29.6 MB (29609749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4142b629d14b095e53393fe7517de298256667c5e720006413dcc427276bb9ed`  
		Last Modified: Tue, 19 Dec 2023 16:03:43 GMT  
		Size: 3.2 MB (3237337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:ff9588623a4e8cbe2de17f2b7d701c88c896c977b4e8e97f53abf4e2fd396dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.3 MB (348339264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668ce790a4427d77975912fc4d7e236ba84e265084e6f5fb112eb0b1f9d6444e`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:35:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:35:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:36:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 16:11:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 16:11:18 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 16:11:18 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 16:11:18 GMT
ENV PYPY_VERSION=7.3.13
# Tue, 19 Dec 2023 16:11:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 19 Dec 2023 16:11:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 19 Dec 2023 16:11:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 19 Dec 2023 16:11:44 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 19 Dec 2023 16:11:44 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010797996cc86cf2cf7495aebc22e5be7d18a10bde1e11562dbe5283c226c0e9`  
		Last Modified: Tue, 19 Dec 2023 11:43:17 GMT  
		Size: 15.8 MB (15750308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70092c2a6b382a0cc0bd2adeb187b94d74c8bcf2ceb6f33bb8e4e4e9c6561141`  
		Last Modified: Tue, 19 Dec 2023 11:43:31 GMT  
		Size: 54.7 MB (54699871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc4a505c38c38e8d9b219e6c3ed4fc061369233b452cca74b29876a248cfea2`  
		Last Modified: Tue, 19 Dec 2023 11:43:56 GMT  
		Size: 189.8 MB (189799678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0729ec742e2d07c0f9185f92debc3580535e01fd1f5bc72bd68a7cfca9c32c19`  
		Last Modified: Tue, 19 Dec 2023 16:14:52 GMT  
		Size: 3.2 MB (3215581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8ca1fa0fd069f3b8d174366690a38f334af1ebe3755b0f0a5f27463a3dccba`  
		Last Modified: Tue, 19 Dec 2023 16:14:56 GMT  
		Size: 27.9 MB (27928511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6760d4d3f5c4a6c72b013e9662cab148f4f82055cccdc425a59b5843fc82325`  
		Last Modified: Tue, 19 Dec 2023 16:14:52 GMT  
		Size: 3.2 MB (3237224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:1e077ff3f09d505e10facdc8b4ee7073db0fe17f9331431c47680dcc42db7aa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360678551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309d20ce042c0f1170a03ed2519333ec0ed925167712b2650ce81e8a66ad2f88`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:26:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:27:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:28:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 23:47:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 23:47:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 23:47:42 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 23:47:42 GMT
ENV PYPY_VERSION=7.3.13
# Tue, 19 Dec 2023 23:48:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 19 Dec 2023 23:48:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 19 Dec 2023 23:48:08 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 19 Dec 2023 23:48:20 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 19 Dec 2023 23:48:20 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386e6c873ad0aec679cfb967e1449dc2223a2543dd9923e9491c8d4dfe25ff9`  
		Last Modified: Tue, 19 Dec 2023 03:37:37 GMT  
		Size: 16.3 MB (16268921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a344c33a496f0c80e861246ac1b15db106b888d28c7bb89d17b87d06a5f1abc`  
		Last Modified: Tue, 19 Dec 2023 03:37:57 GMT  
		Size: 55.9 MB (55937182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb89bdf92d460c8b83c3effc827149c832709e4d9e4e2262456e267a2e4decf`  
		Last Modified: Tue, 19 Dec 2023 03:38:42 GMT  
		Size: 199.8 MB (199796881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3cec183b43c8a3d5f8282fa32ffff91813b0f9b4596d842eef3ec5604b0a83`  
		Last Modified: Tue, 19 Dec 2023 23:57:11 GMT  
		Size: 3.4 MB (3361663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b9f2ec9795fce24a8fbf299d259bb7c2cf364db596ab4c44e271ba82bd590e`  
		Last Modified: Tue, 19 Dec 2023 23:57:17 GMT  
		Size: 26.0 MB (26030335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f67cf3547c562c956551dbd7bf28a6d8e872a471c748023b6fab0ae05bf668`  
		Last Modified: Tue, 19 Dec 2023 23:57:11 GMT  
		Size: 3.2 MB (3237233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
