## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:2bfb7f355a43610d50e6e949e0a84214f4f3098235cbe0d13a10b2b8b35c553e
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
$ docker pull buildpack-deps@sha256:71b8a153f306df2c53e4a7b244024f2788be4041819651a41b8e0042e7ac7d0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71080900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a11fcfa73b1d118a0ca6cf6e30a8799442473a865a4c1aace11091fc587793`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b3e52685cb7d6a58850247d639960d7a6c7969e8e0621e1a42ac63ceb79f0743
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68188869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07df827da1b57f4c05a008bc9398949fcb696e9e1c729beab2f4511494e3e209`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:01 GMT
ADD file:1301cc1a3eec72236eb8cfb02c81a3e956e32a32025a89995435b641e1d9330d in / 
# Tue, 15 Nov 2022 01:49:02 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:42:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0655cdb20ead0094190060645bdf853e9427b58a64f0c7d92ae439b80ca81fdf`  
		Last Modified: Tue, 15 Nov 2022 01:53:55 GMT  
		Size: 52.5 MB (52542295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb37740fe3185bdb0707209ff5ad54853d540c2a95c40ae3d998c9d4dcbe26`  
		Last Modified: Tue, 15 Nov 2022 05:48:21 GMT  
		Size: 5.1 MB (5072242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce25a37fc4ddb3f5200d17fea7e9ac780e294a18828ae0381ccb9c923c0d0f4f`  
		Last Modified: Tue, 15 Nov 2022 05:48:22 GMT  
		Size: 10.6 MB (10574332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fe379b1cb877618883028c526405ae8a45527d4cf30a889c511dbd595617267e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65357715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86deecc4a038c32934e83eb0447627721c43994502e9589de7597e4d03b850fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:61184f89072a3c78d3fdc6e10746c2315c3dd04e0f896e4e5486e0dc876388c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69725443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805fedd3356c66ff320ebb73f506860153f1e79d80dfca0e179000409d4389af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae7924efb119b8e546bc847cfbb05a97a6c41274d7002dac9b3be1e451037e36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72140149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3214e76be9d9a0469bd9bcf8b028a28fbe1841128733092c197071817e5b2feb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:11 GMT
ADD file:2962b9f6c2d1271d6b4d04e8eaf82fb990726e0593bbe685576851ef47447301 in / 
# Tue, 15 Nov 2022 01:41:11 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:03:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9c6907f3cae53506b5149dd6542c3e51b750fdf5adbe19d7e949974888503c1e`  
		Last Modified: Tue, 15 Nov 2022 01:46:36 GMT  
		Size: 56.0 MB (56020725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2336bc5de2024196f448b0076a64552ad91a769c80127a224f16c9a01fb8ff`  
		Last Modified: Tue, 15 Nov 2022 07:11:36 GMT  
		Size: 5.1 MB (5086828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be24ed5e811e8ae9e25d22e72f2576ffb0280f9f49e1656cdc09cfb11b66d6b5`  
		Last Modified: Tue, 15 Nov 2022 07:11:36 GMT  
		Size: 11.0 MB (11032596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:926fb683e7f53979eb804c55a9299b25e5b403981ea343fcfce7776406cae41d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68841438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba302ed7e5ac196e7d0e07c8a5c5a877a25854c6a9e2db01c3c12494395e87b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:08 GMT
ADD file:65d4d16b7aebde0e13c3de84312e229b51904d161ba4ee74a427b6fe7c6dc6c9 in / 
# Tue, 15 Nov 2022 04:13:12 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:12:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec4356bce7812bc703a76dd14989fc14f03913b2da506e0bdcfcecde9d90e7c3`  
		Last Modified: Tue, 15 Nov 2022 04:20:33 GMT  
		Size: 53.3 MB (53260363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a6535eedbf12518e9b359dfc8738afc5b9728263ca9f95d8b79b809788832`  
		Last Modified: Wed, 16 Nov 2022 02:30:43 GMT  
		Size: 4.9 MB (4919324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f0bab15c9a3054d6f2cf26d98a668e19adc16414e5cff4a165374c84263b3`  
		Last Modified: Wed, 16 Nov 2022 02:30:44 GMT  
		Size: 10.7 MB (10661751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f07bd378b50b32ced77fb76c2d07cef3c771323300d7f360de3cb5a229107744
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75955529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1d69192f14562a5959b5236ee4397950c28411d106ae371844aa1463c368cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:22 GMT
ADD file:ad50fc3eae09fb4e9dc960bd1a5071e059a703490dade7d93f45e6f3889e18b2 in / 
# Tue, 15 Nov 2022 05:18:25 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:57:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:57:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:36378cf2e435aa3fe86342fd5d14fddae4340c0e37965daf7b433470b18f6a02`  
		Last Modified: Tue, 15 Nov 2022 05:23:47 GMT  
		Size: 58.9 MB (58910757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e429c88c903b14c73fe6d1f43e9cfaa3f3ef38261640a928b3d6c552a3d3be`  
		Last Modified: Tue, 15 Nov 2022 12:08:15 GMT  
		Size: 5.4 MB (5414506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0cf7a4cdc822cd5fe6b34d29ac6282bc7758b04321292ec5d3e729ca7dbb0a`  
		Last Modified: Tue, 15 Nov 2022 12:08:16 GMT  
		Size: 11.6 MB (11630266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2ee6080501ef260d82b88b9627e1751e319d88d81ca4867ed9a2d25de6e3d494
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69186784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bce5bafeef58855d57eb59a90f7e50e517897cd3e5a81522d323177ebd9267e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:23 GMT
ADD file:85bcb55b71ee57dffe1ea720e85546e314d2691e98658779a6f732d13e2e1038 in / 
# Tue, 15 Nov 2022 01:42:32 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:24:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4b50a7f3d916ceefc2228edab7fc6bc3e2fd142f385b7a04544973edc988c99f`  
		Last Modified: Tue, 15 Nov 2022 01:47:12 GMT  
		Size: 53.3 MB (53271656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0393fb4aa0f74da410291e84bc30299dd564dd10213b10075a53b1b031b797`  
		Last Modified: Tue, 15 Nov 2022 06:35:54 GMT  
		Size: 5.1 MB (5148419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4197b7e030ccca45de7e8f69883bb8230075d4a2145a8eed213e69d9a4f4fcd1`  
		Last Modified: Tue, 15 Nov 2022 06:35:54 GMT  
		Size: 10.8 MB (10766709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
