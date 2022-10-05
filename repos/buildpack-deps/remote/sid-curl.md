## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:c738bb54e54f5ad34d9260265bd71d691f5e8f56de0c84177c20ef1cb9d1cf66
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

### `buildpack-deps:sid-curl` - linux; amd64

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

### `buildpack-deps:sid-curl` - linux; arm variant v5

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

### `buildpack-deps:sid-curl` - linux; arm variant v7

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

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

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

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b5b9cce12f09fe605dfcb09f6fe8500023702df50163f827ef19bc9038b7fd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b40f92cafe5909bfee9b18a6b30b1f595e047ddead64f49c8681bb408ffaac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9d75da7404fd11d9c4d9f1cfda7e84d06616c2862585b352ba3d0cb4fd437`  
		Last Modified: Wed, 05 Oct 2022 00:24:14 GMT  
		Size: 9.5 MB (9475965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e558ef32d8acfcaa5f0d607d533c5b5febbb588f2a71986dc1bab69c9a091e65`  
		Last Modified: Wed, 05 Oct 2022 00:24:14 GMT  
		Size: 11.6 MB (11578263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

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

### `buildpack-deps:sid-curl` - linux; ppc64le

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

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4a2fb00746c69ff675e9a4b7c33ca1d49bc7876081e0d523d3d5c0369ce1d8c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d5b08235820d175371883da59a21eef0884d079863088dc9f96c4b6e759832`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:351e6bb97c4530999209dd802fe5783171b732d943ede9e08fbf6bab8088f374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ad3c0b67922fafd3e3d967c69b973cb4d020d9b599305087220c64f1c8fc93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:55 GMT
ADD file:8280bb7f6237b831709e5dfd56222a9c3d008ae3b174b51b6b08872b0c95265d in / 
# Tue, 04 Oct 2022 23:42:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:404349a84514468a0bbf4e37aaf50d49282c5496638b7e2599fa70e9472a0fbe`  
		Last Modified: Tue, 04 Oct 2022 23:47:33 GMT  
		Size: 51.1 MB (51096269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f66e3c468d6d9450e7350c47bd350eef8a8bbc581e0ea5e2e4ff1452f62f629`  
		Last Modified: Wed, 05 Oct 2022 00:33:11 GMT  
		Size: 8.9 MB (8938119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6880a5b72798c50be5ca11b4b2c503df48724317991d3f9df84b880ee1e227`  
		Last Modified: Wed, 05 Oct 2022 00:33:11 GMT  
		Size: 11.2 MB (11244096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
