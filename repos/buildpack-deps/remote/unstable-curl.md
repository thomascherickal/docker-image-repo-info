## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:92772d5257e595421a91f1f43c5353085ed31a8bc6ab5c18ce065312a79b0ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cc22c156446c9313c4680623e26c6e48bba2f98ec6ce87c8ed3a0d52e716c0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73367169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8c38f75980c2def43a2d61e770ccc0b3c9955ae57c722bb79d7f977a21e31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6d4954538c468e745a487851cb44a6cceee8be373e805c22bd384678992c8a39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72339574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5de3670778fe98accb2c7d82cff835e13b367e2d981e9b6d033403159e07eec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:23 GMT
ADD file:5da40917ed11781002a72811aeac4336d50b3100f4e25213b5b18cb733468d31 in / 
# Tue, 04 Oct 2022 23:49:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:19:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:19:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f013d31fa02ab56c7186e21477e4fd559e7e9de70eb511ed30a523990b759421`  
		Last Modified: Tue, 04 Oct 2022 23:54:20 GMT  
		Size: 51.6 MB (51568969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f385ca45e727337dc6e057766a57c9badc26c5e75234bf0aae01ff5692ac8674`  
		Last Modified: Wed, 05 Oct 2022 00:25:04 GMT  
		Size: 9.7 MB (9739988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b50d6779e58a2088ad2ca98253c952ea1e71f4dd19953b82651ee27cd45794`  
		Last Modified: Wed, 05 Oct 2022 00:25:04 GMT  
		Size: 11.0 MB (11030617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67e81d32e4a379ebc001840f12d827e5f67833629cc8d825dc7e62681fdec972
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead5cdfb9f5e5c275759c55be9d11eb1dc155f3aa55dad5b5be0cb66efd70376`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4571ecef8762e4a8bc6310bbadffc5b7d34becdff5cf8be7b450b7c5805cd2df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72965627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efdc59fbf88b4af5a8031ed4caaddc0726357acdc036ee20c3b8fa26c9c4e3ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:25:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:26:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd5d318557d24479e128b2af516b73eb0b625f59fb7ac36f3a3e2b978ee3b51`  
		Last Modified: Wed, 05 Oct 2022 00:39:42 GMT  
		Size: 9.1 MB (9129572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba060498e8e695e4806f18c967a447d15dba20c396936934e95db6995a21549`  
		Last Modified: Wed, 05 Oct 2022 00:39:42 GMT  
		Size: 11.1 MB (11136064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7a92edc5d0d1d9b005fc402881b8f8eddac8e13c8f5adf57fb62e1a26d00983d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72287451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1893a81cbf84a850be47ff4f28e1dd4035b9c2256bdedf86584fb4079c771d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:177c731ad458bb98287f9b7f0ff300408fc1a53c32e1d406bb638c4c00719d21
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d48d0070c45b656746927bfe7b8ec4a82c7b00acdd9cce150d2c20e17feb87`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f0fd4ab9d4da3b6fa3a8000cb9481cf35e68b38ff3471abe82967ab413c3d9b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78816852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df175a7c6922a086c362aa53ec99b3cc113f66535939a6fae9ae4b4bb482c030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:23 GMT
ADD file:9a1fd28de3c910076975890aa736e3f3bbff1b433c668f4121cf52af264cd06b in / 
# Tue, 04 Oct 2022 23:18:26 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a99fd400e2fbb8830bde6fd270def7df44ad1a841ec4e7cb5f33d7f5661d181a`  
		Last Modified: Tue, 04 Oct 2022 23:24:45 GMT  
		Size: 56.8 MB (56786765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d06bb7b49d3eb3a82cbdff85d58cb0731d3d80785b0934f25001bf5bd3fbf`  
		Last Modified: Wed, 05 Oct 2022 00:06:08 GMT  
		Size: 9.9 MB (9885071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e5e780a2b80f3c4caf46c625dd63314a82efa8edc7f5d9d6442a7edb4905aa`  
		Last Modified: Wed, 05 Oct 2022 00:06:08 GMT  
		Size: 12.1 MB (12145016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:91c41397454a62656ddc234f54c6ce9bc6eebb7463198b379aec9760ef9f5ce3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67996548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c82f669a88d6376397cb790855001ce2a2328184d9fc8f1fbf316b588cd40e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:459e259ac9d973e273d44f4977a901a7c57dce7f749c5caf0ade7837350bf940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68792946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8919e63d46a3758bb8046627e26a7d852ed8e26e8b044f56948b519863d33fd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
