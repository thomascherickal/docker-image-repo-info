## `buildpack-deps:groovy-curl`

```console
$ docker pull buildpack-deps@sha256:616b272ded42c7208911081efed5edd9c30941fbcf6f149d58d9c151f69f312e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f0b2e0716a3d61005ef197e0ee3076617a85d83317743df8be59f22492a333bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40409348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d37f93daa64c8bddf66502925abb561e68e4fa5151e53627b71fabac8f09c16`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:31:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a187db8c68613bb56c28a4f1c711d24248f3be342e2b2e98c6d162d37b9286c2`  
		Last Modified: Tue, 13 Jul 2021 23:46:40 GMT  
		Size: 5.4 MB (5404370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd548091a4b68a282f178caf8f237861b35ad281d3b8408ad339223262a181`  
		Last Modified: Tue, 13 Jul 2021 23:46:39 GMT  
		Size: 3.7 MB (3663412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7536ccc1f755d8778266098ea95e4d657b401a554760debed405369e1c5ac3a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34293734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0601093a516c81d72db6edc44b40ba9ae8de46ed66ea5f297250ae4ef34b9bf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:33 GMT
ADD file:80b5f21ffac906a8416f39204cb526afaf64f15559123cb3a8fb311e312a703f in / 
# Tue, 13 Jul 2021 23:21:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:55:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7ad80ac50e31c20115b0366841c81a92d1916a7f2113255fe1125324250475e7`  
		Last Modified: Tue, 13 Jul 2021 23:26:54 GMT  
		Size: 26.3 MB (26312397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87836ed84bb5f0e1d7b61439e8458826efce0a52158d32f928c2efc41367ac4`  
		Last Modified: Wed, 14 Jul 2021 02:19:01 GMT  
		Size: 4.8 MB (4840704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a0657bf22de96a1925b7c31d415ed9eff49f3b00971444459ee9b696832ef`  
		Last Modified: Wed, 14 Jul 2021 02:18:59 GMT  
		Size: 3.1 MB (3140633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a27a6457e1fcbb6289b44a780596c486da13f26b759c4c4c6faef263f9eccb9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38885224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c2f30a170191f17451a2019aa83e410ef0ef262e9e094a589c7a7673f73ed4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:34 GMT
ADD file:8fe3c90118921d388c31ca28a21ff713dd718197e04654c6e0b7a09435f5287d in / 
# Tue, 13 Jul 2021 23:01:35 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:53:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:53:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3da8512ba050381848a454507530b9a467063e06b22a25eddc01311dbdf35301`  
		Last Modified: Tue, 13 Jul 2021 23:03:58 GMT  
		Size: 29.9 MB (29877377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055ca1e90e094916911d8a92553fa0422dd53e6e43fed33614623edae8ca22c9`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 5.4 MB (5372770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955901556b2298b0b4c51d2c60f4312309d050d4152c6e9cbf8a27cc02b9357d`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 3.6 MB (3635077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d783add69d2804fe48bd463685ef867ddf1092dae7a72b456fbf651c912f286c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47125494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1786ea2c6d7caab11adaf79a4e4339f0da55a88538c8237b8838f61a885d8d85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:45 GMT
ADD file:d810eebdcea73da6a0b9c4546fc356b13b60da24827c29923375b8e08f2195b4 in / 
# Tue, 13 Jul 2021 23:22:53 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:30:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:97b0da8da7b9eb227e28852cb467ba3f76ac379708648200f035c072d3bbf4eb`  
		Last Modified: Tue, 13 Jul 2021 23:28:00 GMT  
		Size: 36.6 MB (36562496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19019a66a1c7600fb2159a63b0e68f36b9d9f55e9e56ae7b70139ac7565616c1`  
		Last Modified: Wed, 14 Jul 2021 03:24:17 GMT  
		Size: 6.0 MB (6040945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e113d40008d7a4f01ffb65b6bee553ec1af6ea5935387bfc2677d6a9888ba`  
		Last Modified: Wed, 14 Jul 2021 03:24:01 GMT  
		Size: 4.5 MB (4522053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4ef55d3db45697231ae33a7f544d7106782c08f999176b342bec9b0005255213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41364083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d55d2cb61d52ec89734ffc764835af769003de9c3074e699e5068e5ec8a464`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:46 GMT
ADD file:02a1c687ec9417cdf601518590b3a21fe31a0ebd2cdeb9bc63792512b95de989 in / 
# Tue, 13 Jul 2021 22:53:49 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:44:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:412af85569a706b682c00eeeaf32aeacbe1a5df158e5b67ddff07842b7ba3080`  
		Last Modified: Tue, 13 Jul 2021 22:56:02 GMT  
		Size: 31.6 MB (31577497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ed9de239c255124abaa7cd10a81a3e295829e47c8f990a740c9de4638d328e`  
		Last Modified: Tue, 13 Jul 2021 23:52:18 GMT  
		Size: 5.6 MB (5629821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612d9fc542d056eb20ee90480c45cf9b38afd821365ceecc6ce517204872126`  
		Last Modified: Tue, 13 Jul 2021 23:52:17 GMT  
		Size: 4.2 MB (4156765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
