## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:eca53212a38ea21ab9ad8a1529de0e674b901a16400278c01f9512d59dacf576
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3b9052fbac34a60289a0f98a8418250e263b629ca01572f0aa3116675561baf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73549510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f1bf79628ea9b0ece162831f53a1be7fedac3b4a18487fb6463a34618895ea`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:19:54 GMT
ADD file:7e968e6ae38ede120a52f1d2e734b4fee4fd4ffd6e5f747edc8190d2a8bc6a52 in / 
# Thu, 23 Jun 2022 00:19:56 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:48:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8849e73adf621df4a443e9ac4eec9b698476e4f14f8ed894806f302d5b33156b`  
		Last Modified: Thu, 23 Jun 2022 00:24:12 GMT  
		Size: 53.0 MB (52993983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a3004561e732519f3aa704178d4bc2d97eae3c1cc556af0ea0d3e66e28ba24`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 9.3 MB (9291497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0f93f12fe636ab6b9beed73979390ba6a1aa6fdcf7bbc5cb403f683142a0e3`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 11.3 MB (11264030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:653f106c506aa90509da1173e802c778235c9266dc48bf5f300dee03c085cb3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70422433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26bd66779589c7c7ebc3135bc7e39d139ed1412a6891bd98094afaa6225cfc0c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:49:07 GMT
ADD file:d8a58d5f4d1c34aefbf2ca6b2eeab0bbf20b8cb6400548926c6a16cce570dc9d in / 
# Thu, 23 Jun 2022 00:49:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:32:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:32:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5248fb4f18035bd1257a3136675241430095c1cdf250910c001999b7f421381c`  
		Last Modified: Thu, 23 Jun 2022 01:03:30 GMT  
		Size: 50.8 MB (50767843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b7a64f309184d3ebc17e9dbe6bed869037215ff9f9748c7dffa9ffd3e631ee`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 8.7 MB (8726860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a0203b6e2645c48e6d7e1a1ec99807f7da08cea315ce1d19d9ca8ae62d6246`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 10.9 MB (10927730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cec99b356856c9867b8814f565bb3eed4778ed225c2aa632a14ba17fb356050d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67476367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecade07de1a96c6f49299b77a358afd85fbdfdb208a95a9e7f39eca06c89a5b1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:58:08 GMT
ADD file:485670bbc3d21c74d06e079229d1c74d05970c4bdf8c5d25692ab1464f0acfce in / 
# Thu, 23 Jun 2022 00:58:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:42:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:42:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:da5c76d2fa54760a1e859c83968ea6d7dfee1c43064fb6f34c27f8d639859b07`  
		Last Modified: Thu, 23 Jun 2022 01:13:19 GMT  
		Size: 48.5 MB (48506514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231adce49f6a983a4cfa3f3683a6c276af5ef432ea37e705272135b3a56084b1`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 8.4 MB (8397133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487327d153dbcbea96feb013bca9efcd1fa6319396003a967515da5f4ab1d6a`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 10.6 MB (10572720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3c6e1c91cd82b6d69eb516a5f017b9064bcf887bab8f1462f308fb682756577c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72242992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876a62fe8cbafb7ada691e9fd43fb9130ac228927fe65c5cfcdef51156181259`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:05 GMT
ADD file:149d923f098f33a347aa57ca673aae5cc103628b202337e4ff2ea5ac278e5c18 in / 
# Thu, 23 Jun 2022 00:40:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e34000263ac838bb9254930c5e34d9fa4b486f544707ae0aa508bb7ded624d59`  
		Last Modified: Thu, 23 Jun 2022 00:46:09 GMT  
		Size: 52.1 MB (52074605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d844fe46570aeb3a40b42c67a4714c432ac2d6ccc31125f7eeb076c05e919ff`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 9.1 MB (9126954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39d92840e0fe1b4aa70af7e37d1e6c48b3c61da85b2b3d9e13efb83c990d2d`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 11.0 MB (11041433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:65cf46d760f73749c7674db469da8436e0de488df7fd77368da8d6046d635cfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74892536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b856c9b31c533e0b1f9d5b60b96fbb7daebbdb6ec5368fa60d7896aaac101f32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:38:52 GMT
ADD file:d8108af9af2f3fb7f3dd905a9b4dd8391d568ba8dd590a9ca2bbeecd44354e03 in / 
# Thu, 23 Jun 2022 00:38:54 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:08:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0120d80f9ec3d96114e34087bd467cf9989c9c723cf7622bb16fb3675443565c`  
		Last Modified: Thu, 23 Jun 2022 00:45:18 GMT  
		Size: 54.0 MB (53963635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a0c1f242a443b42292f09b23bf00a038a40230b125f2d832ff706e0b0fd009`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 9.5 MB (9464738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2c7e9a858ffdd4f52faf3fc1e4e080485c9024f299858237d4b3961f4e27d`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 11.5 MB (11464163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:40c37bc6cdf6cddfb29a76ef7e74ad2f1187f868292f0062b9255023b25adbd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71766462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e24a8cf4b182495fa008fa59c75741eb00eec064cace5d891954e37258a4987`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:08:42 GMT
ADD file:8bc6b496d7debb22306bce782f6b34ee75efae7151dc19314b45a9751b8fbdb4 in / 
# Thu, 23 Jun 2022 01:08:47 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:44:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25ef8061366d5e6abd7ca324b8c1f08ba96be6bd0e55fd310e046a1e4becfdb6`  
		Last Modified: Thu, 23 Jun 2022 01:18:17 GMT  
		Size: 52.1 MB (52089294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8d0efe31fb7f6ccd1d5334126a57a6651ed1009e9a6eb93f4fb51019078cf1`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 8.7 MB (8657797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d342e8e78e8778dab632125fd70a05b026d9c29cfed07832f8527747409a8a67`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 11.0 MB (11019371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e1944d3105905a9346fc89b32171c042ce5ddde9160ae5c968b06b747b690553
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79146572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab721b3b86bee7065c7a4c4ba25785bb41a6cfd197e38169fbde7626e2c431f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:00:58 GMT
ADD file:d857864fffea40faaeec8c9492ef1805e6c891ebf06f1427f02398a3824debce in / 
# Thu, 23 Jun 2022 02:01:01 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:43:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:43:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8afb6214160c68cb540431e94c7bfe898f1a094dc45a834aa07634d34b1505a3`  
		Last Modified: Thu, 23 Jun 2022 02:12:13 GMT  
		Size: 57.2 MB (57198049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a70dd21016ae34b7615f4f27bc039c2c609a2ac123e43b625424da683ee24b3`  
		Last Modified: Thu, 23 Jun 2022 04:54:13 GMT  
		Size: 9.9 MB (9883483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb14a4d02ea4ebe3ab1ddfc7a7bfdc8945f0478c8c9592495931e4a0a21b69d`  
		Last Modified: Thu, 23 Jun 2022 04:54:12 GMT  
		Size: 12.1 MB (12065040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:70e8c0be7716884bbf6e439fb9b4ed79c066cfeac29253ade7997e17c23914a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71626792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5809a878b0db1a9448348501dd6faa37724070efc02128249503451721616d0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:51 GMT
ADD file:b7c920f3965a4e47e7a0f42e020e195f493babee2f175c563676dd0d45c0b27b in / 
# Thu, 23 Jun 2022 00:41:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bb926b744d748e9437f2a0a451eea25192350981dae9cf0d8effd239dd22e761`  
		Last Modified: Thu, 23 Jun 2022 00:51:01 GMT  
		Size: 51.5 MB (51530571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ecccdf5c546fed3b800725dd538dd6145ccb9ae337d876c51b657ce9b04f1`  
		Last Modified: Thu, 23 Jun 2022 01:34:04 GMT  
		Size: 8.9 MB (8938768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98bfe7c167f54ada5e3d22060e56ad9ef2d8269fb0c0bbd4e5683afaf21b548`  
		Last Modified: Thu, 23 Jun 2022 01:34:03 GMT  
		Size: 11.2 MB (11157453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
