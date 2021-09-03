## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:160fb6732d0c7e61ee4d351ced056fb9a48cacb5d55b57a436d60b8f4526e88e
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

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9f458071c07c1922362c241070e5e92fcae56e600b5fba756c6c7f016a7b8dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68653424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e3b381e72d26f967883d0038a368254c7a7d6c8a34171e0360b55d6a190f08`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

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

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

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

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:172f86014cfd23f8534f1d81a96c73a480f0fcf8f38814951938b8646bc3cf67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73100008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ceb13982ea1259ee29ad6b3ac68115fee570615ace45461936af7d9edd4e5f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0742b4ef0a1e6d36f6a1baf7431d7ce25444bf9575509f0ba031b8b243cf1251
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70167872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fac613c7b4b40ce813d10d55b6b0ad58587ca17e308844e5aa980796ab1392f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

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

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bedca7b6c6375e09dd1ffb3eec3b607a8b8b9a15dd142b77525579bde87a41b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66588742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183f6c97e7e26c4086f4b6cb32c3908d6b090e56eab64119950c4a699dca29b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:91057d86526bc5e96ff66eeb074c812f9321e33bef9d4b0ced773e1083ae997c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69717090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66bb7f34fb2e0b2a3dd65188ea09c38f4c42f4f90fe3d73d760f0816a9dde63b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
