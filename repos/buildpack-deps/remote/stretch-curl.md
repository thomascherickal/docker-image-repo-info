## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:849c71083dec3e7946916267ac6e24f6ee3c3affd5dbdb9e7f100d67bfc5cee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2922844f39d525a99e64a36b3f06d235494d89bc647140f5334bb5cbee8c8212
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60457250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b88eaff333c16c5e76df0b9ed59f2da5d3a8173fd114c4a1eb809039b4851c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:32 GMT
ADD file:a28d8a949b7577768d87fcbac346797fc5f7bad0539625339edcd09a32d6bf77 in / 
# Tue, 04 Aug 2020 15:45:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:35:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:419e7ae5bb1e4875c367f3249b7bb7f8f39dd27dfceb4ee9d6a92191ed1c452f`  
		Last Modified: Tue, 04 Aug 2020 15:52:05 GMT  
		Size: 45.4 MB (45366706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848839e0cd3b3acc96db8a39c4520a40f98dc8f3a2a5f80b575ff4a1c88f1fcf`  
		Last Modified: Tue, 04 Aug 2020 23:42:18 GMT  
		Size: 10.8 MB (10750599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de30e8b35015c7302e071e9c2b449290f270feaf2a419f6466a555b6907e7d72`  
		Last Modified: Tue, 04 Aug 2020 23:42:17 GMT  
		Size: 4.3 MB (4339945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1bc6846b475c0c950671b6ed83fa67e9c232b27a29b0f847ab7fbd8b21b408a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58064680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ba39d4b74ef7fdb7f04fa95986c8951984ed6f7a06d70e72993d0a96e89182`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:23:56 GMT
ADD file:c82979276574ae052b356c92955110dfb283d33659ea097871176d1a62ed98ff in / 
# Tue, 04 Aug 2020 03:24:04 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:30:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8653f8cd9e4c7c5ecd1cd925507522d43ec49dea7127050e56d71d3447f39292`  
		Last Modified: Tue, 04 Aug 2020 03:38:23 GMT  
		Size: 44.1 MB (44081220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04472d0cf19492fee43c5b2d567c58a8db05101bc378a4f87aeb6dbbf7d953b8`  
		Last Modified: Tue, 04 Aug 2020 06:41:42 GMT  
		Size: 9.8 MB (9824577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057d6a311b4078c040c92aa3f3f070583b89400a46547d07c690bedd9bf535f`  
		Last Modified: Tue, 04 Aug 2020 06:41:40 GMT  
		Size: 4.2 MB (4158883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:122c8e6ab63991550d4174e130d380e609b060b060f1bc02704a4bc13e7d7754
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55473753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5650fc4d52de8901d3330de8c2cafe5842d7e34caf2c0c692fa20e0a462eb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:04 GMT
ADD file:0ba6f3203fb10e66124d03088d234e92fc908c572ec7eed268e866623a383a7d in / 
# Tue, 04 Aug 2020 05:01:07 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:16:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:323178d00ec2c5eb5ffb9cb696a52eaf8683dcf2eb605c742da2953556f06e37`  
		Last Modified: Tue, 04 Aug 2020 05:08:40 GMT  
		Size: 42.1 MB (42111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b4e15a79453f6ae10815d79c8f4590aef2f1ac2979c192ff7f1ed0fbf04e60`  
		Last Modified: Tue, 04 Aug 2020 08:30:43 GMT  
		Size: 9.4 MB (9443881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9cb1ef704caf3af8a2ed43dc12884b4f74ac867ce95f60bd8996f51fde770`  
		Last Modified: Tue, 04 Aug 2020 08:30:41 GMT  
		Size: 3.9 MB (3918490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3255b9a593051c9ffa0945dd424b16f7cf0993eaa1a8c13799ca9c3f3c2791ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56967714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83cf7c41b365bdcc582403e117c138c83a482139c690369f92fd9980ea45d8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:23 GMT
ADD file:f74bb8d38ef70a022988428f254630d1f424ed9a3b957687b0cd0f85b9d49e29 in / 
# Wed, 09 Sep 2020 23:54:25 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:35:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b396f138ad78ffceac749b105c676dce568fa15a7b9f2273c2ee13ba023cea1`  
		Last Modified: Thu, 10 Sep 2020 00:01:33 GMT  
		Size: 43.2 MB (43171697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5db606bd1ccd8d11ca18492ee5d5122fdae2e7172ceb0df9cd15dc4d9f3c259`  
		Last Modified: Thu, 10 Sep 2020 00:45:55 GMT  
		Size: 9.7 MB (9700841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd3b5402f1859618a8e455e6bf04a916c8460da1c5f115568ba530c96f6ba3`  
		Last Modified: Thu, 10 Sep 2020 00:45:52 GMT  
		Size: 4.1 MB (4095176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c2362d1b8dd0a0efeb04e88e03de4a5dc224f3713c011e6076d7ba2ca4a59810
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61421774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edabfaf8c8cbf8f7c43f471d1313950016cf8dbe932d9ff61e5a8f0e87b39844`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:59 GMT
ADD file:af30f23f89d9bbdd6ad60199f3d978a5e426835c6138e0c76a3453680945a121 in / 
# Tue, 04 Aug 2020 03:39:59 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:21:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:36eaaca1a8d1677d2d2aa93f595d838e71ccbe4254f548ff566f97e8d555df1c`  
		Last Modified: Tue, 04 Aug 2020 03:45:28 GMT  
		Size: 46.1 MB (46086777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312e98903306441f0b9bd43306e20722d14f9f02f55de10e037f31f8e9887d06`  
		Last Modified: Tue, 04 Aug 2020 08:30:08 GMT  
		Size: 10.8 MB (10773882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fa371da331bdfaab943357b965c1839c24c25c15a78aaa7180325db8fb59ca`  
		Last Modified: Tue, 04 Aug 2020 08:30:06 GMT  
		Size: 4.6 MB (4561115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
