## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:207f50e59fabb88d78c4176003fe96ac785480475b5cfe356ef8808abd41701d
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edb926861a9d4f502a93284830ab70dd511f10dba22d427145e7cef74971a4bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68267001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd96ac6c32156cf1a1c658177b9a3ee1c76550262bb5f66ea623755636e8df5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:614551a10c9ad7fccd0189f174cbf1fb15ea6db182f9158bcb7d472e7d0ec87c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d956c4cef36a85f57f008f68da4d1e02c289909cd4607c52fe1bcfe63079b6a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f6bf363f70c4023252f05afb24e47707d679a7228fa239d8cab73aa597b22b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5a3989375ad180ece61400975a554ee45480a60a4f7f27a3815e180bc6edf6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2616077fc9c85155a8638e3e522d8f64954d4729c41f266ab5c08725865e3863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd63debe5398b56ac201dd8e696edba5a4ebfbc032935e65f2a77a0697f1785f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd063e941f2bd56c9767dc264c9725a8aad4b1cb540589077951538b80e08cd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8221d1cae77e18f41dcecbcf9a45df7f68f7964a3fcd54081714b98ea6f1b9db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f28d7aade7f73d14ae1136cef4108958febc1311acc07fcc5fcc5a3078c265f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb0417ec2edc8a010da78cdc28304c5b85cddce016a1cbacbcdfdf4ac7a6462`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:06acd573d66fccb4d006a69d7299464eade5f43cf3257765ff58cfdd52e9c505
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73183321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c2ade806dee7826b8dc1619005e756a05fc525d79818df01e1bd6779cb8b15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a0a905bf7ea807b467faf44795dd9bc40297712a3c86f2f4871bc6e031a23f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7636bb61ce8f549e8684021e135baf9a7a29dfb066c765ef9068fc2e83ac9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
