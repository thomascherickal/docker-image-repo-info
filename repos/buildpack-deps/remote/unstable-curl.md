## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:cd6017fd6da5c8c3a1485da7bc8fc505a08da6e406619edef1c5c0a9d4be6824
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:147ac244dcf0ee76cea1a8c302e2a3401f6b1cc750b1d35487292c8152e1a3b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70920002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22294fd9b52d4f51ccbeabbaf08feb69f47f1eb59be80155ba467b98a3834a2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:57 GMT
ADD file:97b8c276224b2b9407a1635d61780b968f86726642a00f3d49298ab19e9ea714 in / 
# Sat, 10 Apr 2021 01:20:57 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:55:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:55:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9097f35530b77dcae85a27364a3301e3362adb2860367422ed06b99fabe94b8b`  
		Last Modified: Sat, 10 Apr 2021 01:26:23 GMT  
		Size: 54.9 MB (54881626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4657bb2202fe6d13371845dabecbb1843dc3e9ab3d45afba017280a24f40`  
		Last Modified: Sat, 10 Apr 2021 02:03:17 GMT  
		Size: 5.2 MB (5169536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a456d1fa6a4d732964fc57896f119a9e85d6cae028f4deffc62729e23624641c`  
		Last Modified: Sat, 10 Apr 2021 02:03:18 GMT  
		Size: 10.9 MB (10868840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8a120eea3b841c2fc6392d38db6f498acf085b987bd2c674153a8d2b09dfe484
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68058777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91727bd35dd4ecc99fd2c0d74f24f443d9554503afa686251fc3c4821133801f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:52:44 GMT
ADD file:9bdb85e8b11f9d011901b496376920ceaf2a43e4dd9f7dce303f362c5cd9847b in / 
# Sat, 10 Apr 2021 00:52:52 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84ee0e585c798c84e07ba41f87e072c0fb43795cb12e325a126f9026f876059c`  
		Last Modified: Sat, 10 Apr 2021 01:00:27 GMT  
		Size: 52.4 MB (52414024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f91ce0c40daeff87428c76fc2b11803ad6153af50d86ab3e84d37fb8ad8ca7`  
		Last Modified: Sat, 10 Apr 2021 02:20:41 GMT  
		Size: 5.1 MB (5074282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126b0b2e172136e012642af22312fd73d761d735f0990caf91f35b6f294fb88`  
		Last Modified: Sat, 10 Apr 2021 02:20:39 GMT  
		Size: 10.6 MB (10570471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b8f7b5b436096f185a90340087617addbfa9e70b7442d497fdbd218f126f0788
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65223551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:862f6183aa2f7e335540fc44a1a1cac010a6aebf1f7d1754653b3d1eaee8f3b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:09:57 GMT
ADD file:3c49310ff7c2a9c21073b7ca0884f4b8e783606a6653a2d74d1aa04196a3ed8f in / 
# Tue, 30 Mar 2021 23:10:01 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:25:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:26:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f41ab33290e85402afe03e9a82d0262689d71eccbba0d79246595731d24f2688`  
		Last Modified: Tue, 30 Mar 2021 23:17:34 GMT  
		Size: 50.1 MB (50070962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d173ac9612777e7e6d56bd74819357eb0a74fdd29dd54af742a5652ae5ac6d`  
		Last Modified: Wed, 31 Mar 2021 01:38:18 GMT  
		Size: 4.9 MB (4934354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b41bd459aeb849bf22b88bf2563aeffb2527f25a09c92049467c43605bdc30`  
		Last Modified: Wed, 31 Mar 2021 01:38:16 GMT  
		Size: 10.2 MB (10218235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:aaee5e83bdb0f365342f3f062a636eca92d811c8ea8b6d4b761d3445660e008b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69594572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb29fc43c5f15ecc2e7866dd945255f28b32403297bfde4a3cb3905e9c51853`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:30 GMT
ADD file:6bd461aca61a6c4468971e152cdd2158ba47c56a30fedd2560ab69bc0d5429d0 in / 
# Sat, 10 Apr 2021 00:42:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:50:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e4d191ad9b976ffe4d9719cf4d8241d751e0870f7abf4ded747f4258cce757b2`  
		Last Modified: Sat, 10 Apr 2021 00:48:46 GMT  
		Size: 53.6 MB (53568143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779dd445520bcb3f8ff73ed0cfdf91d218d8c0272557c8e2959626d83c1e6cb`  
		Last Modified: Sat, 10 Apr 2021 02:02:23 GMT  
		Size: 5.2 MB (5157782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c386828fc4d261064c2034ef6ea283e4de5534b6dc52e8f7dd4d4cb671677`  
		Last Modified: Sat, 10 Apr 2021 02:02:24 GMT  
		Size: 10.9 MB (10868647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f93786f5e22f1a574b3c98c29d7140e86e06f3bb0e2412e7f8d03f305f4e1b58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72438979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a89d937930465e0ffe7e72fb4170324bf77a1679bd04815093db030f2f9078`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:23 GMT
ADD file:e8f1dc678a4622b7caa83d305ed03d778d1fd4b248d1217382e32f2b6e88b87f in / 
# Sat, 10 Apr 2021 00:40:24 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:19:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:20:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4b3e9fd2b852472b6f69da429722bff4b757f5da21d5bbda36f776b73d788c39`  
		Last Modified: Sat, 10 Apr 2021 00:47:25 GMT  
		Size: 55.9 MB (55891041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db588734c7a8e3da8896097246345eb23edcb4069f24b1a38de4542876f761`  
		Last Modified: Sat, 10 Apr 2021 03:32:16 GMT  
		Size: 5.3 MB (5298882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb805f0843d55104ade8cf43636ecbace50cec91d8361219a4ccd38dc91cb756`  
		Last Modified: Sat, 10 Apr 2021 03:32:17 GMT  
		Size: 11.2 MB (11249056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:329bb2e591a67f5e47299211a063a94438ae280a89ca1e894947c2812d782972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69138062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31db54519c9a1182343e5c7774be9287685cc215a3b167259c2654b9f906b5da`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:10:06 GMT
ADD file:a0cb4c0af6dee6c99c3739fc2b27a4d60df79591342d18fd79bb4e38a25d28d5 in / 
# Sat, 10 Apr 2021 01:10:07 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:11:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6eda60e328d687e0091fed92ed18129ac8eeed03d72dd92f7941c847f05a6dfa`  
		Last Modified: Sat, 10 Apr 2021 01:17:00 GMT  
		Size: 53.1 MB (53138256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b35bc44f5e1748a146c217ae7f8eeb19f129f8171afdfb72f50c2e672425aa`  
		Last Modified: Sat, 10 Apr 2021 02:22:09 GMT  
		Size: 5.1 MB (5128904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290332c458e552d3d40e8db4b52e91c80f460edf5da9ee4bd9e86668fe97738`  
		Last Modified: Sat, 10 Apr 2021 02:22:12 GMT  
		Size: 10.9 MB (10870902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dfe048de582cc5a1dd0f1c14efeca12c506af5d0d9b90f6ba8c0e6726003f573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75819119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337af443a6b5a399a1f993f55cf09d5a0154cceb47112574066aa40048b87442`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:27:11 GMT
ADD file:a41b62f9bc6147a0ab13a91e4ce5169739d220f716dc3752d7c872c9bf22748b in / 
# Sat, 10 Apr 2021 01:27:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:47:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:48:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:907e6a464bad63c32df38aaa0e848e3e09634237527afb1f8728bda2038576ed`  
		Last Modified: Sat, 10 Apr 2021 01:34:23 GMT  
		Size: 58.8 MB (58777775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d1d0df065cb2c84ba66e763425b139d7dc18eb050bf8cc5cb8dca7e25ac80b`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 5.4 MB (5420160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebdfc94479ccc35bbc35f2da43ced87239a8ca75ef23ce43d8dd981eab17c3a`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 11.6 MB (11621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fca010e2397f8a38f4c2b041fada4aed2461ac5146f1439f6dfd10d825f279c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69065284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8cb14d4ba367ebfb04b4284d75ac51cf5e6f7b82e6e76f058050b7822e80cc5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:33 GMT
ADD file:95fd1353430dde759ab86e64384180601d2eec1359d5a81ebeb58e17b8998353 in / 
# Sat, 10 Apr 2021 00:42:36 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1b22aeeaee0a7589a5b67e1a3571ce4d1a0942461ff2075b104514fa1967711d`  
		Last Modified: Sat, 10 Apr 2021 00:46:02 GMT  
		Size: 53.2 MB (53155408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9ca0514c5f0614720863667ddd96ff334dce5555e8ae2112bed88bfa4c6711`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 5.2 MB (5151136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe0daca911ede51529950150d6623adb8cf7f5d56b37a6dcb3e07ee55232054`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 10.8 MB (10758740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
