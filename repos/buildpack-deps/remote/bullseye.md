## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:70ed158e021856737cfe2ca05a8edd4728f6c661a21a8b9b80b8dbcaa7b29f76
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

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:13c0fb2e1647f7e8915eeb6383bb81b3796f32cb21175490a8de341e7a636eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.8 MB (320777758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdd575905bc767f659be3f09f727a37d4db22df9e3c6d7bf18efcce77a584ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:09 GMT
ADD file:695398a9e249223d1e07b12d735ae1a0ce3d645d0fd4cf1478400a985311f1cc in / 
# Tue, 09 Feb 2021 02:20:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:33:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:34:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6f7b6573b5973ff98ec7b4368f16ac39a85fa4fa49a414c58d0a9a012d37354`  
		Last Modified: Tue, 09 Feb 2021 02:25:52 GMT  
		Size: 54.8 MB (54757786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e06a77fb30b0ab01ed40c4454b51ebc1989110fd455036a95486c37328845d`  
		Last Modified: Tue, 09 Feb 2021 04:44:39 GMT  
		Size: 5.1 MB (5143859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423fe70e1db2a70eb1116ca8f81653348710538e8027421da14d99331de5cc9b`  
		Last Modified: Tue, 09 Feb 2021 04:44:39 GMT  
		Size: 10.6 MB (10642715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f359fb7565f24ff7d3550e209a1c78200845886b937ec87f656d52a9e9c102e7`  
		Last Modified: Tue, 09 Feb 2021 04:45:00 GMT  
		Size: 54.1 MB (54146699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20eb577dfe607546a14c45a824371b3710d9a5ec9e28e5c1695c042f23289d4`  
		Last Modified: Tue, 09 Feb 2021 04:45:52 GMT  
		Size: 196.1 MB (196086699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:80a2ed6761363b1c5c0aee45f1b870ddc1da58f49019c6b7193848a2495334ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293888259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e0c41e7a14c8ce5934e752d82bbe138d069e1faead05181bc916738845341f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:49:05 GMT
ADD file:e692f14c1c4483cbc88d3f2b2b98df48a5589bdf417d84c2dd9dbb7388ad079b in / 
# Tue, 09 Feb 2021 02:49:07 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:22:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:24:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da2c3be8f08cfd7ddd509966bb4655b1f7c74b4eaa31a7ab733c50e91684f29c`  
		Last Modified: Tue, 09 Feb 2021 02:58:02 GMT  
		Size: 52.3 MB (52282753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9638f6c6794cf8abb357179d6515914ce152a277d089f8baec5e2553acf260`  
		Last Modified: Tue, 09 Feb 2021 03:38:28 GMT  
		Size: 5.1 MB (5054036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9f24461ae5121b4bee6d238f5d67ac3f026a1264614cf4428418453a0cfb5a`  
		Last Modified: Tue, 09 Feb 2021 03:38:30 GMT  
		Size: 10.3 MB (10327727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6aac75072d35d2f69c3a2b1aa298ffe4ac70c699a9eb8f183438eef5768f883`  
		Last Modified: Tue, 09 Feb 2021 03:38:55 GMT  
		Size: 51.9 MB (51892242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0bff821de1d37bfc64afe8b5d9c1912085d06b93a22d3ffddb0b33800b4cf`  
		Last Modified: Tue, 09 Feb 2021 03:40:04 GMT  
		Size: 174.3 MB (174331501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:00208a87d1a0fe4b83c091836f46b6ff00121c66da596d682c241cb04cdf7a98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281333004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f6ed1a96897a1df06840d4e6209932b0b0be76cec2de0d00945d8dd6ea201`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:59:45 GMT
ADD file:dbec72322674e09aeb852498a932b1b1be67734644d9efa41f70930b49e956ea in / 
# Tue, 09 Feb 2021 02:59:48 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:22:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:25:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ffa24fa47fc6ecfac0851b7ffbee3dc36b7d721e5a4d08285c3577bfe04c31a1`  
		Last Modified: Tue, 09 Feb 2021 03:08:35 GMT  
		Size: 49.9 MB (49936256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95997d63d97278978549401c96f2fa498f1420591bf0a8fc3bace484b2250bb2`  
		Last Modified: Tue, 09 Feb 2021 04:38:08 GMT  
		Size: 4.9 MB (4914496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001ea97578ff6bb0c099fa0742f2ed56527bfbc1c389ff125d63e64a5aa83f`  
		Last Modified: Tue, 09 Feb 2021 04:38:09 GMT  
		Size: 10.0 MB (9968574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afadaec42633be00a9a4693b59384a6827e4289d090f63d4cb7204302049649`  
		Last Modified: Tue, 09 Feb 2021 04:38:35 GMT  
		Size: 49.9 MB (49914243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4c5b827f02699f710398812b264942ac35a4d21b7d5b05fb25e70d03925fcd`  
		Last Modified: Tue, 09 Feb 2021 04:39:27 GMT  
		Size: 166.6 MB (166599435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:db6ff9c11181bf9918cab52635ced5722153aef29b791cbddf866b6b1b7d06a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312434492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae048f9385682033595a242a8dd2c5a4b2b03fe593eaf45d3506a9a48286bff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:06 GMT
ADD file:33be07279470bfff8a3572cfc0847b56f8230b343043052761953a9c6a60acf0 in / 
# Tue, 09 Feb 2021 02:40:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:40:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:40:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:41:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4a012a5760f92ca41c31246ef8e4d918873156a81f765b0a7c5d840e0f5704b6`  
		Last Modified: Tue, 09 Feb 2021 02:46:23 GMT  
		Size: 53.4 MB (53428538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79d28ddd44a525843a64c4a38bd53e21517f7cea2429e5566c98fe63eca0100`  
		Last Modified: Tue, 09 Feb 2021 04:55:58 GMT  
		Size: 5.1 MB (5132214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b66026d3757ddaa2f953691aee45d95fad0e392e5f27c9030a7a327ff1972`  
		Last Modified: Tue, 09 Feb 2021 04:55:59 GMT  
		Size: 10.6 MB (10647722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c92b5698b826bfb29a287cdf4912ab499906cb679c536a5b91b31830a65a45`  
		Last Modified: Tue, 09 Feb 2021 04:56:23 GMT  
		Size: 54.2 MB (54248869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba30c1fb47743627149633be96c819837e9b5da1ff4917569b66f7730658cb29`  
		Last Modified: Tue, 09 Feb 2021 04:57:13 GMT  
		Size: 189.0 MB (188977149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f71915e4faec8d533558a400f27602cae94a2071595f8f1ac0ecfcad74ded07e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.5 MB (326537598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e327691d140693a7611d0ecb4d2f4ade945af71fa86eb9913618fcd5500a001c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:01 GMT
ADD file:f81099d47b3f99bd08895e4a96fb89eec618d9d0e6c9c8b2fb34681259f340d5 in / 
# Tue, 09 Feb 2021 02:39:02 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:07:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:09:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e734eb27dd94c1f3c88a6f32899a659ba2861df7282687c7b9c90f8df744b794`  
		Last Modified: Tue, 09 Feb 2021 02:44:51 GMT  
		Size: 55.7 MB (55737065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e825922dd50d020f9bf23f62b411455511e3368cce25b3304525c231209ec605`  
		Last Modified: Tue, 09 Feb 2021 03:18:46 GMT  
		Size: 5.3 MB (5271393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c92fbb51c2a913e1648e9cfa5323f95e95123462fef6d2370963c8b8c23052`  
		Last Modified: Tue, 09 Feb 2021 03:18:47 GMT  
		Size: 11.0 MB (11024699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c4482327d66e8eab5dfb6951b0eb3805b9c6c836f78d1c355dbf8329e845c`  
		Last Modified: Tue, 09 Feb 2021 03:19:11 GMT  
		Size: 55.5 MB (55486247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabe6ac42f81045f3421bae4b1a37ea7b193cf2eb28ae8dda1dcc2b37c3822b2`  
		Last Modified: Tue, 09 Feb 2021 03:20:26 GMT  
		Size: 199.0 MB (199018194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d57f89b1003ba8753a17b3a268ede1513f096f2a6e8950d2c404c7ab553cde57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299768288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fae579de94a8ab76ad464d348be934a5a066e1878c5869ad44651ebd242044`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:08:17 GMT
ADD file:7f68924af238bc101419c6fcd9a321aa3ff88b6234d508100e66c9234756eafa in / 
# Tue, 09 Feb 2021 03:08:18 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:00:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:00:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:01:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:04:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cf1c8f9242008a01fc5567967aa7bfb87bd9f5dfbbd4f4b296fc463a02ee18f`  
		Last Modified: Tue, 09 Feb 2021 03:13:48 GMT  
		Size: 53.0 MB (53004321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaa6f5a332631981e084265abaccebb0a60c433eb0544f48b4c9a36acd40c1`  
		Last Modified: Tue, 09 Feb 2021 04:13:19 GMT  
		Size: 5.1 MB (5107186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a371ec00a3dddda57cd21f3bf82cdceb3fcb8f04ef78924a1357172ec6fd0dc`  
		Last Modified: Tue, 09 Feb 2021 04:13:22 GMT  
		Size: 10.7 MB (10651726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbf907fe8af3f07949f495a086e9156683e57668cb9a568985259d5576da5cb`  
		Last Modified: Tue, 09 Feb 2021 04:14:12 GMT  
		Size: 52.9 MB (52867122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8c2a712bf216a0d12206484f0561515b05ee55fb2e8fedbf92966c3564ad7`  
		Last Modified: Tue, 09 Feb 2021 04:16:21 GMT  
		Size: 178.1 MB (178137933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0549af4dbd8b7be8c2dfec161e8fe9c99ac33566c2959ce7a0ae7f249004db3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338109806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01b9b6f26e528c702ea931c7de96a9003bb9fe19ca2dd1dcae5083bec129ccc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:23:03 GMT
ADD file:840490bff9a0b2cb1e20599d893c1160f6884327f51294479567e5d43f91b885 in / 
# Tue, 12 Jan 2021 00:23:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:39:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:58:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d21ce86f5496c36ba2ba289acb977a3b160c6c56fb257c10e3adb8b55164a16`  
		Last Modified: Tue, 12 Jan 2021 00:32:24 GMT  
		Size: 57.6 MB (57562164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42b61558772eb59064c0ebad8029e0e7524bf865c29218b048871cd3e43fe7`  
		Last Modified: Tue, 12 Jan 2021 02:37:14 GMT  
		Size: 8.4 MB (8431230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663cfe2e2cfc28477e509f0e7aaffd4159d2f37157b32a7327bb6f43a7508ac4`  
		Last Modified: Tue, 12 Jan 2021 02:37:17 GMT  
		Size: 11.4 MB (11421868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe449d18af822c075f40a6ecd99422667906a91875941e650eb90b9743412ec4`  
		Last Modified: Tue, 12 Jan 2021 02:37:47 GMT  
		Size: 58.1 MB (58136248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210b3449c8291088f7275f584257b0d05753e64c6666b2b09ff58782b600765c`  
		Last Modified: Tue, 12 Jan 2021 02:38:43 GMT  
		Size: 202.6 MB (202558296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a7d81595706d4b970a7df165c8df2ff76e9161e4552f186b448f8932cbc2b86e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294369628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dd0760df66077540635cf1e2b33ebc55ab4bf67e409c2c079a3d0db582e99db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:32 GMT
ADD file:b29f05e744766860cbed836c9527b8ec4e72570959bb61a8aa0e5c363cb72484 in / 
# Tue, 09 Feb 2021 02:41:35 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:03:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:03:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:05:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6eee01c120872bf1700180eee1b04681a66f946d188f352a1a7d516d703e4a66`  
		Last Modified: Tue, 09 Feb 2021 02:44:42 GMT  
		Size: 53.0 MB (53006960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d2f6f124d0127ebcdbee7e40a00127640a914d79503aaef238ab4afe12cf36`  
		Last Modified: Tue, 09 Feb 2021 03:10:53 GMT  
		Size: 5.1 MB (5127719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3216ed6227ef8df582c34143415b588c1ed64bb3ed322108f9c67d4318a5e6b2`  
		Last Modified: Tue, 09 Feb 2021 03:10:54 GMT  
		Size: 10.5 MB (10518230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e263653485abd2123ff66f14705a1f6615493469f7da9d65bf82943eb579425`  
		Last Modified: Tue, 09 Feb 2021 03:11:11 GMT  
		Size: 53.6 MB (53616922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2d900d6218452c0196a69efde97f81f02f6e3144272edacc2c70d18d735cf2`  
		Last Modified: Tue, 09 Feb 2021 03:11:39 GMT  
		Size: 172.1 MB (172099797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
