## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:9b97a82b23b86ecd2ab8f8697c4524c3c5d7822db5630aebc28129abbc3447c7
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

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ff20b5aa61168cb54cd269b63916ca89224104c7819cea17465ba64afeb14bed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.1 MB (323149990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb89c5d4fd21f16b8b67e65a5dfde87aac49efcf8f9e672e2501a575967417a6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:25:32 GMT
ADD file:2496494632885054452c6f15317aaeace67145465fe0f719da9d3b5c95e6c8ed in / 
# Thu, 16 Apr 2020 03:25:32 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:09:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:09:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:10:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:11:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4396830990ba6684412015e660aecabd027170dd4336124dd128865a6a81898`  
		Last Modified: Thu, 16 Apr 2020 03:33:46 GMT  
		Size: 52.0 MB (51976212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e4b8dc00ccde83638bcdc38c48e437757b1891ffbc63bba9e3fe11cd2f70d`  
		Last Modified: Thu, 16 Apr 2020 04:18:37 GMT  
		Size: 7.9 MB (7933282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1945a2e225e1c6c7667997f238da1810114a7c8260dfd32f9fe4281719b17c6`  
		Last Modified: Thu, 16 Apr 2020 04:18:37 GMT  
		Size: 10.3 MB (10298119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b97794719e7218495589ddaa99735f4c9a7a87113187a3e00ec3cf7d29784c`  
		Last Modified: Thu, 16 Apr 2020 04:18:56 GMT  
		Size: 55.7 MB (55706282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb742b1b214dd9249248a00df8aa44277cf39e5c12aeb8c11a0dc6037e7df05`  
		Last Modified: Thu, 16 Apr 2020 04:20:12 GMT  
		Size: 197.2 MB (197236095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f25bd212c91b62dcb74a55dca93578b327ddba4ab400c69258a2eebed8a36145
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294557061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c40ad164dc8e633786e026e300ffcceb16dd9f928cfa20868ead17a85dbcbd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:27:39 GMT
ADD file:a797b22ab77042681c9442f161cd9c34b230f5e897a7c038c5e619cf0e8159f3 in / 
# Tue, 31 Mar 2020 01:27:45 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:35:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:36:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:37:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:39:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a071e689ab0273b55b5ea6cd2f8c7f83096ceff8fb3d7a616e059804c29d70c`  
		Last Modified: Tue, 31 Mar 2020 01:35:22 GMT  
		Size: 49.9 MB (49891269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e955f774e68fb041a9d50840f6e6c139bb7aa9f26aaeaeffed32316761a69b1`  
		Last Modified: Tue, 31 Mar 2020 03:50:06 GMT  
		Size: 7.5 MB (7512962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97a6ee6cfc96be92a20ec0b7b805e4c521d088957adbd612a4252a4f45ed15c`  
		Last Modified: Tue, 31 Mar 2020 03:50:06 GMT  
		Size: 10.0 MB (10008505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571262e91f17243db435c188e3873071be5aae97276bad3f0a2e436bd99b555e`  
		Last Modified: Tue, 31 Mar 2020 03:50:31 GMT  
		Size: 53.3 MB (53267425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c7452ff8d54812d565249b583f15108c582baa2e5eb169a14220de65ec25ea`  
		Last Modified: Tue, 31 Mar 2020 03:51:25 GMT  
		Size: 173.9 MB (173876900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:711a48fc5aac99c8b4c542ec4d683606461f918a66b2569e69cefe8dab42465e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288863095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d22b4354066d76251fb55d562508e1b259fc7ad403e5f91649d6ede1d1461`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:50:55 GMT
ADD file:fdbba631aa2e54ebb3f3a92627367ce7e2e6efb1157a884945e4d69c360073ea in / 
# Tue, 31 Mar 2020 01:50:57 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:49:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:49:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc5c37e59a5331bf2b56343097ed41f57f5df3c898439059baccb2d6dfbcb203`  
		Last Modified: Tue, 31 Mar 2020 01:58:45 GMT  
		Size: 47.6 MB (47626226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c70a792a98ea8510fe5ed73c7568e177f2c055525cabdeec63f3b252f9785d`  
		Last Modified: Tue, 31 Mar 2020 04:03:18 GMT  
		Size: 7.3 MB (7253641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f4973145ed34075ebb198eb399df21ca2d3d039494b853c612c0848fb447c5`  
		Last Modified: Tue, 31 Mar 2020 04:03:18 GMT  
		Size: 9.7 MB (9672910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f44d80d06a7a6f1d0a37e8ac63f05264d98ae04e13c146e3610e0bd40c8d930`  
		Last Modified: Tue, 31 Mar 2020 04:03:40 GMT  
		Size: 51.0 MB (50966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e8fbb1a745c8b0ae1003abd83aad9271e7b102e6fb48b8847aa883d1db7fc6`  
		Last Modified: Tue, 31 Mar 2020 04:04:33 GMT  
		Size: 173.3 MB (173343508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5792a13a6a51a2966ca3c6894bf96567d9c328346f4730ee5e529d538ca68d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (315042930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ba1271e94ee8be258cca3aa25b960bf446153705bf0be834cf1d2c4cc12377`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:43:10 GMT
ADD file:ff8b5c2517d26b49a4c8114e515f5413a0c64b28ff1e5d3fa1bd70603aaadff6 in / 
# Thu, 16 Apr 2020 02:43:13 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:18:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:20:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f361d4eae096128866baf55f9d19448df20331f319ad8df0f05397bfd2fe7fc`  
		Last Modified: Thu, 16 Apr 2020 02:49:55 GMT  
		Size: 50.9 MB (50910038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c3a136011851aa29f08165cf962f4b5df6865a2236b90a5fc6d0f1c01ded33`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 7.8 MB (7808061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d0c43c17c0157ca9f4cd6b676d7a8e76ef248c724901495c897b950e8ff1b`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 10.3 MB (10294341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a324e1cc769adafc8b7660201edefbc372e565378179fb1de4f142725a42842`  
		Last Modified: Thu, 16 Apr 2020 03:29:48 GMT  
		Size: 55.8 MB (55809319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6da6a182aa0c6b85a665f864bf43d76924f3e6730b05cc66eacb504106819`  
		Last Modified: Thu, 16 Apr 2020 03:30:42 GMT  
		Size: 190.2 MB (190221171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9987c0458b1b8df2d94e09865df8ef1b9318e36276990c86f5ff53ee34e727c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (332955288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25b6dcd363b76fb520f28fefc2113db0fefb88c2033919cdea1f8a36d09e400a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:41:56 GMT
ADD file:af11f81927371cc0ed957aa36f4036c71c73a0b79ab27523cf0d49d8e0260041 in / 
# Thu, 16 Apr 2020 01:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:31:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:31:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:32:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cf4ce40baf558f42709af03658907805f477c72b1b1a39869aef429cd35cd3c`  
		Last Modified: Thu, 16 Apr 2020 01:48:16 GMT  
		Size: 53.1 MB (53130042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcc2dce5f80bcf713e09688ddce4e707509747c60ac5dcb21b50ba63fa26bf6`  
		Last Modified: Thu, 16 Apr 2020 02:39:42 GMT  
		Size: 8.1 MB (8110058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96fa002b78190463928c6db889856164ede953e0bbc48a860d1856d448dd69`  
		Last Modified: Thu, 16 Apr 2020 02:39:43 GMT  
		Size: 10.7 MB (10657287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7351fce1761580c1a90469f6a39ce4b504f9c1b1c46ac9de64a36b5067846200`  
		Last Modified: Thu, 16 Apr 2020 02:40:03 GMT  
		Size: 57.6 MB (57552290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafcd6750aabbb340f9ba85c9c542284cad359876a28e94fc2e3fa34baf2fea`  
		Last Modified: Thu, 16 Apr 2020 02:40:51 GMT  
		Size: 203.5 MB (203505611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e317064ad0ddcb7814a2852d51699be6fafe58e824a7b7cf55524e978978bdda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.4 MB (342419507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f5aecbd896de12d2283272db6ae6135ef388158e15349d2c75d58ed46f885e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:34:16 GMT
ADD file:8f010ac42180d1a69abeb831a2cf65af2b505dc37ca5566d1f8e0af98223a68d in / 
# Tue, 31 Mar 2020 01:34:25 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:32:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:33:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:35:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:45:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a96cc3285dca9557b63f3a1daed7cabe2c2e3fd70599474a054f37ae9105c6c`  
		Last Modified: Tue, 31 Mar 2020 01:48:49 GMT  
		Size: 55.8 MB (55834936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616d46070d2d79dda9e6b725a456cc523fced90f731b94a80fe3b63dcbb34f63`  
		Last Modified: Tue, 31 Mar 2020 04:04:16 GMT  
		Size: 8.4 MB (8354814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30854a2a0cd6b68888c600cb3b15000ac47d6f0a9bb3ccafda003ddeebe996f`  
		Last Modified: Tue, 31 Mar 2020 04:04:16 GMT  
		Size: 11.0 MB (10975756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371525c676a3a79f437345a7eeb988835dfceaba7ee6c5cd16e3e63ca520fd21`  
		Last Modified: Tue, 31 Mar 2020 04:05:16 GMT  
		Size: 61.0 MB (60995864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94c90a728d9ac9dfd6164d3c8ed063c7cee43143c7923a5c80a2ed8259ad1cd`  
		Last Modified: Tue, 31 Mar 2020 04:07:03 GMT  
		Size: 206.3 MB (206258137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4752bf335713ff05964ff36edb85ffefcdcafc53d2badaae12b1927297b69c9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303841011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f959fa9a40062bccc88eadec33d35bfd06d37f9d8568e6d071ee2a9e755986`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:56 GMT
ADD file:1d96a73c9c03d31b0a60aa6b4e0215085afcdee6dc39954655798110c12c223f in / 
# Thu, 16 Apr 2020 00:42:59 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:01:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:01:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:02:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3633d30b569d7f8e4addec62b3bb5c460572eb82d6568a9bc40a9f189dc4bdcb`  
		Last Modified: Thu, 16 Apr 2020 00:47:02 GMT  
		Size: 50.6 MB (50576543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275dfe1709bf7bfd1a7e225a7b974994148dca503ef21f837a74970529f9eb01`  
		Last Modified: Thu, 16 Apr 2020 02:07:15 GMT  
		Size: 7.6 MB (7600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae5ff7d1251f85fd4f476599f4408381f4e029ec36f4f1b66a96e89b921e7a0`  
		Last Modified: Thu, 16 Apr 2020 02:07:16 GMT  
		Size: 10.2 MB (10183857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686e996ff9bb08017109e59fc8068db8d4300aea3359952891468365b7d82d4d`  
		Last Modified: Thu, 16 Apr 2020 02:07:29 GMT  
		Size: 54.9 MB (54938818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d362dfd0707b3fa482170b42639e30066018bcd3bfe71db17f87006b35d38f7`  
		Last Modified: Thu, 16 Apr 2020 02:07:57 GMT  
		Size: 180.5 MB (180541722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
