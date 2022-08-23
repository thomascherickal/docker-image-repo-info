## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:2cddd8710936ac43710fac7ed0f613bc068e03b9eaee0c030d2d3a3680d5ff3f
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

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fdd46ac593b0dc4c54497b36e00e54c7759d068d9b9f014bd5b47bed430d4c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322416189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1966d2c176635cea14ac52f6a8a1d7d57101cb829eae63a9f3597cdee7a0ef6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b983117533b718374f1701ef593dd2afa6613c7908c6553be8e2a150e6448a`  
		Last Modified: Tue, 23 Aug 2022 00:56:35 GMT  
		Size: 196.8 MB (196785008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:48f086404ea033fe19fa0dd18cd1989c0b585f07c7353ff246098068b1075971
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295500312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543ae8ede83fbb55855cee053b3a548534170a1c9e89ce34e227685abb1a46f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8993dbe2a09d90eb21f3d73a07f953f77bed210372ca285a9f7d8046891b8aa`  
		Last Modified: Tue, 23 Aug 2022 06:28:23 GMT  
		Size: 175.0 MB (174987686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7987ee20b3a50997d12b674687af46607da3ad57d1fe204f0cfa233f7f259fcd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282952810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1f5bdfe776fa370ce01436f7274c312e50139c8660690269e0e2bc01800814`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:36 GMT
ADD file:4e2780cf1c53cc1c475d2ebae48d4bf03029fa68ba9fbc991be76ac9e3944977 in / 
# Tue, 02 Aug 2022 00:58:37 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:47:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:48:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05aa23077de69478dfc20e56aa2d54a2b13bbef07c4d2578524585d098af4e72`  
		Last Modified: Tue, 02 Aug 2022 01:06:07 GMT  
		Size: 50.2 MB (50195271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47a4ec510d3ede75fd285276ee8b3d9dd3c1d2bce8f21ae0f2de4898c015b9e`  
		Last Modified: Tue, 02 Aug 2022 02:09:14 GMT  
		Size: 4.9 MB (4930860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef792f88dc77db1940eec048a6d0b4d691c7650b28cd058aed9314fea5f708b6`  
		Last Modified: Tue, 02 Aug 2022 02:09:14 GMT  
		Size: 10.2 MB (10217964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f493c1b0c9a50775af17259c793561f1ce1c5ab4bbf3947d8ca612f476bfcf23`  
		Last Modified: Tue, 02 Aug 2022 02:09:40 GMT  
		Size: 50.3 MB (50342099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c48ddcd5b44d4a1497734e2118bcf667a1db4348a386add70caf1c8577c09`  
		Last Modified: Tue, 02 Aug 2022 02:10:28 GMT  
		Size: 167.3 MB (167266616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6a657d9df2ce6540c05ceccaae91f294cb8ad870d9ea7cbc582a0642a5a8e0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.7 MB (313684616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c31d31f8a9a1673a5b75dcc8e41518512dc0227c069e4cb4a48a9d45a3ade89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10f752bfb9bb5888d549687e75a51ad78e1523ee87958e8b464cbd4dee4bb2`  
		Last Modified: Tue, 23 Aug 2022 02:37:46 GMT  
		Size: 189.7 MB (189711278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6462b9cedd6360f9ac58ef0a745ed79497259cf4382b330b0a6ade58054037fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327786054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a954a50143d33244bd5b54771fe808f36befea012da728e64638c4f80b3f6b8c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e27a84eb0ba3a89f9e9e474d9c853c2dc7e9c83ef7d1e7281d208fd866b4c3`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 199.7 MB (199732145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:35816b67004ddac847e68d474485fc3fb5e5ee3b8dcd4461884f7b36a96a2678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301278928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153a518aa28b3de0356ff748589cf74b2d627c49254dc6b4add1883a093425b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:09:59 GMT
ADD file:d4bcd76354f6ce92e52e206333ebbe2399c24e2ee5b19ae5f758b25dbda35efa in / 
# Tue, 02 Aug 2022 01:10:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:55:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:01:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b6232334ba5947043903a2c95b6b7c6e6b613d66b10b9cad82702032585b0d8`  
		Last Modified: Tue, 02 Aug 2022 01:20:18 GMT  
		Size: 53.3 MB (53263487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77db3f931ef8e6c6e59d3af4773381ee1557b70b35c21e01543324bf664e132`  
		Last Modified: Tue, 02 Aug 2022 02:24:11 GMT  
		Size: 5.1 MB (5123478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cd018f526c1a738a2f7b90dbeb1439a31059e66e9d09c98807c316b6c72e1a`  
		Last Modified: Tue, 02 Aug 2022 02:24:13 GMT  
		Size: 10.7 MB (10660940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35e4a84a02a342bcbd6764be5e369e4b07630db2011302157f21d32c41a72ef`  
		Last Modified: Tue, 02 Aug 2022 02:25:04 GMT  
		Size: 53.3 MB (53303907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e589fa8497a937455889b1ac4e6dea238215588e05be5006c22a453dfe39eb`  
		Last Modified: Tue, 02 Aug 2022 02:27:09 GMT  
		Size: 178.9 MB (178927116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d26e0e6609eee5d0cc12d24a0e666e615785a20c5f2bcc91b8c39a3a1a85d14f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330981508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4404daf2be9fe8125eb280020678875923138a2f95a6de510414b2979fc8ea78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:01:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fecee5c5cd927c82781b73850d4cbf96c866f08985a8a76ee30c510df49f06`  
		Last Modified: Tue, 23 Aug 2022 02:12:17 GMT  
		Size: 196.2 MB (196164591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5584b9a69f182e691aa74e57df2bd2d1d7d8981bec87ab04be4e75b56d4c5e25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (296008380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22679580e8c0a7d957b4067b5b3be708088a9fec04390ae38a7c617efe04eec3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:09 GMT
ADD file:86774aefa6717c0535c25f8700d8730f44cc43c33371edeb7dbd33e29cb68d32 in / 
# Tue, 02 Aug 2022 00:42:12 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:08:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:08:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:09:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:09:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:718eef7927531d5ec3c355d6b6e5c4ab83c23778e693b087ac8a3b9adb4f63e0`  
		Last Modified: Tue, 02 Aug 2022 00:47:40 GMT  
		Size: 53.3 MB (53269308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75c9e8bd2b82703a7391c7c97d600a7dd7c19920de10bdd95845e75ef24b782`  
		Last Modified: Tue, 02 Aug 2022 01:35:15 GMT  
		Size: 5.1 MB (5141077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c031131df71d864714d521c4e6f6628302c2013df50dfbc03a037f443dc7e2`  
		Last Modified: Tue, 02 Aug 2022 01:35:15 GMT  
		Size: 10.8 MB (10765648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a89f4f0aa5bac70077c0ec90c8258fa1ce257b76c156456acd2105445eaf7f`  
		Last Modified: Tue, 02 Aug 2022 01:35:30 GMT  
		Size: 54.0 MB (54045416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf5db7c4836a151fe7b056fe47baffb43cb449aa279f50558932dfe163b6ab3`  
		Last Modified: Tue, 02 Aug 2022 01:35:59 GMT  
		Size: 172.8 MB (172786931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
