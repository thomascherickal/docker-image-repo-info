## `python:3-buster`

```console
$ docker pull python@sha256:0fdf406aca07ba87d97bebe59573f80772e2cc7f8e90b4ad0a287028b67ae4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `python:3-buster` - linux; amd64

```console
$ docker pull python@sha256:76aace0349933165c34ae8f99b32d269103bc14818c1914b104c34521b92f288
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349196581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a3a95c81a2bd8d2ee9653097a4e0ae63d8765636874083afb5e9a7d52b6b9f1`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 05:27:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 05:27:44 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 05:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 05:27:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 23 Nov 2019 05:27:53 GMT
ENV PYTHON_VERSION=3.8.0
# Sat, 23 Nov 2019 05:38:30 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 23 Nov 2019 05:38:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 23 Nov 2019 05:38:32 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Sat, 23 Nov 2019 05:38:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Sat, 23 Nov 2019 05:38:33 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Sat, 23 Nov 2019 05:38:41 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 23 Nov 2019 05:38:42 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8659dae93050c1ac9ec02542a046e4b40109f6ee13d16472442de03dd15b792e`  
		Last Modified: Sat, 23 Nov 2019 07:46:07 GMT  
		Size: 5.8 MB (5792245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b57a0e98ffc2067920d65ca5d099bf6c24b93d6aeb118deeed8e76688751a7`  
		Last Modified: Sat, 23 Nov 2019 07:46:14 GMT  
		Size: 29.5 MB (29515324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d187245c5fc44b61e97b8e7a5db9ea7b875e600de412629d205b8a0ba7dfe37`  
		Last Modified: Sat, 23 Nov 2019 07:46:06 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd75e768c3f7fbc2213506bcc3bac8c77951175aa8d51255b4482ebe88cfe51d`  
		Last Modified: Sat, 23 Nov 2019 07:46:08 GMT  
		Size: 1.9 MB (1869709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; arm variant v5

```console
$ docker pull python@sha256:dfcbcd2dfb91298376ce2230ab8e5e003cf027bab5c7c313471cb70049e7e744
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320171708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c309746a9b37c45ecabc188094ab4e01ed93ded9f7016344860fd9ba32211386`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:23 GMT
ADD file:23b24e6b66abab81b6f02095b5a46f724972b126daa5a21c8a4212ebd3874469 in / 
# Fri, 22 Nov 2019 12:13:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 17:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 17:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 17:24:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 17:27:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 22:16:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 22:16:59 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 22:17:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 22:17:20 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 20 Dec 2019 21:14:05 GMT
ENV PYTHON_VERSION=3.8.1
# Fri, 20 Dec 2019 21:25:33 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 20 Dec 2019 21:25:35 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 20 Dec 2019 21:25:36 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 20 Dec 2019 21:25:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 20 Dec 2019 21:25:37 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 20 Dec 2019 21:25:56 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 20 Dec 2019 21:25:57 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:96156da8e12fc015ffbd186837e04c6c4e2dfe5494840348c48ae55f01c0542e`  
		Last Modified: Fri, 22 Nov 2019 12:21:53 GMT  
		Size: 48.1 MB (48092724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806d6fd28bc0410ad86d18a4e083e02ee35536140cc371e3cdd7c0c7cf362cef`  
		Last Modified: Fri, 22 Nov 2019 17:46:14 GMT  
		Size: 7.4 MB (7358489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751f24651de16e7bde026c4f4aefaf31be196ed92db3b2c81348c694693f213a`  
		Last Modified: Fri, 22 Nov 2019 17:46:14 GMT  
		Size: 9.7 MB (9686943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e004d78f003015c8e6ad1f62b7419b0ac5f28c4501cd153ebd898c7390a95`  
		Last Modified: Fri, 22 Nov 2019 17:46:40 GMT  
		Size: 49.5 MB (49525038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fcdd3dc072ec607aa4e1f587b5bafdf98981e3cb1c56264d3099b07808b3cf`  
		Last Modified: Fri, 22 Nov 2019 17:47:41 GMT  
		Size: 171.0 MB (171002346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d1bd6751dc982eb210e0397e2be2f8c79622e42cadea44fb66da31e8dc52f2`  
		Last Modified: Sat, 23 Nov 2019 01:15:17 GMT  
		Size: 5.5 MB (5490190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ebd9e4fd0c5391546bd7e2e4dcfd8b45ba100680690eff34e7ea2bcfb5807c`  
		Last Modified: Sat, 21 Dec 2019 00:34:45 GMT  
		Size: 27.1 MB (27145050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d09d2438e6940fc81ed1f37a1b6d193fe49da49d484f5576e2c4b687c516`  
		Last Modified: Sat, 21 Dec 2019 00:34:30 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0db78268d92c41ffdcf250f9ea11164acb880d6a8945fd4e01c7cd6db55559e`  
		Last Modified: Sat, 21 Dec 2019 00:34:30 GMT  
		Size: 1.9 MB (1870694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; arm variant v7

```console
$ docker pull python@sha256:cad069a590c55214baa1beec36516c7cea772442e394654458b98510dc340b0b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311645724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43a5ba6f3af12e9a82bd5cfe3a169430de1e3a6a34464bfe9987d8f0453dbb6`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:15 GMT
ADD file:4c51a92fbc511319241c84feac408f0040600ab2230fd8ef007c322f6a5b9532 in / 
# Fri, 22 Nov 2019 13:22:17 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:09:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 23:11:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:13:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:47:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 00:47:19 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 00:47:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:47:35 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 23 Nov 2019 00:47:35 GMT
ENV PYTHON_VERSION=3.8.0
# Sat, 23 Nov 2019 00:59:13 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 23 Nov 2019 00:59:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 23 Nov 2019 00:59:17 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Sat, 23 Nov 2019 00:59:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Sat, 23 Nov 2019 00:59:19 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Sat, 23 Nov 2019 00:59:31 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 23 Nov 2019 00:59:32 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:6bac76f7ec397955852a282870ca77ba8bc17beaebffc52bc9053aaa18afc45f`  
		Last Modified: Fri, 22 Nov 2019 13:33:01 GMT  
		Size: 45.9 MB (45859502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43968e81e0eda7d56c4e052a87cd68ef88c023cea38c51a9f30375292f9642d`  
		Last Modified: Fri, 22 Nov 2019 23:30:31 GMT  
		Size: 7.1 MB (7096035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecba33550822d3a153c6be10451c2d9e738070ee19367ec3136aee9875636ac`  
		Last Modified: Fri, 22 Nov 2019 23:30:31 GMT  
		Size: 9.3 MB (9343198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffc58cc3ec62e27b8234a554691e44c19d566effa798a9e88bf039d3958d5d6`  
		Last Modified: Fri, 22 Nov 2019 23:30:53 GMT  
		Size: 47.3 MB (47301080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a69590e0d6b359167e2d103e39617e28e2d5da74e7327194e72a2a0b4828107`  
		Last Modified: Fri, 22 Nov 2019 23:31:41 GMT  
		Size: 168.2 MB (168243234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c43046833dc87303eef175734beaf61a985a5e570bc0f920fa03a201f45c2`  
		Last Modified: Sat, 23 Nov 2019 04:21:53 GMT  
		Size: 5.2 MB (5196232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c08f485be984f84d1220afcc45f7f5e47db68c99ba646c47fcdbba19d773a4`  
		Last Modified: Sat, 23 Nov 2019 04:22:02 GMT  
		Size: 26.7 MB (26736270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a6c27eba0ad2be89339d8e73751efdcb72526d7dad093255e8f3b07e574ee0`  
		Last Modified: Sat, 23 Nov 2019 04:21:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eba9bc2a6caef11991be4ee58a7932bc2b6d34dcf5a2e2e28310c64bccf5d75`  
		Last Modified: Sat, 23 Nov 2019 04:21:53 GMT  
		Size: 1.9 MB (1869939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; arm64 variant v8

```console
$ docker pull python@sha256:a32098940b088a477518a0ea7174d32c69c7011cef2dd2862cd92319d8c2ac20
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.9 MB (338862243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b78fa2ffaa4fa39ae6428c74f7bdec7cc1d9599ae555505da7dd040dcf3c96d2`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:03:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 08:03:46 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 08:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:05:13 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 20 Dec 2019 20:58:45 GMT
ENV PYTHON_VERSION=3.8.1
# Fri, 20 Dec 2019 21:08:24 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 20 Dec 2019 21:08:27 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 20 Dec 2019 21:08:27 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 20 Dec 2019 21:08:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 20 Dec 2019 21:08:29 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 20 Dec 2019 21:08:41 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 20 Dec 2019 21:08:42 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1da11f97bb2014cee3adefc29d8eeab67c59e39e9f93239eabdc80885fb1e9`  
		Last Modified: Sat, 23 Nov 2019 11:55:11 GMT  
		Size: 5.9 MB (5909459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b05002aa816bb155ab5a4b2b9c6007d19be1df771cb2f1a1adf442dcfe0d35`  
		Last Modified: Sat, 21 Dec 2019 01:40:34 GMT  
		Size: 28.6 MB (28598397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80584c495f4e0f339efac09f622b7480490af8c4030bc22c15d42b4e220e7c67`  
		Last Modified: Sat, 21 Dec 2019 01:40:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ee9fba577341055f78d59b2ae17195224ab6aec38e50a23d786443fecd460f`  
		Last Modified: Sat, 21 Dec 2019 01:40:23 GMT  
		Size: 1.9 MB (1870724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; 386

```console
$ docker pull python@sha256:ea99aedbd84bfb0b58c62ec43ca3b0e5c109e87fb2db17134651c5bf793e68f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357094109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6927a9333fb4dfab6a7dcf356ccc8d8253ffa49f7ff6f1ab4ffcd98ac755e4`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 16:49:50 GMT
ADD file:637dd256233b11c890b47c64e1116a873db07060c542d65ed8c5e1f1692b93c5 in / 
# Fri, 22 Nov 2019 16:49:51 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:39:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:41:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:48:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 08:48:35 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 08:48:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:48:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 23 Nov 2019 08:48:49 GMT
ENV PYTHON_VERSION=3.8.0
# Sat, 23 Nov 2019 09:04:25 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 23 Nov 2019 09:04:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 23 Nov 2019 09:04:26 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Sat, 23 Nov 2019 09:04:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Sat, 23 Nov 2019 09:04:26 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Sat, 23 Nov 2019 09:04:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 23 Nov 2019 09:04:33 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:d34dc3661e80ce84b97704f402da563467559a0af488425969a76a38a8761a63`  
		Last Modified: Fri, 22 Nov 2019 16:58:09 GMT  
		Size: 51.1 MB (51141757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a002a28e7af0825b2efeca76651a2e3e98ba4d0ee10eed07b3d1495cc86a50`  
		Last Modified: Sat, 23 Nov 2019 01:01:39 GMT  
		Size: 8.0 MB (7981294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d521d3b916711e34309354077f7f65c55009c0845fcce1b34ec7de57e3d97435`  
		Last Modified: Sat, 23 Nov 2019 01:01:39 GMT  
		Size: 10.3 MB (10338436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a5cecf8b6e164d82cc59bf21e9316e3e5e98d21dab1a969d690c117d83ae2`  
		Last Modified: Sat, 23 Nov 2019 01:02:01 GMT  
		Size: 53.4 MB (53358180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d04d7f177748111a9f0984420d86be7db6e1583a9a71bf27b890d0034907e8c`  
		Last Modified: Sat, 23 Nov 2019 01:03:05 GMT  
		Size: 198.6 MB (198593521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234bfef9f740aa5b0b1e4071705bf47a9ff727aea2a8ae5547f71b75addfe6e7`  
		Last Modified: Sat, 23 Nov 2019 12:09:33 GMT  
		Size: 6.1 MB (6139184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e92d57503b11fc0c1d70dff9581c931c36fd1fe1bcfb9d8616b4db8d7d048`  
		Last Modified: Sat, 23 Nov 2019 12:09:40 GMT  
		Size: 27.7 MB (27671857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3283d366ab14d9b042d8dd36a19ceb85c1f55940d61bb0f401a959ecdde0be`  
		Last Modified: Sat, 23 Nov 2019 12:09:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0287808fdd55dd2fabbf2fe9e3f02eb6e8f5afe3727056c7aafcf9b2c61c5c6`  
		Last Modified: Sat, 23 Nov 2019 12:09:31 GMT  
		Size: 1.9 MB (1869646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; ppc64le

```console
$ docker pull python@sha256:ca4a6f2ee2ce7d622cd300827adb34fe49d6f71709e7999322805d15474b1148
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.0 MB (372033657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bf58faf5945f53705ce7d7889d65fe0a98488f76e3f434313563ba798585f1`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:52 GMT
ADD file:7ea1f6679a4179527d68a59a76ad469bf07b8ce30b1288b4b6437bba9982b896 in / 
# Fri, 22 Nov 2019 14:54:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:01:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:01:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:08:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:53:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 08:53:06 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 08:53:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 08:53:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 23 Nov 2019 08:53:49 GMT
ENV PYTHON_VERSION=3.8.0
# Sat, 23 Nov 2019 09:03:09 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 23 Nov 2019 09:03:18 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 23 Nov 2019 09:03:21 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Sat, 23 Nov 2019 09:03:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Sat, 23 Nov 2019 09:03:28 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Sat, 23 Nov 2019 09:03:48 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 23 Nov 2019 09:03:53 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:127c50d67aec36464937a4593797286304a844c7b8ca8263bbbdd8967229cf5a`  
		Last Modified: Fri, 22 Nov 2019 15:03:30 GMT  
		Size: 54.1 MB (54132225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f59bd6a64d30e2f2a4a62e9589199153ddb61c2f77cc445945b67cd56d87db`  
		Last Modified: Sat, 23 Nov 2019 00:26:54 GMT  
		Size: 8.3 MB (8252166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c8328c28b5029be40abe47ebb260b0dab06a48ca9afdbd9a04b1d91fe6480f`  
		Last Modified: Sat, 23 Nov 2019 00:26:53 GMT  
		Size: 10.7 MB (10727041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1a63bd0de74997185aa941953104c26c47babd2334ce4ebc507eefbd72b724`  
		Last Modified: Sat, 23 Nov 2019 00:27:38 GMT  
		Size: 57.4 MB (57400619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7f7cbd4299e83d6173d1cd36c3636a5dc569334823a99166f1a3eeea2e8302`  
		Last Modified: Sat, 23 Nov 2019 00:29:24 GMT  
		Size: 202.8 MB (202845331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdab507a591b99fa7825e6f3dcecb59e1a130a2c59e2105d2a9604b2c7ab178`  
		Last Modified: Sat, 23 Nov 2019 12:13:48 GMT  
		Size: 6.5 MB (6527543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2e5dd63930b6d7d297698c06a748532967838b33fc55eba675bdf6746cb87e`  
		Last Modified: Sat, 23 Nov 2019 12:14:00 GMT  
		Size: 30.3 MB (30278657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a324bc71acf075e39a2f4d6a2a852002d204c96ded501c4f57dea7e5b86b5e19`  
		Last Modified: Sat, 23 Nov 2019 12:13:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143e8a86ef058ee2132cb4e60527be04eee319a3a2b93e5300c17dd2f13d7a9`  
		Last Modified: Sat, 23 Nov 2019 12:13:47 GMT  
		Size: 1.9 MB (1869842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-buster` - linux; s390x

```console
$ docker pull python@sha256:048055ea163df722fff82ecfe6a360c345c18948980b5bdc45bd9dccca56ff86
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330951821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e52cb655f346deab791eafdbb3a36b7c0ee13a4b5f27a4ad2860c8b635dd9da`
-	Default Command: `["python3"]`

```dockerfile
# Fri, 22 Nov 2019 10:40:18 GMT
ADD file:72d4939c469faaa7a7e3a81ea946b8effcfef763585a28c0da719de4acc60c40 in / 
# Fri, 22 Nov 2019 10:40:19 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 11:27:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 11:27:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 11:27:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 11:29:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 16:07:28 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 16:07:29 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 16:07:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tk-dev 		uuid-dev 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 16:07:36 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 20 Dec 2019 20:54:47 GMT
ENV PYTHON_VERSION=3.8.1
# Fri, 20 Dec 2019 20:59:01 GMT
RUN set -ex 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 	&& make install 	&& ldconfig 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Fri, 20 Dec 2019 20:59:02 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 20 Dec 2019 20:59:02 GMT
ENV PYTHON_PIP_VERSION=19.3.1
# Fri, 20 Dec 2019 20:59:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py
# Fri, 20 Dec 2019 20:59:02 GMT
ENV PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee
# Fri, 20 Dec 2019 20:59:06 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 20 Dec 2019 20:59:06 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:8fdf0c9621bb3a044b28b3bea9f60b87248b8648961de4622d4a93da641f4950`  
		Last Modified: Fri, 22 Nov 2019 10:44:13 GMT  
		Size: 49.0 MB (48954550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec52e72b73f26a9f14f7ff349840b08041045d4e6594216d838e1257596d56ec`  
		Last Modified: Fri, 22 Nov 2019 11:36:39 GMT  
		Size: 7.4 MB (7380308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c00a95b68a3c0dcde68488ea0c573ea5820e7b0326c2740d9eeb1fdc6a16984`  
		Last Modified: Fri, 22 Nov 2019 11:36:39 GMT  
		Size: 9.9 MB (9880255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf76353462bec8e44bb5f54b6e7d087125c79ff62836b4d836919cdcd325e1b`  
		Last Modified: Fri, 22 Nov 2019 11:36:53 GMT  
		Size: 51.3 MB (51320300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994860555cb6d25865cdfe04d284bb1ab8f4935e705376a2c5275065c5438e09`  
		Last Modified: Fri, 22 Nov 2019 11:37:19 GMT  
		Size: 176.6 MB (176583881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61820025df096e9007aaaa75d76b0f84648aaffcd68633ec3c7d43e93fe5d5bf`  
		Last Modified: Fri, 22 Nov 2019 17:26:05 GMT  
		Size: 5.7 MB (5705038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84395c1f37ec6b015cd3bbbb5a5408883ae74934042998886017a6b0c7294642`  
		Last Modified: Sat, 21 Dec 2019 01:57:02 GMT  
		Size: 29.3 MB (29256910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1f4518d36b3fde3924201c913c332f848146d2e76398c491deaeb220914829`  
		Last Modified: Sat, 21 Dec 2019 01:56:56 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cac879f92473ba8a2c71bffbcde48106990572411f2e9d3b7e01daee3d24b9`  
		Last Modified: Sat, 21 Dec 2019 01:56:57 GMT  
		Size: 1.9 MB (1870346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
