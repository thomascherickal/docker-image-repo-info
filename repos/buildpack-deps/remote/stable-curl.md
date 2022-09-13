## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:af6b492797c0fd11974144ef18cee6c9c52df6957163f19e61ab986a29e2b780
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5bdb1fe4f9744583e9bdc673baf4e40f07814bbd277e50bb6d5f28e74e8914bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71069316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8138e50ba7833ea9e2e3591614d95cdfbe11098791fe496122899e1e804d01f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f801b184d3dcd91d5ae56c3d969a1d264de6e24c2c3e76691e326c27f951b861
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68176859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a50234ba8db46e295440868b5ee1b9b4caf2cf7b0457cf9a1512062e4353b0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:03 GMT
ADD file:ad560226d0aa0be51fbe1d98a8877aeb30110956b3a7c0f849a4331e99477ee4 in / 
# Tue, 13 Sep 2022 00:53:04 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:24:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f33103174415e8d15c8ebada62aae8327ecba6afa6035819128965eb1a64966e`  
		Last Modified: Tue, 13 Sep 2022 01:00:25 GMT  
		Size: 52.5 MB (52532200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74e3dd9c2e4e29e0f4df5b3d5a6bb6b72260bbd689082c1a14fa9f93bb7356c`  
		Last Modified: Tue, 13 Sep 2022 01:31:25 GMT  
		Size: 5.1 MB (5070938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ac23bd65f92366f98c6b75e0e91d6a10949d9f11f5c82875829dcc719266d2`  
		Last Modified: Tue, 13 Sep 2022 01:31:25 GMT  
		Size: 10.6 MB (10573721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ae0f8079029fda4c5276378547b2b7a937f5a51e5c3d13720156877ae4892080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65344693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be6e1842e1c61cc1f772c3570303395e657760d4c7dcc72e71f8961ff5e964d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:17 GMT
ADD file:c60a3ffee6188f27e9b642109e01c6145bdbb8d4fc17475a2711795799597766 in / 
# Tue, 13 Sep 2022 03:42:18 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:31:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c0b863d4b31f0197ba7a7b6995cafb984dfbe6a0dcdedf88f2ce4a2f2c70b2cd`  
		Last Modified: Tue, 13 Sep 2022 03:49:09 GMT  
		Size: 50.2 MB (50195605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8418b877b4075c62cc53eb0d02b6b19d0d930a8e54ef2875bff8e9a948025c2a`  
		Last Modified: Tue, 13 Sep 2022 07:43:57 GMT  
		Size: 4.9 MB (4931269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d43cbe35130a47e93c66cb18df3b645f264e50e2d44ba95531a11148d4029`  
		Last Modified: Tue, 13 Sep 2022 07:43:57 GMT  
		Size: 10.2 MB (10217819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ee008b29bb7ec30101a87203d7cc939b791459cddf1fd9e8e65986e727ecd94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69497803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa3f0560f94904ca621db9ce326557b8ac8de449377eb1ef627748cc3aedda4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b6f06c1891a3f41f9129b81cc88f407d82d94ed3bf13c85f799b0afd8c482269
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72333619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b278b2633159a5f2bf2918874fe4e283e00f970eea9ee68d9839e2948b083d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:28 GMT
ADD file:7cd0a464573b537cf29f9a72bf3b895bfe96cce867ba3851402a98bca7272ca0 in / 
# Tue, 13 Sep 2022 01:39:28 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:49:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c56ebffcd7db97f938c62b9ad03478fefdde78fc8b85916da5d75054970df458`  
		Last Modified: Tue, 13 Sep 2022 01:44:50 GMT  
		Size: 56.0 MB (56009860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b2926e999b0f68db69f91ece9d0bb97c79da80699d3a387e1ac5681d01b1f`  
		Last Modified: Tue, 13 Sep 2022 04:57:05 GMT  
		Size: 5.3 MB (5290983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25017ef00a9bb56c10606c65882cf1a863cf50ae6da48809e67da77aad2607cc`  
		Last Modified: Tue, 13 Sep 2022 04:57:05 GMT  
		Size: 11.0 MB (11032776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4db12cc0ba630b1436bc6abad64efb317f331f269fd436f10bf9b2d00e2c2d36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69036675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b46efa153f17452a6ad1dc9d6203893574222c0cbfb1385a4270990de5eea1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:24 GMT
ADD file:01a7dd1465cd33040941b52c4ec3699247b2ecf8c53533b3a234445013452157 in / 
# Tue, 13 Sep 2022 01:10:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:50:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec9a494c35bfb06348155378649b8055458795ad2d004f471b887021323b94f2`  
		Last Modified: Tue, 13 Sep 2022 01:18:07 GMT  
		Size: 53.3 MB (53251789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee02f93015f130da8dbe807a5b123a0f332fa75b55257f44d6a0f3c8fcc5da3`  
		Last Modified: Tue, 13 Sep 2022 02:05:49 GMT  
		Size: 5.1 MB (5123957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f6f6b0c2dd6acd42de4af694f71bf39f08a8daf7243600350b63f5c4b85787`  
		Last Modified: Tue, 13 Sep 2022 02:05:50 GMT  
		Size: 10.7 MB (10660929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1847a6cb82bc9358f1c9884c4e3042252f08d2daa91004bf5dc17a1a99a8e2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75944608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d281ed50207d322bd4059ce5c93d9eb0ff87f6dc5c913fb78caa40a61ac78e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:07:34 GMT
ADD file:01cdcbf6300ec08ebb8bff41970509b38aff6d26164dea3fb476a6254e441e9b in / 
# Tue, 13 Sep 2022 02:07:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:14:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7d6144dab736564be3fb6a092ba7b12047adae858b56388b2c30f57e044d7565`  
		Last Modified: Tue, 13 Sep 2022 02:13:01 GMT  
		Size: 58.9 MB (58902594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7fa9a7ad3fd314802c655b3450a54569fcfa864dbfa0229721d8bc79f2a0b7`  
		Last Modified: Tue, 13 Sep 2022 05:24:55 GMT  
		Size: 5.4 MB (5412954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2712f6dbb2a2d0105245643b5cbd920b09c66574e06dba7618247607f8c8827b`  
		Last Modified: Tue, 13 Sep 2022 05:24:56 GMT  
		Size: 11.6 MB (11629060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6c18ae0bd6a4b238d8361c37b5e342e005b5d70991e956c983b33c2ef08c5c32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69177602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6362e9080b927e255299abfd45174a8989307ebf26f17953e2eb5ecd2b0ec4a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:47:47 GMT
ADD file:2965b342d27ea25d073bb5f216362150cb8ec0e05df43fae8e4ee6251006d17d in / 
# Tue, 13 Sep 2022 00:47:50 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:25:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:25:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf58bfabf9fb5ab735277c32678e319fed106496e2f1070ac6bcf35a57d3870e`  
		Last Modified: Tue, 13 Sep 2022 00:52:18 GMT  
		Size: 53.3 MB (53264823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce515b66a74a291f416a7fb9b6e39594047957a72b0b2f38367f724790639590`  
		Last Modified: Tue, 13 Sep 2022 01:32:46 GMT  
		Size: 5.1 MB (5146951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bf6be09afafe08d5aecef2a5a139e863d43fb30c9c5dd6aed8fe8bee2c15c7`  
		Last Modified: Tue, 13 Sep 2022 01:32:46 GMT  
		Size: 10.8 MB (10765828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
