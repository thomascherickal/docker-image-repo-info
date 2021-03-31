## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:ddafc3737f47b5900e063497e6bc98a99378776fc45a7eda8231155746585962
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:993c09037932672ae5a8ea72f7495dd558b7ae66aa9cf41457912c71b31708ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70906218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6999481b2d3adddd601438ce8f18013dc50c5eb41ec3825f8796d6ef5f7ab36d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:01 GMT
ADD file:3d2836abb42f177ad29a584ba02ccc6421b1613f73325823603fc98578f17445 in / 
# Tue, 30 Mar 2021 21:50:02 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:05:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:05:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff28f9110f9a07cc7303cdae0cac6dceebc733170af8336bff099af5e4b0eed1`  
		Last Modified: Tue, 30 Mar 2021 21:55:15 GMT  
		Size: 54.9 MB (54868057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b440922f9fc7a15146adf7cc4d35ea9d0bc9a6a6004a905f240fcad22cfe0bcd`  
		Last Modified: Tue, 30 Mar 2021 23:15:47 GMT  
		Size: 5.2 MB (5169284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd6e01879bcee5c3b6f0a9e069f1f61a436d7e55e344931794bbe2af8c7fde1`  
		Last Modified: Tue, 30 Mar 2021 23:15:48 GMT  
		Size: 10.9 MB (10868877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c74f625fc2632cb866705627945d23572d32948b27d22da47a54ee9c7678cb37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68046255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a293f49c1682cbb3c0e39505073cf5985571e0b059df0a85ceef7253fd10af8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:52:17 GMT
ADD file:c74b1cfc1e5bf1a62d213de82dd043a95a19f0f67a947b54c449d8ee5d53fb37 in / 
# Tue, 30 Mar 2021 21:52:19 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:51:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:51:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:06ea7b1cac1276634323a37913fac1e0f60820f2aae1fd14d07c2c573bfbce6d`  
		Last Modified: Tue, 30 Mar 2021 21:59:54 GMT  
		Size: 52.4 MB (52402138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d6173e3da10cc42bd51156af90984c02eeb52327364153f9648d30fe084fec`  
		Last Modified: Wed, 31 Mar 2021 00:03:10 GMT  
		Size: 5.1 MB (5073685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918922db8190bce87e065be6997a39e948ef367b3b3f4ab60ced0d40e98f335f`  
		Last Modified: Wed, 31 Mar 2021 00:03:12 GMT  
		Size: 10.6 MB (10570432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:60f29a333364b10385602348bffaff3e46d640c57f5fe52d7140da5951cab9e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65210037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcc3601f76a9fa9ebe4cd36e26b3616d499c0e12b3c7571f1a2e7ffdfae425f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:20:34 GMT
ADD file:f0720ec9bf7f39f48d23428e3a1efab23881784e0db60db3031465e45c1d4893 in / 
# Fri, 26 Mar 2021 11:20:38 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:26:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9215022a83fc46d1d35467f5bc69faee0fabb5fa515b7fe907a7f483cf1e6223`  
		Last Modified: Fri, 26 Mar 2021 11:29:54 GMT  
		Size: 50.1 MB (50071169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c633ce4b5971f906b64dbb1f40d78e435bd4f582179e60994bc399bf45ffe158`  
		Last Modified: Fri, 26 Mar 2021 13:53:35 GMT  
		Size: 4.9 MB (4920691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbcabf672b68dab52cce7bb41819db259dd2a29a05c53c36a0e536ac293ad49`  
		Last Modified: Fri, 26 Mar 2021 13:53:37 GMT  
		Size: 10.2 MB (10218177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1430d9141ac99974332a354d4451160fa9c2052749c185c4dba51073b2922df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69581095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f6ea7ff9d1a70982397729fa7ef9e36309d85d24001f4d6d8b5280b45855f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:48:22 GMT
ADD file:367b87909b67093178b79312d10fd1e5f34fd8f2d88ff86d5db05018c84e1de6 in / 
# Tue, 30 Mar 2021 21:48:25 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:18:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:19:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2f6f2092d4e11ede8755fdc276c7abb424692833ac06435c47705ad7024c2459`  
		Last Modified: Tue, 30 Mar 2021 21:55:24 GMT  
		Size: 53.6 MB (53555909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7329ddb16965a8f564ba84df809cf2bf57cef4de5272f15c7ea208a725068c`  
		Last Modified: Wed, 31 Mar 2021 00:31:34 GMT  
		Size: 5.2 MB (5156631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800c7b57132ff5a24ff23004e5ee11478f43b53d722d70dab97db2330112cbaa`  
		Last Modified: Wed, 31 Mar 2021 00:31:32 GMT  
		Size: 10.9 MB (10868555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7e1d9840bf16a395503e5f6c978ea7813c8e1e39df35757dc5d023f8b5717d6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72428844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd4aa35de62e2c24c3d8c093a8d0e4a590e99a81ae1825186ccd3b810c96a164`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:40:35 GMT
ADD file:1f041945ff890476db13a1209d904306e018db9cc0c3ddd68afde8ba20721441 in / 
# Tue, 30 Mar 2021 21:40:35 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:59:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c1abc0a07df2794b8c01aadbeeb9293997b8a54aaa313f435b4d2d676f888235`  
		Last Modified: Tue, 30 Mar 2021 21:47:59 GMT  
		Size: 55.9 MB (55881675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc5ab305c1c154665b02986b2328de2fd181084b0c296c4d76f131107ddef04`  
		Last Modified: Wed, 31 Mar 2021 00:09:46 GMT  
		Size: 5.3 MB (5298115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95df009a7c979f03789affbb069b0972638a182a6594760beb04e5d621ca33b`  
		Last Modified: Wed, 31 Mar 2021 00:09:47 GMT  
		Size: 11.2 MB (11249054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e508864ca39f8dbaee96371a8ec8c3dbe61bbbd1aeb3299f4cb31d09a18221a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69126266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36dbe3ae2bf1f4c9c1353429bfea53b1212171e3b3404b89b1b8870f1afabcf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:10:14 GMT
ADD file:4d20c8e17f6123a0d4b72a62f938dec2586886ad6d87f246ee55a11ea923b684 in / 
# Tue, 30 Mar 2021 22:10:15 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:14:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:15:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec4a0a6790f3ff962dc7c25a161644b3cc5e5b8758356dab4f112068aa643317`  
		Last Modified: Tue, 30 Mar 2021 22:17:08 GMT  
		Size: 53.1 MB (53127307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90333279e95c41e8d6dddbd8d32157d7b6e64b62fb5b735d17ca9d796904a82f`  
		Last Modified: Tue, 30 Mar 2021 23:25:27 GMT  
		Size: 5.1 MB (5127929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af84110c224d7e9e68767940402f621ab1b3a77a6c7b483749668ff6fccc186`  
		Last Modified: Tue, 30 Mar 2021 23:25:29 GMT  
		Size: 10.9 MB (10871030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8894049f8ed64a860940038abc63a43b95d3fa093b76f77952b16ace4465aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75802995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c30f249f18192d3d96b12bb66ee72e2898db21200184dc61254975412e8dab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:45 GMT
ADD file:7106c38838d3049ea5f78c190ea790f58ea352546fd1b55d2b07a152c34377c3 in / 
# Fri, 26 Mar 2021 15:14:59 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9927b5cbb0465e067777696ede5217a35993b727460cf5c92037d8823b48a09d`  
		Last Modified: Fri, 26 Mar 2021 15:22:31 GMT  
		Size: 58.8 MB (58782693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58a377d45252b512386356a873c76bee0b1dfb06189ebc9b0b723496f735b20`  
		Last Modified: Fri, 26 Mar 2021 19:47:59 GMT  
		Size: 5.4 MB (5399498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6380788cb9eda4a73e189b4139db3eda3a7b9f06d4e61e07160541bdec59499c`  
		Last Modified: Fri, 26 Mar 2021 19:48:02 GMT  
		Size: 11.6 MB (11620804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a91676c9960fb162dc72e51871637a030b983bc5dca5951f2e6c0539f9bdba1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69057191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:257af8772141f0e489cdf9e46f7eacfd10836bee6ba5795dec0e8e4f45b96526`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:56 GMT
ADD file:c96fcc34ba5121a1c8780b0148c4b2ceaaa9ce733fac0a9830e3f557d45d7c9c in / 
# Tue, 30 Mar 2021 21:42:59 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:44:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:44:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bcb476920ff38aa084b50cb5a5e43afc962acdfea91e11abaaef6fc258b79a0c`  
		Last Modified: Tue, 30 Mar 2021 21:46:39 GMT  
		Size: 53.1 MB (53147808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9941cdff622917fbf0a7a90b9b9bd51d58de5471a94cf52add39fa8b62837d6d`  
		Last Modified: Tue, 30 Mar 2021 22:50:37 GMT  
		Size: 5.2 MB (5150758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd7897b18d3d481ba626f3a769e62e5ba9a769adc21d00817aec4735d3e628`  
		Last Modified: Tue, 30 Mar 2021 22:50:37 GMT  
		Size: 10.8 MB (10758625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
