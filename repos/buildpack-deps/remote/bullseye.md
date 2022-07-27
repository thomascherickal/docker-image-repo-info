## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:b347bcbf8af686ae8f1fb07b23540c63ef0b18920b03d7dab7699f5599cef887
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

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:847a7b943c92d9125daed3552642fda88978b9dd3881a34cdfcd7ed22d259395
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322385290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b7450f22becd372d2c4a64821ff1eb9f2383e0e2e777e945988e13ad0d68a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:48:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:48:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a9e63c657ad881997f5165c0826be395bfc064415876b9fbaae74bcb5dc721`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 5.2 MB (5156110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1989b6e74cfdda1591b9dd23be47c5caeb002b7a151379361ec0c3f0e6d0e52`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 10.9 MB (10876416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28818711e1ed38df107014a20127b41491b224d7aed8aa7066b55552d9600d2`  
		Last Modified: Tue, 12 Jul 2022 02:55:23 GMT  
		Size: 54.6 MB (54579006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5084fa7ebd744165b15df008a9c14db7fc3d6af34cce64ba85bbaa348af594a3`  
		Last Modified: Tue, 12 Jul 2022 02:56:00 GMT  
		Size: 196.8 MB (196774352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:230c3127b14b801326ca3e3c131463b1f2acebe9f5c884f2d55236928e75bd87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295471821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24f00569668030e02ec61898131bb16040b0151c6642b6e8f3378188f2f8448`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:49:58 GMT
ADD file:a600937adf471d1624223b1e4fc5af3391a3258d28051f9f9990c978177db2ec in / 
# Tue, 12 Jul 2022 00:49:59 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:38:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:38:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 01:39:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:42:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:458c615f383e394cdb1d249caac254a3148895cc59ef0f317e0c342507c0a43e`  
		Last Modified: Tue, 12 Jul 2022 01:02:12 GMT  
		Size: 52.5 MB (52536893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79ef49a3b907a2575e08477212bfbd57aca6b32371844cdce520dc7a2e688e`  
		Last Modified: Tue, 12 Jul 2022 01:57:42 GMT  
		Size: 5.1 MB (5065360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cf6d68feaf378688713585399ee409bdef4481481b83d4896d6861cb380c90`  
		Last Modified: Tue, 12 Jul 2022 01:57:44 GMT  
		Size: 10.6 MB (10573756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e72d965a8962ee5d2e575801caee59ea34cef71d8b95f502fc38b6c201c9f1`  
		Last Modified: Tue, 12 Jul 2022 01:58:38 GMT  
		Size: 52.3 MB (52314808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd88eaff219dbfcdb23531f2eafd976029dc72583a3f209631b1ff580652c0`  
		Last Modified: Tue, 12 Jul 2022 02:00:38 GMT  
		Size: 175.0 MB (174981004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:19529dcba1211b7f89294587f30d24c9079bcdb8226eee06c0b3646b6df4c1c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282920355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f49549d1328c0e8c83c8f2c7b4c592403e6415786c78dd43c4846b86f6375bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:28:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:28:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 03:29:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:31:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042ae471fd57ff8851607bf0b66366fbd0a499a0ce088f1fb39c5a1caf4123e`  
		Last Modified: Tue, 12 Jul 2022 03:50:27 GMT  
		Size: 4.9 MB (4924746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70da2acc639b7236796e6cb2a0b0e3a21e6f32f8a507bdbfb823a510caf8e75a`  
		Last Modified: Tue, 12 Jul 2022 03:50:29 GMT  
		Size: 10.2 MB (10218056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f084d2e4e20e27a866ad87c0a2098498eddc9f471988ea44068990b299a29c`  
		Last Modified: Tue, 12 Jul 2022 03:51:21 GMT  
		Size: 50.3 MB (50329897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c906e18d849e9c3e642b6247a1dadc627d6902a581866ab147dc84e01b7e3ee1`  
		Last Modified: Tue, 12 Jul 2022 03:53:07 GMT  
		Size: 167.3 MB (167252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3721870178c0e02db9de0f056b067b9bcf8e437f73e590efd228dffc1b2d2a95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313838296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d77170a2d290c76e1c18256d4246566ff1c46fb634227a66d5993b803af4cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:18 GMT
ADD file:2dcc013bca5a420cad3b6a1ac61f52ea58a29ae05fe282078a744979c0e1a89e in / 
# Tue, 12 Jul 2022 00:40:19 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:33:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:33:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfc947b533a3ed8b8ce79820c7fe5e7634bf9c08479ed0aee1e74ee7b4f2b068`  
		Last Modified: Tue, 12 Jul 2022 00:45:41 GMT  
		Size: 53.7 MB (53683129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca36aa4204d2a708dcd1d41d1d4a128b095f8d88a2f9544f89799c36914e356`  
		Last Modified: Tue, 12 Jul 2022 02:42:29 GMT  
		Size: 5.1 MB (5142960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdcd2014de70fbce8c43a70cd1f42bceab4f1e35953db987fc318dbc0fb0d26`  
		Last Modified: Tue, 12 Jul 2022 02:42:30 GMT  
		Size: 10.7 MB (10657500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e288b20a616767a00416e22f7d8ee6390ba5b48061d92577f55bdb11121e6946`  
		Last Modified: Tue, 12 Jul 2022 02:42:53 GMT  
		Size: 54.7 MB (54673820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c814ed089439a4f3618519b0ae7ef02da9c1c3fc1535824d633ca1f76e78dbf`  
		Last Modified: Tue, 12 Jul 2022 02:43:32 GMT  
		Size: 189.7 MB (189680887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6af5c16aa0a669213f7f5c68f537bf71e0e7aab2ad2c4b114e02638f65b186fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.9 MB (327945456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b778bae0856c22b41e469e3707a86b77b316360ac9d10668372ba2e38677152`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:10 GMT
ADD file:0fe47b589e2fdec2c7f7e92ab50ee94c37df9276c6771e612d29fde3aefb04b6 in / 
# Tue, 12 Jul 2022 00:39:11 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:26:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:26:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:27:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:28:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992c2740c28ef02c375c076416e9a24c9172d5343205500b8388cf087a76bbce`  
		Last Modified: Tue, 12 Jul 2022 00:44:46 GMT  
		Size: 56.0 MB (56001770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b010a51f3f025a5092ebdeabc7eb1a2c2b64a0782cb5f2848c30055d5561437a`  
		Last Modified: Tue, 12 Jul 2022 04:35:57 GMT  
		Size: 5.3 MB (5284906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d877135d65d11955788587fb1d70efe0d09ac15edfe3850946b5237926fc322e`  
		Last Modified: Tue, 12 Jul 2022 04:35:57 GMT  
		Size: 11.0 MB (11032943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5afc941d55bf77416ea689331bc9b09d9ea20aea0c8661c44e4840af148c20`  
		Last Modified: Tue, 12 Jul 2022 04:36:20 GMT  
		Size: 55.9 MB (55914438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807d828eab07ca95bc9f3d997d92de917084306d7226205039e37890d4054b5d`  
		Last Modified: Tue, 12 Jul 2022 04:36:58 GMT  
		Size: 199.7 MB (199711399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:902af32232b70553a44efac199b8b180b2efc9b2ce0393ed25eae3b32d8b3fa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301265695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb50ed24d16c433cef10f6bf10f9dda260f02b283232d4e2859bc10b5d3e0cfa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:19 GMT
ADD file:5a045303c511235feda23815b401564f1db25de2c312598258626e9be22c303a in / 
# Tue, 12 Jul 2022 04:40:23 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:09:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:17:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe8f2bf6b579db32fc573a5f145cbb10fddffc9fced5f528ed1b70b2c18dd94`  
		Last Modified: Tue, 12 Jul 2022 04:51:00 GMT  
		Size: 53.3 MB (53263285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3283d319938af21e206873861ea7c615ffe89e2770155269213eb3801ea6ef02`  
		Last Modified: Tue, 12 Jul 2022 06:40:24 GMT  
		Size: 5.1 MB (5117493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169e575c90587844ab6e7ee2c27f5389c260d537f4f69c2b3b97e313f2114791`  
		Last Modified: Tue, 12 Jul 2022 06:40:26 GMT  
		Size: 10.7 MB (10660566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea6ddf91fa6d28cbbcce640b99b4dfb8df5cba0699a38db6924a2ba12136487`  
		Last Modified: Tue, 12 Jul 2022 06:41:17 GMT  
		Size: 53.3 MB (53299246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dc7292e012b1302c8de272ac466fdb4c080d8d2ef319e7a46a4ce3d4682a45`  
		Last Modified: Tue, 12 Jul 2022 06:43:23 GMT  
		Size: 178.9 MB (178925105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:adf2895082dcb323c67ef6ccb5ddd0be52f8611abc775bfe6fe3bab380943adc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330934675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f050ea13310974e946d169d8c7f807c252bb4f9bc829ba8a6f0047a05072ba18`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:24:58 GMT
ADD file:98243e1bfc9c04ce4d47bbf13011c502c01aeea3a0417b4e2b8f90b4debfdd32 in / 
# Tue, 12 Jul 2022 01:25:03 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:32:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:33:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:34:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:44:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fb3da208bae11b3dc38c4ab84ad048c030a1da966740d02681a11866ba2230c`  
		Last Modified: Tue, 12 Jul 2022 01:35:06 GMT  
		Size: 58.9 MB (58895620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e755f0c9224d9a09cafb660e90339be47b26c4c9584cd9d94ee5c943beb9e0af`  
		Last Modified: Tue, 26 Jul 2022 23:47:52 GMT  
		Size: 5.4 MB (5405301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881c506b97552bcd229e65b7d010773118d7abbcbc802525defa3481c7243e7b`  
		Last Modified: Tue, 26 Jul 2022 23:47:54 GMT  
		Size: 11.6 MB (11628514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec75d0c4cfdabee064149a9394d0a742aa9af2d5791f5115e28291f13f91df3`  
		Last Modified: Tue, 26 Jul 2022 23:48:29 GMT  
		Size: 58.9 MB (58854704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f6a6d47b1cee2dd8e275cb173405964162ca156d91a87259a4a87dadf7edd5`  
		Last Modified: Tue, 26 Jul 2022 23:49:31 GMT  
		Size: 196.2 MB (196150536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7daf570af7eddcf3852fe07aeff255e979a825376ca3c753e75dfe34172bc6b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (296011287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f0018466f904ba41a7d569af38c6b66396677238758bdee5aab9302b789cf37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:15 GMT
ADD file:2a729374ad3e12361206aeffbdface900970f010684d6409328d6be136facfa0 in / 
# Tue, 12 Jul 2022 00:43:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:38:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:39:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:41:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8c4856949e70ae5ad889cfc6a747677ca43e6945c3d56e2d4e3ea5e17da91a2`  
		Last Modified: Tue, 12 Jul 2022 00:53:19 GMT  
		Size: 53.3 MB (53268948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85304dce7d82a20f3528edaa2f642b51acaa7ad37bf801bff37fb58285e162d5`  
		Last Modified: Tue, 12 Jul 2022 02:53:35 GMT  
		Size: 5.1 MB (5141175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbadc5d6341427c002ee8974edf24880be07e7dc4f99c9007435edf337f950`  
		Last Modified: Tue, 12 Jul 2022 02:53:35 GMT  
		Size: 10.8 MB (10765692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd57258941e6f27be345136fea0ab731687b040d44631f55e4efcb475508b078`  
		Last Modified: Tue, 12 Jul 2022 02:53:52 GMT  
		Size: 54.0 MB (54045563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323fe7b03f8327e965ce25afaf756752dce8aadeedd53f4b1c220f6a412c48b`  
		Last Modified: Tue, 12 Jul 2022 02:54:22 GMT  
		Size: 172.8 MB (172789909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
