## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:f2e2e7c5e0aefcb6ee3c03701e168cde380e414020ef2e32daa0951840759745
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3e75b6558a382b83b04ec635c9d3335e9c48844ea8f2e8f2b7d15b23eb1a5a71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71031932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6beca0094908803d0ead07acc19cc3113044ccf91cf73938ea957a3bf40f1258`
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

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c036eca1b1f2a7b83aadac74b895a527d7ac7de347c09e1099ac6482b588a881
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68176009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d1a0be2a8922913044c0651ee883f2d8b099579f5842692224186fccd2a5c5`
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

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:abc61dbd232dc248a1264d91399bdf8bcd14ed264350677525db2ebd5cffce5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65337683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32835625c8ab09947b1fa7fce5a27e68377bc59fcf3f534211541dd6202722f2`
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

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ebf5459a2b07f5147e78d8312003a2b97b7ec54f962474380e90260fd9eba93f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69483589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc960316ea3b85073ead675fcf9fdcf79d6d8cd78d74ec05965d22248ef0f7d8`
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

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1e03123ed59286e20cebaac0bc93947931d309fb98b65ff719ed7083f6a5f3bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72319619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90692fb9a0cf48495925582f258911ab8be9664185ffcc59ade82fbdba07f268`
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

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:03c50807bf790f7b9da342df4b3ea9f00e07292f31238decc2a750b5fd696b65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69041344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b27350edf3aa48403d7b865c24a9c1ab51eb2033224e9d8547e07d93586f15d`
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

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:01a1a9c8e98ef67f86716961120b8855a790509ab188fc0ee1a238f272c48498
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75929435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b654a208f54b23d372793f06baa16f98cc357209415bf70d189cb2beff14659`
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

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:18aec7e5bbf67c3e414fcf9498294a318e1ee897bce3489504700f1f9b9224c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69175815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032674a9e9ac6cb49b4fc8fea7e16829d1eb53713a091953c07db784278620d4`
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
