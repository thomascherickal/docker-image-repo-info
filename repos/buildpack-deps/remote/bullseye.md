## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:5565ae130e14c82151d8c1ec3b31a0848879544ca2dde8f0f8e4e2b827751dd4
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
$ docker pull buildpack-deps@sha256:8c71d9a1b9020ca09bf698d458dd1d3de3400d1ea4e0ca9c8b31950f758c979d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321813079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579a4c24651f95aae08d05ee22f0a5410b06404bef0f5638f3f30be59f1dfede`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:48:53 GMT
ADD file:32519b03930d9f5db9010ae49e0987322ce19eab681ad5c841fe1cd6268ad2ee in / 
# Tue, 30 Mar 2021 21:48:53 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:00:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:01:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:02:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6abc78d8e2422868f293b265b6c0ec3ba250fc4987f862ba05e86d7eb277f297`  
		Last Modified: Tue, 30 Mar 2021 21:52:53 GMT  
		Size: 54.9 MB (54868089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1424cff1d2b47e24acbeb3381319a9bbefd1f8dcae5c521f0198833d9b2911ec`  
		Last Modified: Tue, 30 Mar 2021 23:12:47 GMT  
		Size: 5.2 MB (5151423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859f37c645b9a1a4967007d3e310ace7f83d9924b7fd77385ff9e2de20a55a5a`  
		Last Modified: Tue, 30 Mar 2021 23:12:48 GMT  
		Size: 10.9 MB (10867143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1dad4b787cfa0293818e7bb90048de585a8c37b12fab90dc184d527078652`  
		Last Modified: Tue, 30 Mar 2021 23:13:10 GMT  
		Size: 54.6 MB (54565465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa36c31cee26847b9913a77e1631113701b54672f1892eb370c5ec4db2b9da2a`  
		Last Modified: Tue, 30 Mar 2021 23:13:50 GMT  
		Size: 196.4 MB (196360959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:379b05056e5f817f3bd80e7c2677f6c2a002c89843efd33e85407589bce81982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.9 MB (294916475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec16bd53b649b6512b07b30323995e345ea3edbb70fed1ef15733fa65a25fa2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:55 GMT
ADD file:3a982d4cdc7d9461623d85a4b6162531ca9adf2921f0d43a0b548d3710392387 in / 
# Tue, 30 Mar 2021 21:49:57 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:43:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:43:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:44:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:46:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:645891123da6b320ad4fd8cfadf96c77b7144dd25b617222de1fe718cde77e35`  
		Last Modified: Tue, 30 Mar 2021 21:57:27 GMT  
		Size: 52.4 MB (52401170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2ae11e65cec397d581f8bfc50a0c3eb2d363cc2397beaa585ac385f720fcf`  
		Last Modified: Tue, 30 Mar 2021 23:59:40 GMT  
		Size: 5.1 MB (5061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131fae12c09181b2c23186780b133bfe60e76c8af6bc6af4943aed293c993b47`  
		Last Modified: Tue, 30 Mar 2021 23:59:40 GMT  
		Size: 10.6 MB (10569881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e41b734e985a8d169b38913e5fe94cb0348ee05101bc3ad6b952ef8393bddd`  
		Last Modified: Wed, 31 Mar 2021 00:00:09 GMT  
		Size: 52.3 MB (52314580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb3c801e679c04ee82234e325058c6d2dedff4a76fa10d47647f6be5b5c9226`  
		Last Modified: Wed, 31 Mar 2021 00:01:09 GMT  
		Size: 174.6 MB (174569750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b925618eebef2c94b576c7b99baac9705ffec6771cb5b50d7b1a83d32735764e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.4 MB (282375933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13dad972720ac53a49695be1954fe83c267551e5aec0104ce5f648f9d849572`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:15:27 GMT
ADD file:e3651409d9338da981cd9fbd8d9b8511edbde0700ac9e0df8937b859e004990d in / 
# Fri, 26 Mar 2021 11:15:29 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:16:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:16:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:17:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:21:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd9021b04def024e25507cdd1b0967a20a384ad5cc255120cfb8c5f43495fa74`  
		Last Modified: Fri, 26 Mar 2021 11:26:11 GMT  
		Size: 50.1 MB (50073977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6023b28762fcb2cca84dd988c0545da69e2cb9cea40e5fb1a14dce3d7d186`  
		Last Modified: Fri, 26 Mar 2021 13:48:58 GMT  
		Size: 4.9 MB (4920097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94408c405dc2689a60515a2dee289cb3495f53f4b4f9758de6995e07aa073eb2`  
		Last Modified: Fri, 26 Mar 2021 13:48:59 GMT  
		Size: 10.2 MB (10218160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd339501262a81addad6326243dbcf62ca43943542cc42a3b06aeda9a9cdec3a`  
		Last Modified: Fri, 26 Mar 2021 13:49:44 GMT  
		Size: 50.3 MB (50328166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c0e2093ca7e218efcd720cb76df84159a60199e33e382d88d4f9fe16a24f4b`  
		Last Modified: Fri, 26 Mar 2021 13:51:04 GMT  
		Size: 166.8 MB (166835533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6404e114dd358fa6f486ac0c97d06e24fc264ad16a6728d485fbfb7a3193b346
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.5 MB (313481419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5690f9b8f2c4ee878b33b3ec58e8b2eb14bd58b632fed71b92d1c5aec7f5c686`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:09 GMT
ADD file:d2b87aea7c45e4b0e478e3c2eabae00f1c80b5d77f8f579d2ff913c78b44b6b0 in / 
# Tue, 30 Mar 2021 21:46:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:11:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:12:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:14:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1063bcb9135253bd841aad1946f348a3277d992a7ecba4ef1ef68217c3c1b019`  
		Last Modified: Tue, 30 Mar 2021 21:53:23 GMT  
		Size: 53.6 MB (53555197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890e5446d487fcab6d7189e7771c6a50252b2d857c9b70fd4cea1bcfe3a1c8a5`  
		Last Modified: Wed, 31 Mar 2021 00:28:24 GMT  
		Size: 5.1 MB (5140737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b996f43aeb591ca2dd4bc003c5c5e3e982c6b85b7cad5a14591b08209f01b95`  
		Last Modified: Wed, 31 Mar 2021 00:28:26 GMT  
		Size: 10.9 MB (10867476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d44941e2620f2cbcd9d88a5b4b0eb491639112c330530030fb953c4cb4a4a63`  
		Last Modified: Wed, 31 Mar 2021 00:28:49 GMT  
		Size: 54.7 MB (54666730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf3a9a9bdcd7dcf9fb0a769057237cede8030ca48543547d79781868610cce8`  
		Last Modified: Wed, 31 Mar 2021 00:29:49 GMT  
		Size: 189.3 MB (189251279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c8fb48c6e53c4a0ca6cab99fec4d51d410204da40029b57ab7446195870599ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327616347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328fc4c399bc3de3c0c72d5012d0aa421eb40c17daf9c3d8c9a1996f1ad6c12f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:38:58 GMT
ADD file:b5024008ca4ac295c015d04d146515efd534f38efa8793979ad8a6c1cc41a2b8 in / 
# Tue, 30 Mar 2021 21:38:59 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:54:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:54:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:54:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:56:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46dc83097f0241a9cf1128d563661cf2cacf0ca9445152008a4c686a8d125595`  
		Last Modified: Tue, 30 Mar 2021 21:45:11 GMT  
		Size: 55.9 MB (55881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96203cf1270a0522cb74805c17be141b6be163c96591b032d0aeceff808d7b6f`  
		Last Modified: Wed, 31 Mar 2021 00:06:09 GMT  
		Size: 5.3 MB (5280209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63af79a424e53c82e0807d0e90f60c2456bc0ce3accdcee7cb3f1f9f5f70a96c`  
		Last Modified: Wed, 31 Mar 2021 00:06:10 GMT  
		Size: 11.2 MB (11248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaa2fa19667aacbe54d69da17398fd2ae22b23b7bf991725d64c3139c6eb5cd`  
		Last Modified: Wed, 31 Mar 2021 00:06:41 GMT  
		Size: 55.9 MB (55909080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d5f71162a3a85cf57a08e2cdcaa51b4f99fc5755bb072ecf0125455d101213`  
		Last Modified: Wed, 31 Mar 2021 00:07:45 GMT  
		Size: 199.3 MB (199297079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e585adabf3288c4291e822f97d542094daea8f12200b713d902b3e2cc1f889ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.2 MB (301221112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e3d625fa7098641bce312fc178dba8b64faecb7ae45ff584badb5f7a8d820c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:08:38 GMT
ADD file:4c1773eeb1eb8715f5ee35943b6ec536fef99670907da849b45a0a757fbba521 in / 
# Tue, 30 Mar 2021 22:08:39 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:06:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:07:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:10:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1bfb759abe39ebb60de9072afdd4e8e520a2faad8d254176313a6e6015b23b2`  
		Last Modified: Tue, 30 Mar 2021 22:14:13 GMT  
		Size: 53.1 MB (53127187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9534d5829810d03b9be336ae682a19f3b3af31e49b6b2cecd48345d02bd56074`  
		Last Modified: Tue, 30 Mar 2021 23:18:40 GMT  
		Size: 5.1 MB (5112994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efe461f21748a446fa26cb598f3c639bb1d56f946ec69917e33bbf0d1afe79b`  
		Last Modified: Tue, 30 Mar 2021 23:18:41 GMT  
		Size: 10.9 MB (10870209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af545e3a0b4ad1282fd353de2b1a13f1cfb41fddeafbbd5d1ab541524ae6898a`  
		Last Modified: Tue, 30 Mar 2021 23:19:32 GMT  
		Size: 53.3 MB (53299586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e35c40e3db7eb70abb233c649c0d22b681926f055b0822a198ff86b47287a35`  
		Last Modified: Tue, 30 Mar 2021 23:21:48 GMT  
		Size: 178.8 MB (178811136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:05c5ff1d2d777d6b0e8c6140f4328068a61ec87356bf286bc27241def238e093
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.3 MB (330278898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5edc32d331387d4e24476fb2dbd22b3c2b76bd3eb021ac8062174df50a6b74`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:12:40 GMT
ADD file:28f7d129aaacc2de6bb78dec104b788d0aa25aaac87e07873668354a5b755268 in / 
# Fri, 26 Mar 2021 15:12:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:13:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 17:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:34:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18ddfb418fe2dc2d92f9b851d0345827010c7b001ef98bb5a8b1730d80e2eace`  
		Last Modified: Fri, 26 Mar 2021 15:20:35 GMT  
		Size: 58.8 MB (58756702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e58f4581a73db06180cd5d10d619dc8b47cdbf57bed71dbf9eb53d28bc4749`  
		Last Modified: Fri, 26 Mar 2021 19:34:46 GMT  
		Size: 5.4 MB (5399177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e302f47f5e7c563d0f23745e32bd160587a44a206808295a2ca9d29a6b9d67`  
		Last Modified: Fri, 26 Mar 2021 19:34:51 GMT  
		Size: 11.6 MB (11619666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9f221c0a34707baac4ad94f19a4bd62b803303c74a200e7d8ced228745c108`  
		Last Modified: Fri, 26 Mar 2021 19:36:24 GMT  
		Size: 58.8 MB (58846493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309330cad3618c41f1fcedf5b26c33744337ec55b741feddf35bda0d56d9e50c`  
		Last Modified: Fri, 26 Mar 2021 19:40:05 GMT  
		Size: 195.7 MB (195656860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:317acb802563fb3cfc611003071ebf02f2c63d7ab17da8d8d40e610006b7d5d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295440220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96dbbec2bc883fed75705825f047d1e752958a5b1566745cb578b0caea63bf1e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:00 GMT
ADD file:06cd9dd574d91229d3aa7c645dda03791fcfbea17bb5964aaa1c5830d4174ab2 in / 
# Tue, 30 Mar 2021 21:42:06 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:41:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 22:41:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:42:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1babe08b94dd6b44aca97f5f46b49d3c3e8b1571a49971cc87c69f9c91056218`  
		Last Modified: Tue, 30 Mar 2021 21:45:29 GMT  
		Size: 53.1 MB (53148454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870ee6737fff361d9c0e6f905afcc7d45e779397ee67aa5b284eea46c9bd446d`  
		Last Modified: Tue, 30 Mar 2021 22:48:10 GMT  
		Size: 5.1 MB (5134079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54e0f71a88fa90537f4f2b0b092586cde9dc64e5833c45246c5d15be4e2ea20`  
		Last Modified: Tue, 30 Mar 2021 22:48:16 GMT  
		Size: 10.8 MB (10758401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6830c9f51e858407cacbf4450a91779c76f65e97ce85e9cace8d2eb566302487`  
		Last Modified: Tue, 30 Mar 2021 22:48:34 GMT  
		Size: 54.0 MB (54038371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a357dbc6b0a8ff3aa1ab3ac042bc3637679a84bd1c21298d8a1f6ba9a66c58`  
		Last Modified: Tue, 30 Mar 2021 22:49:06 GMT  
		Size: 172.4 MB (172360915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
