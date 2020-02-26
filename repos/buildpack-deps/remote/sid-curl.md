## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:c21dda5512891d72d8f23d14a53e273868ef29a8bad2bde96b440d4f788867e4
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
$ docker pull buildpack-deps@sha256:75370b107b116d7c4e8ba71d5c09afbafe0f0d17bf3514e73bf36ed4aced2bf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70035499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4612f747713456c5691f382594eef42af7b4701540a3a3e726fe540c7247b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:40:05 GMT
ADD file:bec180e92743e5024fcf273019085a4de227f49fe65e76828b9c7f740fafacce in / 
# Wed, 26 Feb 2020 00:40:05 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:15:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:15:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8ea0d19362f06fe2b59b222ce913ba48c67c375897c1011c35ae714403602dae`  
		Last Modified: Wed, 26 Feb 2020 00:46:06 GMT  
		Size: 51.9 MB (51852485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2dd00a16259f5ef437d658e1c9a35286e86c1b1e57ee707e76e7f633f9addcf`  
		Last Modified: Wed, 26 Feb 2020 01:22:25 GMT  
		Size: 7.9 MB (7923560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd95542fd67b65c74ba330b9fbc3a0338708e71af91f677f4c837e08e89f590c`  
		Last Modified: Wed, 26 Feb 2020 01:22:25 GMT  
		Size: 10.3 MB (10259454 bytes)  
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
$ docker pull buildpack-deps@sha256:9b473de0976fa6b4ec77bdc5e52d70745d88ed0ff7065d80f0606ab5c3f605b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64464718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99d2cdc9a34935f2b2bc7ebaafab56f0969b41c3d97a4c14e71729a446bf039`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:56:58 GMT
ADD file:30aa400682ef7dfcd135a9f9a7ce18e83290a6cfc96893e530b1601d79691bd2 in / 
# Wed, 26 Feb 2020 00:57:02 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:22:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7565e2c5d4e7edc07eae55400f5a90bb7e3cbadf4008fb3f77acfcb3c9cf3cdf`  
		Last Modified: Wed, 26 Feb 2020 01:10:06 GMT  
		Size: 47.6 MB (47586966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41118136e87d29bef0a68251f8642bb1356a3d2e3f47a2f27be5762226d865a7`  
		Last Modified: Wed, 26 Feb 2020 02:36:03 GMT  
		Size: 7.2 MB (7238491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1fe1d11ac7f4f8e86fd0b1041300173ac89c0fbb2ff4d8a7d84c5ac366cf5b`  
		Last Modified: Wed, 26 Feb 2020 02:36:03 GMT  
		Size: 9.6 MB (9639261 bytes)  
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
$ docker pull buildpack-deps@sha256:9045131b2f67d7db54106a9794af988263480fbfb879df6aabef6ae9c60eaa6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71726340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b37692a0c70dd5d2001cedc814f9b672e6550de99ba798717c6f596ab3d33e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:34:15 GMT
ADD file:527aa2259b2366e4270d004b42a2eeebcb49adafed28b5a8e91d2e1eeb66191a in / 
# Wed, 26 Feb 2020 00:34:16 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:21:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:21:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:00a1553babb601009b2783a2a5321157baa25a79030b9f4ec05a591f0ab4dc19`  
		Last Modified: Wed, 26 Feb 2020 00:40:36 GMT  
		Size: 53.0 MB (52999556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dcfea1de6377d5d7b7f4a8dd9386ef6919ed23af5811eca5c9cd495f45c97b`  
		Last Modified: Wed, 26 Feb 2020 01:29:48 GMT  
		Size: 8.1 MB (8103631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6adb539590202db492bc8bd3bc0c15f73c1afdfc2c040ace64c75cb8cfa048e`  
		Last Modified: Wed, 26 Feb 2020 01:29:47 GMT  
		Size: 10.6 MB (10623153 bytes)  
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
