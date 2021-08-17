## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:a05af5c4679bd06b9e9f8395fb4afc822653673d9a922b909ba54003df3109c5
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
$ docker pull buildpack-deps@sha256:5d6bc794b03974feb0bca10638255c61d229c30482c16488bf76bd19de3866c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70974998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b61c222380eee70d755288337c14d488c6aaa25dcd184ed039dbaef3fabab8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3d791feb2549b4b03c2e48bcb7d5deb42f1a8752dda92091267f9867edfb81c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68141653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebd6ddbec1219266e98b1930904201cf38f080dc8ab6427e0c39b6fdb448051e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:145f85437ade6ab27652a447c637dcc1efd6d627d69571e89a9a30de68e9ca31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65302676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd861564ad7af9f83d87f0b53feb3deea7080ddbfaed0678f2fc99c2b942ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:95d6d67d8406fecd07f2ca47fb1c181429f99d8aa0fc2ea109f9f7e7ce9e9a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69659445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da9d49ec2b2035e68d98fe9d85208d455692b9c1c6a998f4e214216593a3973`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1fff776b370dd15d9693f26b99eb5780cdcdb3bb8e65edd38597f03b4e64d758
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72519728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddda0428d54281258d8a03082810ed4c348538dc58305c7e6a3471f26fe2df0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9574c023c1bd1d12c66b471db94f95c90303711848b34d1757fad4cf185c6a24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69165997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b353911a5e0986a17337cd29fb8e2c9509b62bfbd1f7a09800bdd6533689a35`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:10:12 GMT
ADD file:21823f99ac9631853baf61992ae48f9aaefd9aa14689bdad76945cbe790d4b23 in / 
# Thu, 22 Jul 2021 00:10:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:46:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:47:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b7674bbd759fec6741d7d94cfebb5e0cf54c599cb2a824313eb96b1d6622a44b`  
		Last Modified: Thu, 22 Jul 2021 00:16:59 GMT  
		Size: 53.2 MB (53162150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bbf92e62547174ba9022d0c0fe12fa84126289620f8148cf33269681b8273c`  
		Last Modified: Thu, 22 Jul 2021 00:57:29 GMT  
		Size: 5.1 MB (5130754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2614779dff3229eb62dc8a974d88a9bf60cfd085721871ad71d642e0517eb35`  
		Last Modified: Thu, 22 Jul 2021 00:57:31 GMT  
		Size: 10.9 MB (10873093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4f884fa29acd285b5b2771d8cc4bce5275b8afc32f27f4bd75703664d0fc3a10
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75903789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f518063b21791802c1bda67dbdbcc4e0499960cdc1d888f032263ba4920d1e48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ea1ea7eb3f215c84403554672c91c22945344400c673d6f1522fd607ee45c612
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65716534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7bd69c97313ca7d402f43854f393547d6854ae7a3b046c650dadf00adab219`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fab97181f913819d52d80648d12308e39e2b6edf93eed0dd25b6269b1e975638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69143422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b34924373ab74ba0650cd2931dacfef322ec14458f9202a4078c99c5f43650a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
