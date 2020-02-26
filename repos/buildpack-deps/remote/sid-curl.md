## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:23a523a6ba12e2945a54e8c588262fb974c5ae72042c74c8b55f10227e064537
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
$ docker pull buildpack-deps@sha256:3e04457d160417ed5b84d9bcc8bd27638a9efae98e4363fcb872ec6af9ce60ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67331268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41493ca79b5f5a37cfbe4e2830cca7adbc0f608da2685e7b2867bc8fdfcbab7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:40 GMT
ADD file:6f5d17638043fb7ef05ca0f1c1d20b54cc5e6b65f1c56dddffa5c9b9a0c499d8 in / 
# Wed, 26 Feb 2020 00:50:49 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:48:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:49:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cc5a3f6ff999f547ce2337a1307b1bdd7bc19f327358e69994e1d288b2e95aa`  
		Last Modified: Wed, 26 Feb 2020 01:02:02 GMT  
		Size: 49.9 MB (49854601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c3c5021d94167dd69f630d803a6d0eced6e577ad4645c38b09339ae8699386`  
		Last Modified: Wed, 26 Feb 2020 04:03:55 GMT  
		Size: 7.5 MB (7501600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3042081863acbc3c403980506dacbfb08207c794e8dca78c7aec29e279d805c9`  
		Last Modified: Wed, 26 Feb 2020 04:03:56 GMT  
		Size: 10.0 MB (9975067 bytes)  
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
$ docker pull buildpack-deps@sha256:2412dfc45b4de4df93f27c61fe89d75d45bff581845a5f71e83df66dd56d425b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68878452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:082114cf0f4f2c2ebed027129e4e98be476b66ed622aac665994bdb78670d77e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:48:15 GMT
ADD file:dd5929937313448ee9b3d8640f7868a744a021a2795207ffb95b84e16f7af7f3 in / 
# Wed, 26 Feb 2020 00:48:20 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:55:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:55:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:39684676301c5f1b4bd75510ba0132ffcf4cb0d41ee99702ffef900f06db4fe3`  
		Last Modified: Wed, 26 Feb 2020 00:57:14 GMT  
		Size: 50.8 MB (50825108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27a4d3ca3fe90120d925f3e4e10e613078f4130d5ce9a4dab2addbab99a69d3`  
		Last Modified: Wed, 26 Feb 2020 04:07:00 GMT  
		Size: 7.8 MB (7799823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273e8497f8b87f730468a98640fb9e0328f1d1eefcbe99c52ca4815168f8d8d0`  
		Last Modified: Wed, 26 Feb 2020 04:07:01 GMT  
		Size: 10.3 MB (10253521 bytes)  
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
