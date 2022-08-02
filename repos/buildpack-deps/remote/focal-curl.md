## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:a8b84a6b07a1d7ce40373d4c46df6456dda83608dfbb3768a2d54c3ef6612bae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:533856bdcf2ca47043a383980e1e631ef56f691e50017be44199e110e0f8f7c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39963959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36b5de254451154bc47a98f0a00e270cd89a7db644d3bf6ba8b914689584ac5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:59:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7717a5180c5ae3a4a32707e77e623829962665d9a0172f2009dbfb4a8eecd8a6`  
		Last Modified: Tue, 02 Aug 2022 02:23:14 GMT  
		Size: 7.8 MB (7766992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac35116152e46014e5a995b6ee1e2d20c86c70dae249f2fc9c37034057162d2`  
		Last Modified: Tue, 02 Aug 2022 02:23:13 GMT  
		Size: 3.6 MB (3624371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:906ed436fe65f8c2c684d883d3da1561827838dd0bc17e144d188a281fdfc753
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34449771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18ab99087c24b628efd9e394f93e2e04ea1b5e24f38fbc08e4f517e0ed66ce9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:56:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c939440c1bd88d1d1d434d3aa1ea94785fdbde5a1afb6314202876a124622a25`  
		Last Modified: Tue, 02 Aug 2022 02:15:15 GMT  
		Size: 6.8 MB (6756450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945d9dd06ca6053a40015193ee5c594f3eb35191a1cb14f2256dfa9a0c2cc08c`  
		Last Modified: Tue, 02 Aug 2022 02:15:14 GMT  
		Size: 3.1 MB (3104048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:196e4aebc99648365b96cdf49675a7565f1a2f51b7cbf9d53ab2589bb900f2c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38210796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b04598a2bdb0b055d6b09084c3b5a6dd5733efe3908208649fca71e2667f89d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c444542145972df20962fba6d4329459e66f2f686af24d63dafc2c5a1b6efe52`  
		Last Modified: Tue, 02 Aug 2022 01:49:44 GMT  
		Size: 7.6 MB (7631155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924b49b3caa4a90a845795499c127cec28b1a834dea8b2af26a4a464f5cdfed`  
		Last Modified: Tue, 02 Aug 2022 01:49:43 GMT  
		Size: 3.4 MB (3387837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:10b729472c0498313d00d744337bcb6c076db4e60729684fde4cc4b643bf4299
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46471614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087de4e1f05a8fb01899a7dcf89bacdb21c5b6916ab2b6f4e89b053495de5ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:47:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca086000ee182105fab40e65e78925b959ff132f3014c9bf7acfb24de5b98d23`  
		Last Modified: Tue, 02 Aug 2022 03:21:21 GMT  
		Size: 8.7 MB (8720038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4936b2d19b6d4f30b5a0f63f857c77c3ff1044ff396dca9415d4d010b1fa45a0`  
		Last Modified: Tue, 02 Aug 2022 03:21:23 GMT  
		Size: 4.5 MB (4456224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:3a9320a515e88a4c5f26d2ed6f9ee5a78a323942f2b6b82002701e60a3b72ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34132693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50298c9b870829ca807c6f0909305c557f1e901ef7cec07e0d0dcb1903352e6c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:b0715cfd07e2ddb57c893eea71623a5003563b19ad3176db6cab4f0b79366e4f in / 
# Tue, 02 Aug 2022 01:10:35 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:28:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:27b013c4be5964fe14904a230ee4535e43cd11774e0dc02bf7981a3beb6562c7`  
		Last Modified: Tue, 02 Aug 2022 01:27:40 GMT  
		Size: 24.2 MB (24243569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e88378376f98b3eaf04fb0de984f0ba3f7f78911f518816d823bd05dcfdcb3`  
		Last Modified: Tue, 02 Aug 2022 03:26:07 GMT  
		Size: 6.7 MB (6744171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eea9cb07191a486c30dc13b845abd6c3c220a2d93d1b3925b675ed4fb3bc22`  
		Last Modified: Tue, 02 Aug 2022 03:26:01 GMT  
		Size: 3.1 MB (3144953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0920173b3f0d08861746cfe93e87f123f1213001069c12bfdfe8ffb7ae186aea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38000526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f4730e45e3719d71e10f4a04f9c3c3da90e5141dda3b324bd0a8a9710506d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:19:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:19:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3afb2f7de67ad545f5de8adfd96f7578e1d0e55e79f41f3a7278650d9408712`  
		Last Modified: Tue, 02 Aug 2022 01:38:50 GMT  
		Size: 7.4 MB (7412554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67acf8da821182b10d1d774808bb08ce2cf3de1b28764bb20bb702984a97f18a`  
		Last Modified: Tue, 02 Aug 2022 01:38:50 GMT  
		Size: 3.5 MB (3542609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
