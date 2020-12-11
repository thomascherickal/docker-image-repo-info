## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:619f17b6add805758b2f5d31124d5d58a11995905d36457c1103f9a083b3c89f
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

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:64d6de9a9db943893c0f0d5042009b45509d09854a3a1eec2bf7f939aca033af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68205675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744c73c6a4c0aa153eed16df0c8df8433d9d536ba8df1ec5c875cab819ee54fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:30:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77915b4e630d47296770ce4cf481894885978072432456615172af463433cc5`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 7.8 MB (7811717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37a0a41b6b03489dd7de0aa2a79e369fd8b219bbc36b52f3f9790dc128e74b`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 10.0 MB (9996233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ee54138871f12977441370ce2371d2d5a5d34ec9c64b4cfb64567b7bb0567d4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65160719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37c5b1a068c8a9576bf19d0eea1cb33079f7bfe70cb67c1ce26b3d5c9cc49cd2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:16 GMT
ADD file:955829a14d270d20f9903754a57858fd2dbe3bcf8845491c1cdccae1e4896249 in / 
# Fri, 11 Dec 2020 02:04:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:45:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d0f09cc3b3e26671eb372263913148f5c37e856980aa747129a90a3e14610461`  
		Last Modified: Fri, 11 Dec 2020 02:14:15 GMT  
		Size: 48.1 MB (48110951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6dfd2752660733cb28140557883aebafb300f8d5feb54cd866371882826509`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 7.4 MB (7362304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70af9e49905885803a3a9fb626687874b912388320ca5bc2ab1f9ee2576787f1`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 9.7 MB (9687464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a737b957fb94f8df70b4111e14bd44481fef3b216fa0eab7a3de998b27131be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62309768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:322433ead2733fb0b9d42dbb93a1eab6c0955a39a39173e48bead07c21d09ef8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:30 GMT
ADD file:81141d8fa450e1e5af67bb3757057f3fc34d3ed35cfd0caedb0aab64c5da9aaf in / 
# Tue, 17 Nov 2020 20:20:33 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:41:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:41:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ebde10b2510128140d24e66909ceb0c80e00656af313829f82d31ae8cf08bcf8`  
		Last Modified: Tue, 17 Nov 2020 20:31:13 GMT  
		Size: 45.9 MB (45868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05478d2a9ec4daaef33a6c87d057451c262677d02e4d9c61125bbb68bc56a601`  
		Last Modified: Tue, 17 Nov 2020 22:07:16 GMT  
		Size: 7.1 MB (7098267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5f002cc82f5d62a78100714f451edb33a717fbf6795e309e0b1768712c093`  
		Last Modified: Tue, 17 Nov 2020 22:07:17 GMT  
		Size: 9.3 MB (9343289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cd2564311a38fc2fbf1ad424b3b5dd86e7801f1658916cebec6c186b36f28285
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66845056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24526066574dba30b46bf4fb15fe968d10a45b2dae2f4a19df706a9b82c688ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:04 GMT
ADD file:28343d2066831f0ffb2002914f158698f92b4af6dc16ac22e3d8e9c388c688bb in / 
# Tue, 17 Nov 2020 20:23:05 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:20:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:22518ad4a7da48a5acd01946dad2fbee99e4fca910d23b78cd7e4a16c3bd1e5b`  
		Last Modified: Tue, 17 Nov 2020 20:31:35 GMT  
		Size: 49.2 MB (49179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ed68dbf09ea059b44b3e1013706c78f868e5f07beb5f16780ca8f52aa9594a`  
		Last Modified: Tue, 17 Nov 2020 22:36:39 GMT  
		Size: 7.7 MB (7681805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeb09cb5ac2e2a9553920a21389f08df1b6b08c816ae4b8e60866d84119492`  
		Last Modified: Tue, 17 Nov 2020 22:36:38 GMT  
		Size: 10.0 MB (9984036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:cb1e350dadb3c8d09e257dc9a34b596f134476c1fecf3d04851d939c13b5a2a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69479221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18b2b2970a8f6f92308e5864750a34538651332f04ab7e96f830c525a775e8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:39 GMT
ADD file:4805e11ec22df9454eb4759523111e031e84c8078bcaef178f089baca9e83cdb in / 
# Tue, 17 Nov 2020 20:19:40 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21c39c42a8e082b1b164b44e463e4752c74821dbc51451f2ac2518ae6f29dff3`  
		Last Modified: Tue, 17 Nov 2020 20:26:25 GMT  
		Size: 51.2 MB (51159492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afab7b21aa8cddd140983ed21a34965621db1efb35f635bc756479b30c3deaf3`  
		Last Modified: Tue, 17 Nov 2020 21:23:47 GMT  
		Size: 8.0 MB (7981231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a1ce1fcda982662c6c9be38bac7b53e9fd405b0b367fa902cfd957be683731`  
		Last Modified: Tue, 17 Nov 2020 21:23:46 GMT  
		Size: 10.3 MB (10338498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2888a6c726ad4b7d6f6b4c1696a3d2a470bda59a93e7edbf59aff77b35107b81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66271005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0145d8ebfab83b74300dcd069932a0bd272b396d9499bd65826b4909a114c9cc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:06 GMT
ADD file:de28e706af92bb73003a6ea1969c51666f52e0cd0286cbd99c624f3bc49e4666 in / 
# Fri, 11 Dec 2020 02:03:07 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6057d98f1b0dc943648ced0ad33983792fadf9f1b0eaac90fd62165829122340`  
		Last Modified: Fri, 11 Dec 2020 02:09:27 GMT  
		Size: 49.0 MB (49022625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e90ff301a3d0d856fb4e7e6911036aa68b68b2c71f3be423ef654b42f0be98`  
		Last Modified: Fri, 11 Dec 2020 03:02:19 GMT  
		Size: 7.2 MB (7232151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9b5cb9bd92be17ad45be69b85a627b3fc368a8486765bd25f83e7916c0484`  
		Last Modified: Fri, 11 Dec 2020 03:02:18 GMT  
		Size: 10.0 MB (10016229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f1fcd58dcced68dfaaf27f8c720d9c9aee7bb75a1d7a1553712866cee4ecabcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73125826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bbc4ddc1ebf81026e781d1686a6c5a21dde75672b8fdc1bfb372079193a15c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:22:28 GMT
ADD file:b5112ae3b22de1d8a373191ad01151a6c1cdde605887b1836672be39787e2213 in / 
# Tue, 17 Nov 2020 23:22:37 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:55:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:57:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:94e00adb98ff1f971add74025ff2a8ca87e003568d828bdb0df26ecd46c269a2`  
		Last Modified: Tue, 17 Nov 2020 23:31:43 GMT  
		Size: 54.1 MB (54143125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46d858a6e31a5aa25fd9c527cdee95fe08fc11f45038212d1c5c7e52dc7b40`  
		Last Modified: Wed, 18 Nov 2020 01:53:05 GMT  
		Size: 8.3 MB (8255326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfab907b4d9fde9fb35f17a366b653e709c31cbce8602a2ae23c23d39524820`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 10.7 MB (10727375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e8809e19d91aeb0d17f04154860320f3ac86964b3a0bc9aff369de83d2379d29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66236484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fb1dd6ff683d8b1f7a85c3d33d978e00ce3c8951ef6f1cb4c9942f1d07ad8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:17:56 GMT
ADD file:dfb1d2f775a9c4493397d0ca05aa6486393c6dad4f0fb5f48ffd209397301bdb in / 
# Tue, 17 Nov 2020 20:18:05 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:32:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:32:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e95a7d20e6bbf957d2bb5912f19784daba6953d8afac5562453108dd45940e1`  
		Last Modified: Tue, 17 Nov 2020 20:23:18 GMT  
		Size: 49.0 MB (48968246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab56d289be912cd903623a00b35bdc52f4f1b54a6778c1ba4c076e5cfe339aa5`  
		Last Modified: Tue, 17 Nov 2020 21:48:36 GMT  
		Size: 7.4 MB (7385996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29ee109f7efbe0700da6e225717912b22d8e015d8d9a9968e564419b1ba97a3`  
		Last Modified: Tue, 17 Nov 2020 21:48:36 GMT  
		Size: 9.9 MB (9882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
