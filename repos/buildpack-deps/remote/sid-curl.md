## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:4a9bf8e98655b0a3c9f41c0ecaad46121be1b0cfeceb74ae5517eabd13c85fb8
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9ffd496c1d65d2ab8d141b60b9cb0f101cc2f93ba0c9d35469404d4967ca7d90
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69726826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b84678c778b3f827a4a02b40899748399b1d87a8b55f31454fb4f4b3b1d6220d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:22:27 GMT
ADD file:5055617b757ba2ab1ac6772dc2ee4cfe2ba79dd3900150b470dc61e950b9ce78 in / 
# Sat, 01 Feb 2020 17:22:27 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:31:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:32:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:32a93ca5e0379da8be0d576367bec537380c472d398bfe5587345c3b95c3bf4e`  
		Last Modified: Sat, 01 Feb 2020 17:27:53 GMT  
		Size: 51.5 MB (51549534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19e480f63f2edd34af658275271f6d3372323ce55f29df69de46b9dcaa7723e`  
		Last Modified: Sun, 02 Feb 2020 00:40:54 GMT  
		Size: 7.9 MB (7919872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf4aed71250b9a2716765ef62b4879d32e93915e7ec10b4f1cf248de8edfdc`  
		Last Modified: Sun, 02 Feb 2020 00:40:54 GMT  
		Size: 10.3 MB (10257420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ee14bcdc60f2859f6ed2b27812e12f77af4f866ee6ed52bad3cf11adcd037f7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67008884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fbd6a664f1138c80674c2a00e92933da8598ef4b81ab7fb8b87cc44db06547`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:52:33 GMT
ADD file:e863dd2efdd5f4a6e29a4da391218d83cf13d07b263a55c438361d48079dd528 in / 
# Sat, 01 Feb 2020 16:52:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25551be68c42d4da1cad9359e21cdc842a69363b035a77721ddf9ad7db276105`  
		Last Modified: Sat, 01 Feb 2020 16:59:21 GMT  
		Size: 49.5 MB (49540705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718af626bdc2f1b7d5facec6b5ba8016afa8bb5d691f4ead7274c55588a7bf48`  
		Last Modified: Sat, 01 Feb 2020 17:47:57 GMT  
		Size: 7.5 MB (7494164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19493feb9c608ccc1c197cb34c49c8902d9e560ef999db9500a91a6244e10e0d`  
		Last Modified: Sat, 01 Feb 2020 17:47:57 GMT  
		Size: 10.0 MB (9974015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6c358efea480f5577835f092b9ddac5c933268b5722a1fa9f4bd4dd26f4876f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64153881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1a2a1840bd699e40a7a57b330f5f7ebdfb04c72faa85b808515e282cb79a45`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:02:49 GMT
ADD file:a4c8ca5f07a6e213b314bd30a4cd27bba9df71ed8ad4f5f82c07878e8cf99f39 in / 
# Sat, 01 Feb 2020 17:02:51 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:14:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:14:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:983ca3edff7a1184ea4165bcc490182822501d698a99e9d6bc8d6c042881bb97`  
		Last Modified: Sat, 01 Feb 2020 17:09:51 GMT  
		Size: 47.3 MB (47282209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087eb801e68fecc5e62e530d27b51862c664c2f3864a49a5de683335fe76ff32`  
		Last Modified: Sat, 01 Feb 2020 18:29:32 GMT  
		Size: 7.2 MB (7233892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39dcb92a180a0696b4e0192f43515454f02db1da2f7c7eb7d2fab9f7fc58fb75`  
		Last Modified: Sat, 01 Feb 2020 18:29:34 GMT  
		Size: 9.6 MB (9637780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6f72ad10ec6f1980ca1d9e1563a7f60fac241d7b1a5806ac6fb4d3097099fbbf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68551681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198216a0da7f9255c3d05108c9781f871197b9debedc93bcc2242aca845a4372`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:58 GMT
ADD file:636edb6845120aa418f3291c0858ab38c7d658cb2790c08b113e8068fe152a32 in / 
# Sat, 01 Feb 2020 16:42:00 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:26:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a3f06cbd9a524c44b9b8c92922dc9c06d87668d76af414bd34aeb7238502e475`  
		Last Modified: Sat, 01 Feb 2020 16:47:18 GMT  
		Size: 50.5 MB (50505966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66da598f357ac8ab4c813dc7a16cf57b1d0fdc7579b59a9a2cee24efb09f057d`  
		Last Modified: Sat, 01 Feb 2020 17:37:33 GMT  
		Size: 7.8 MB (7793001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a8f172b9e64796699f56dc5a838982165c0591f68740791b1d1e8971e09602`  
		Last Modified: Sat, 01 Feb 2020 17:37:50 GMT  
		Size: 10.3 MB (10252714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:26ab61b13abcf9a44c08aa0b9c60d748ede05d95fb2037ee555f41e82ae5cdda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71395451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6c43c712fd8fda7a88e24090be4b4e9f3c12eab94d9f52dd781b792292e463`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:00 GMT
ADD file:941e54a7461d61d84748dacc44e888cce50acfb10e34f38a7e4083e19f23b7ce in / 
# Sat, 01 Feb 2020 16:41:01 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:36:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8901e4e25f1677947cce32c9111e1a14e167a08c1c9b0f38aa3b62ad8dfa24aa`  
		Last Modified: Sat, 01 Feb 2020 16:46:18 GMT  
		Size: 52.7 MB (52679793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a37f13c8736e8d302836bf7f36d02b6d21c78ea34eaa0d441bfac8ab1e8c15`  
		Last Modified: Sat, 01 Feb 2020 17:44:29 GMT  
		Size: 8.1 MB (8093419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf161fe0fa72e46e5ea25da7008f0141c7c33bd269c543c8f95df1e56c25b90a`  
		Last Modified: Sat, 01 Feb 2020 17:44:29 GMT  
		Size: 10.6 MB (10622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aafaf30bd9089575e8765092202b8ae6636c030ea8bbf5075cecc6e4f609e3cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74636563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689c3183bb53aec20866d1502e701bdffda7c77cfebd231bd0fdefc84c64f8ad`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:19:01 GMT
ADD file:2546930304b6d429e56e56557d14acb509152fb02a657d195dc0595d0f5a4523 in / 
# Sat, 01 Feb 2020 17:19:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:55:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f9186c7a47276773316addd180b90c065065663e993fe107956ff3f68e5245ad`  
		Last Modified: Sat, 01 Feb 2020 17:28:20 GMT  
		Size: 55.3 MB (55349044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4e183e934f7fe63d5cc430bc444d8bc8d74f0c7a34d5c296a7ec8ed6818544`  
		Last Modified: Sat, 01 Feb 2020 19:22:41 GMT  
		Size: 8.4 MB (8352504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a69e974fc4af43c554b35a2c9f65fd85b3aaa73f605838d1eb693c55f6553a`  
		Last Modified: Sat, 01 Feb 2020 19:22:40 GMT  
		Size: 10.9 MB (10935015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:40b8b5f59607de15faf15ff945c295b68aedaac44b626c5136527042c33ac3b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67931636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688948344922f2a2a771ff5fb69f405e400a30a4cca4b29998acf4ae790779e6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:00 GMT
ADD file:967a85341ab042321428ced1b4d7f5dbdbb8d9f2356b825a4904ac635fd3d22d in / 
# Sat, 01 Feb 2020 16:43:03 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0f7573b6b276747f41f68da62a4262a7441ff49e4c1231d18c674b31be00a6d0`  
		Last Modified: Sat, 01 Feb 2020 16:46:30 GMT  
		Size: 50.2 MB (50192313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08d4727245007c4f9adee1b2b8d19c1edb9dfd3fcee5a9e21f17b775626c570`  
		Last Modified: Sat, 01 Feb 2020 18:05:30 GMT  
		Size: 7.6 MB (7592458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f6008c2ca1d93fb6eade84d84b0c35dcd4e6b6d056df78a2babcda2d74dbc`  
		Last Modified: Sat, 01 Feb 2020 18:05:35 GMT  
		Size: 10.1 MB (10146865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
