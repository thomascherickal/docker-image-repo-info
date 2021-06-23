## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:4f950618b68175c17b26ec17bb867297fad79a129272ecdddbde0d1c0c8abc11
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

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1c7ae77d3064710dd7fbddc0e19bbd0ab754e15b5f7ab56c02fc02c41bd0f480
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312501150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c9e1ff4e82bbd1e727b1b9a3e606426b93ee35558d9b1ba1ffdf9857a4434a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:53:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:54:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd09c11b021b756b7a92a4f70a3d444ce7e63a1c24e5749d236dc2c6e68514`  
		Last Modified: Wed, 23 Jun 2021 01:02:12 GMT  
		Size: 51.8 MB (51841560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14feb89c4a52c44f0a7e23a46ebb76e1c25c4b2915a39656a3ab634c74bcda46`  
		Last Modified: Wed, 23 Jun 2021 01:02:56 GMT  
		Size: 192.4 MB (192393721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e374f012609d7a8fe6a9cc31821b24d6ed3ed8c52e484966bf1a496000aa00b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286093359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e105fc7e11bf1a80104b65e2063ab9561feb1d2fa7c7f5c06343b102ae7475`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:54:57 GMT
ADD file:443be99157e29a4ccb29f5d0ffc9994ce41fb51c512815f76fec9e1fb4d5d8ba in / 
# Wed, 12 May 2021 00:55:00 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:52:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:52:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 19:53:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:54:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db69af0c9ce605b61ac30d118d6c6ab4f8579b8c80e5469335f2108afa5d2c66`  
		Last Modified: Wed, 12 May 2021 01:09:52 GMT  
		Size: 48.2 MB (48150747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404ba73f5eb1dbb487e50a5cd752625acb36ffba758e241579e2cb88c3becaac`  
		Last Modified: Thu, 27 May 2021 20:04:54 GMT  
		Size: 7.4 MB (7376519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d6b363679cfa0fcdf5dc9c8564dd9eb369d8d776652cb414b2b23d621ae51`  
		Last Modified: Thu, 27 May 2021 20:04:54 GMT  
		Size: 9.7 MB (9687524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fed7877fa156e7f1cc5cf959724daf2f0db0041371f88494647de4950b987f`  
		Last Modified: Thu, 27 May 2021 20:05:29 GMT  
		Size: 49.6 MB (49575033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badcf08fa154bdb7a325e5f7442706ce7f5578dc21430927abb531223f80f97d`  
		Last Modified: Thu, 27 May 2021 20:06:30 GMT  
		Size: 171.3 MB (171303536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dc0efd75dbf4217b3ee19dd45f841cc2c157623f361cb3cab9b2a74b51d0d04e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278309527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd532b304f6e4c5f08fc53c160de68231af884137539b8eedf064afc5809bb23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:02:10 GMT
ADD file:51a0472692adf18117444dc1f35d6eb3b4d6d672f28a7f6631f9d5d269b0b85d in / 
# Wed, 12 May 2021 01:02:15 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:40:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:42:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89475607b1df9fc7eec7efe2fa845738a16cee3e92c1bb864c1f5a93b8303bc6`  
		Last Modified: Wed, 12 May 2021 01:18:49 GMT  
		Size: 45.9 MB (45916922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88447de5eb3eca4a1d96b6980b44d82ac19d121f6b77b826989f8d611fd001b0`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 7.1 MB (7124249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25b14665fd0185f2f3b90a8d1825fc8ef9f330e1aea452f60fd70cdcfe99bf4`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 9.3 MB (9343721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba65a331625e51ba8f0e1af07dcb97c0583204dda094b5da79672fdf554129c4`  
		Last Modified: Thu, 27 May 2021 01:03:40 GMT  
		Size: 47.4 MB (47356403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ccefa3ae1f76cf09b3c36f8db24962372acba8b951ea5ec9a55a0ef62b6676`  
		Last Modified: Thu, 27 May 2021 01:04:38 GMT  
		Size: 168.6 MB (168568232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f19459a6d1122c22b699d94ee856d5e4be3119367323a15622e991b0802890b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303040753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdc8918ab44c80a36228ef54651d63d0646e2dd578794ab61412a607bc8f0be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:25:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785171b903c4d81c5b7539417a7b05f4a9bc6a35840595233bf4e369d8aee387`  
		Last Modified: Wed, 23 Jun 2021 00:33:41 GMT  
		Size: 52.2 MB (52165169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0373cebfde2cc9a301ad49bdd4883de5ab6dd6d5416932aa96428f70fac5000c`  
		Last Modified: Wed, 23 Jun 2021 00:34:23 GMT  
		Size: 184.0 MB (183974602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a07c70221e429b065899b6f1b437baf0fc4c682baa9c15466c99f428ab2b0af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321915379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770486e83c72acb13995bfcb63e0f160b1c8646ffa6dfa969e8ce906f83903c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:18 GMT
ADD file:e69bc1dee51190c812075d4b4e8ba1e67f67250af9f2ddbaecaf2c9316a07bbd in / 
# Tue, 22 Jun 2021 23:39:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:09:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:10:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4109247a8f9a72ed1435270480f72d6db8d6f038c6941d86a94f4dd0be8f789`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 51.2 MB (51207098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823a83541e8a9ed59943f9915ac65a73f57137e829772a16bc0bca5031a8cc07`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 8.0 MB (7998521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7455379cfe2e69e9290d3b103e5889bee3e1c03187bb9e2a454325fd6a7f1a`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 10.3 MB (10339805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295349fcd02216e45784e329283de2e5811af98fafed9195ab2cf24bf58febe2`  
		Last Modified: Wed, 23 Jun 2021 00:18:25 GMT  
		Size: 53.4 MB (53436615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15859f8c06830467d6c8e426b5b5e10d0c53a2a8a7cfb7899e7ef81badfd7ce`  
		Last Modified: Wed, 23 Jun 2021 00:19:13 GMT  
		Size: 198.9 MB (198933340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0412342a1356b2d86a49cf7cef3bf464d75799344878d4f8baee3e38f465b4c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297104046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787946750543fd3c737c153d659bbeb5be1753f020cc57de71b172aa229df955`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:06 GMT
ADD file:4673ab387e5a746227250295a00343ac2d03d6aafdc28d019a9bdf26bb97c8c8 in / 
# Wed, 23 Jun 2021 00:09:07 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:42:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:42:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:45:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3f0127f2925aa298e3074daa756fb98cf945e5aa11c7dd3cb6d66cc3ba2c7ac`  
		Last Modified: Wed, 23 Jun 2021 00:15:06 GMT  
		Size: 49.1 MB (49080336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92573df8c3dcb8e821060f2830e027ebc52f7da05600cbb49cfdbb39aedcce5e`  
		Last Modified: Wed, 23 Jun 2021 00:53:52 GMT  
		Size: 7.3 MB (7252466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f80da49549480363cca077bae713c30796f17d3a33620cdfca3a75e0cd160`  
		Last Modified: Wed, 23 Jun 2021 00:53:53 GMT  
		Size: 10.0 MB (10016316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c2138b0b86fd417cc80da35fb6cccb87f7266d2be62853e3611c28a601c32`  
		Last Modified: Wed, 23 Jun 2021 00:54:42 GMT  
		Size: 50.8 MB (50844925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5987a53a9ba28c1218b01fc01df73c7e29278cd3937528e936efeeeb1ca2aa`  
		Last Modified: Wed, 23 Jun 2021 00:56:53 GMT  
		Size: 179.9 MB (179910003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93a4c98c8d88580209f03018ffd2b0ae6f5177cb067abfad670bf4b361011c7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333828785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6ab80ae39ea382247ea01c522b1d015aa944fbf495972e3a0166d503be588b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:34:15 GMT
ADD file:b714397b44737108500b0256abc9750626cfa28cc0bb52623b9a14bb0e2345fc in / 
# Wed, 12 May 2021 01:34:24 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 03:42:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 04:01:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd4ac1330adf594df6c60d33ec5060c79833a8455e6cdb9f5ef2be33cb843845`  
		Last Modified: Wed, 12 May 2021 01:43:19 GMT  
		Size: 54.2 MB (54180124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb8ec8ba72b4c906c6a3b88324130a605cfda687a94ed75e901c7cd141492fb`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 8.3 MB (8271865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46415d7d07194b30fe4845342dd9c5927deb73698c2cfe9a55c6417b98ed3855`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 10.7 MB (10727703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443c274997562dde0054a5cc26e8bbee59190c34ea8b862e917569cfbee85b63`  
		Last Modified: Wed, 12 May 2021 04:20:12 GMT  
		Size: 57.5 MB (57457050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b65c38ce026ad58ab9cdea9319693b6decc25f2f6d5820c42060874468f40`  
		Last Modified: Wed, 12 May 2021 04:22:06 GMT  
		Size: 203.2 MB (203192043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bc23ee5f96170d6ae9d8ab3b6f846f9160148b6fadde7e924fcfbe3056cfb99d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294547576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712e52ea6dad67f2056b08f1a2d681fe566e2e830d92d800877b720913b07c68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:13 GMT
ADD file:b935574081a3fbceb534880a35e5245e10c52a3b9d70224811e221b4c6254cfe in / 
# Tue, 22 Jun 2021 23:42:16 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:06:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b8d113de06cefaa0768df3e10da0c3b8272e15922e18ea75b0bb4dee23b551d`  
		Last Modified: Tue, 22 Jun 2021 23:45:28 GMT  
		Size: 49.0 MB (49003924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de1b6d51a91a64482d6eabf778b8c4e433f7dc198440476d01d0dbb31aee4fe`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 7.4 MB (7400480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64019084b252c52592ff8cab3bf20be9bab2801ea36e88025071f901f1cb38e`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 9.9 MB (9882902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481cb3d9acd652b3fd56e606ff28a1bb48aa89be3365577a33d2cd35c908d867`  
		Last Modified: Wed, 23 Jun 2021 00:12:24 GMT  
		Size: 51.4 MB (51380256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1743770944cccb82c795de20a9395efe75855871d9d8f58a7e3bf8eaef915cd7`  
		Last Modified: Wed, 23 Jun 2021 00:12:52 GMT  
		Size: 176.9 MB (176880014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
