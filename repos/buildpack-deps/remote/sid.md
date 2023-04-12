## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:6fa31d2839b2176bb4d92e7cb1bf4f0acdac4ca440650d2d937bfd713779f3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1cb95d972e0a2c28195432ae6f0b584389e01e1938354a98b61c2d0e4c79f44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350981822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9133db89f5b5ae7caee0f8cca02226caaa3b22832a67d2a4bfc68f2ca38dfccf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:55:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108d0b8f8755100dc81501ff3e762f953171a4a1230223973781ad90f85c1a53`  
		Last Modified: Wed, 12 Apr 2023 08:00:14 GMT  
		Size: 216.9 MB (216931912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7c5689a7aafd87d157899f6caf4601d66e8e391aef6483970f37553b5a868314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.5 MB (318503660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:321ba3c06205c499df306cc1b5cfded148321e0a03dea6b3028714995c1f7d03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:19:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df42d9b3dd685881fab45c09a19f6d1505f1612856e8b0acca62c90e5aa6457`  
		Last Modified: Wed, 12 Apr 2023 01:23:20 GMT  
		Size: 189.1 MB (189138097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13bc1f7227e4eb190e2425e9ae9baaa9afa595247f7c48578dae477f5206c282
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.1 MB (299089852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82add4ff4f01d1f31c7d61d6b83e243c99fc38f0cb8fbe94fc118eaf5a75103`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:42:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:43:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e5e2259a7026a6a42309e4673ccd18c4288dce5b85e2039cb7238e36ce3fe`  
		Last Modified: Thu, 23 Mar 2023 12:46:22 GMT  
		Size: 59.4 MB (59373909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd2df18bf0523ee48067a579083ad967febe18f6eda98aa82f65c4fbb8ff974`  
		Last Modified: Thu, 23 Mar 2023 12:46:53 GMT  
		Size: 174.9 MB (174932032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ddc7753bdf44aa12263963bdb9942af3b69f4ed4dad7430d1a9eecabd6381d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.1 MB (342096356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e722281a223374a931912368ece55c74201c7f46e39795b84006341333ddb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f54a27824f720f86861a2776e1cc4e2f54563a9d0f0b56d1a6ec034866e3f8`  
		Last Modified: Wed, 12 Apr 2023 01:15:45 GMT  
		Size: 208.3 MB (208310077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:413efb8fbcbb35e21e9437afbee83ae1bdcf365d62cc1261952b77c46884fede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352984444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e361eb5030e9416d576bb6456af5b6f82090e0ffcde0ac62558e2c5fa198c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:13:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc32f4359c6fe3187a1f8bab45e405139e65a8f45a4858a27e1059dd58842672`  
		Last Modified: Wed, 12 Apr 2023 01:18:36 GMT  
		Size: 215.5 MB (215455324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3862aaeea79e1c28e659f99f4d362b54d636ab87938c521b7e6c32cd660f4359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321528438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d166a77be6f0012f9af9d61d3c7ad01ee0b80e1584627a75c08c07fee6b7e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:30:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cde7245b1c56e104d5370eab7caa185d690ab7a9d05dd04502c112995eedf9c`  
		Last Modified: Thu, 23 Mar 2023 07:39:55 GMT  
		Size: 189.5 MB (189526884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1cd92695e70eee806ffc668ffc3613c1ae37e09e9905ff84a9ad42e7353a4a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.8 MB (358843576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff6cf39c1a7a6027c3f5251567633ab1cfbf3af110fb104f2f31ece459b538e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5053cb00528479013fa5db3eb35bb36ff11628a7f8c9c6ae0310021f09a7005`  
		Last Modified: Thu, 23 Mar 2023 13:26:59 GMT  
		Size: 69.7 MB (69740333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb6e33785c280f1561e4dcdae27bfcb7e802b5b52d2ebf732730e9c11c4c717`  
		Last Modified: Thu, 23 Mar 2023 13:27:58 GMT  
		Size: 214.0 MB (213966262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b9c02baf674d938d6af39d2f681786407b07e39dcc6c0ef663bbfa3027bb41f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361040206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcff52053934b6b9001b1f614aafda9141bd8e31a4b2680e51f8d44353d4a4ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:43:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16f9d49dc3af209b4bcf7ce13172c2a5a76516c0d39580db79da7b27eaf387f`  
		Last Modified: Wed, 12 Apr 2023 00:50:51 GMT  
		Size: 236.9 MB (236892651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9287c8095d9220df2f988981ac641e97e22f861d9bd87aa2a19a9e6cf396a687
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (319011191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914264ef0379c6c6c2f67b9eb3fd0e99ffc0016a3f81cb006225180ad93d3a77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:29:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81adcc7796eb9dd6b2ccee5b41b08f31d903a15caab787b2edc99367e1c15497`  
		Last Modified: Wed, 12 Apr 2023 00:34:19 GMT  
		Size: 188.1 MB (188084029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
