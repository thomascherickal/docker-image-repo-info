## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:86708854e9514b1214f431caa033f76b65efa1cd616b3c222782bb6f352fdac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bf3cc2ed27fcf938725d13aea1d234157b51a2da0c48624934c0e1a348442cf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37627873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37635220052b6b18506f2480a8b488ad896e56fcaec6b2a3ccca7f270e62196`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:16 GMT
ADD file:9b7b0966dfc440424d605ce69eca7c183576d2d20f1534bab2c169b0550c40f0 in / 
# Thu, 21 Apr 2022 23:00:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:34:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6eb9a17f92a2d3c01d47408a9505c2dabf5eb36c13a06aa25adb53b1ee5ab488`  
		Last Modified: Tue, 19 Apr 2022 13:18:15 GMT  
		Size: 30.4 MB (30382790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5275ba0f5172bfd64048b6b98ac08533fbb66d053934c9c7b813ed878a4da84`  
		Last Modified: Fri, 22 Apr 2022 01:45:40 GMT  
		Size: 3.7 MB (3692700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3cb7c82ce77fbec430919bf961e3bca4f910d57ea0e619a23e23c5c44736f7`  
		Last Modified: Fri, 22 Apr 2022 01:45:39 GMT  
		Size: 3.6 MB (3552383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6696fbf915a0c2027bc41749ff454404b8582fb816771270b5936015ed68f8cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34106873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f53b16ce2bcc22d70462adb95444e8e27aa27899356a241b000c1fd6332316`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:47 GMT
ADD file:ecf74a6452f34ded24f7515e4537aeca812185e117cfc8986807ff6e18f25a97 in / 
# Fri, 22 Apr 2022 21:52:47 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:41:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:41:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dadd872247af43291368f8a67bb613d5cb8cb866f3c4a1485dd86dad2e802953`  
		Last Modified: Tue, 19 Apr 2022 13:19:39 GMT  
		Size: 26.9 MB (26920017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad1cde781047c91b182501ba2a980864b99eeb9e58f485cac23711602e35c59`  
		Last Modified: Sat, 23 Apr 2022 01:59:05 GMT  
		Size: 3.4 MB (3443310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308f4c4ae626d207faf42fc5629df614215c2822ad419cce83125f24fa935a1f`  
		Last Modified: Sat, 23 Apr 2022 01:59:04 GMT  
		Size: 3.7 MB (3743546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d864416af83c7dd57ca07220c2617cf182d0c54edcdce9be008acf524cfe5a7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36034710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3ec56c9e046326caaf2f37e5f884de44106e5a31cdb2df5e39308739357eb4c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:21 GMT
ADD file:6998b0e46e0cd31d7f49d4821785499f9320e937e411c08b366999aa8a168371 in / 
# Fri, 22 Apr 2022 00:54:21 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:33:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:33:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:145dcaaba60b97cb30153830278268147f4aeb48c492406b9aad9b1fbfdb8cca`  
		Last Modified: Tue, 19 Apr 2022 13:19:04 GMT  
		Size: 29.0 MB (29029667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc9e1c1f6be60892f50b5d53584c348b20eff4bea7f4d33b65e7673322f6498`  
		Last Modified: Fri, 22 Apr 2022 04:41:04 GMT  
		Size: 3.7 MB (3677167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a108681f59670606e206adb362c96b8ad0b0195f2949fff6ad26fcf5b356ae`  
		Last Modified: Fri, 22 Apr 2022 04:41:03 GMT  
		Size: 3.3 MB (3327876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:259cb7abc1123a18176085ca8d41a36f491df064640fe46c1c321711381921e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44561273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec74899e0022a5ac1867a28b85f47817014c3cc498084460fc6faa3478f95c43`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:33 GMT
ADD file:f7aa4a99dde17a8de92a81187e400ad5d7c8d77f51c5326a58f5ff3b9bde84f5 in / 
# Fri, 22 Apr 2022 08:08:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:25:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:26:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9679fcb395f86c315849eba78321cd3b3d42168bec93b728e8af50bf74bc3f0a`  
		Last Modified: Tue, 19 Apr 2022 13:20:18 GMT  
		Size: 36.2 MB (36172233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec86ac3701804cbb97b0d974368ed0e361a23b0ba9d44e1d693993f65de57afb`  
		Last Modified: Fri, 22 Apr 2022 09:43:11 GMT  
		Size: 4.1 MB (4146613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cffe7f70cd94d121eb55df172917e21b569060c4fcb4eaf6f171e3a8266c93`  
		Last Modified: Fri, 22 Apr 2022 09:43:11 GMT  
		Size: 4.2 MB (4242427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b0467981015f76d54c516e0715870581b3285d99cd02bf7d328ede25a8457086
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34505107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de40ea1f712fabf8d6e7e2fe1d6c68f8dc6af29fcbea47f396fd03f93b54c64`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:16:35 GMT
ADD file:bf1fbf364f8a0fef0fa4b4a09345adc1e05055c47d99b0751d87240acaf19201 in / 
# Thu, 21 Apr 2022 23:16:36 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:10:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:11:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4422bb9ff39d0068917ac97faf0afb995ffcf3e120e2c72c5948a1f185b17525`  
		Last Modified: Tue, 19 Apr 2022 13:20:50 GMT  
		Size: 27.2 MB (27210182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e51e56374944dbe4502b36fa828f86aa453deb9730c96ef7900ae7788a0a4d`  
		Last Modified: Fri, 22 Apr 2022 00:51:58 GMT  
		Size: 3.5 MB (3490482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05afe80da4939c1390130c76e59671102a5992c02f1438a9426f65d3b9bd5318`  
		Last Modified: Fri, 22 Apr 2022 00:51:56 GMT  
		Size: 3.8 MB (3804443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0e584574d1a57441dc519c04420699d70ac1476b2cf9d53232f264fd1e4d7e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38228463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d273c789749cfaddd40c9ce7451947b6579d593fac01b3c1b9c9bcd888b6c807`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:50 GMT
ADD file:ed9f1a2ce6273c6125a668df86eb3c70b6b86877b70e37f79cc5234e7090fe28 in / 
# Fri, 22 Apr 2022 00:39:53 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:39:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ecf40b50e939ec0e9091530e9b3ce6296dffc47abf68cf7da9d4a2fe6e07c492`  
		Last Modified: Tue, 19 Apr 2022 13:21:29 GMT  
		Size: 30.5 MB (30502266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240bab8b946430851e89cccfdc3e4ff0732fa4df3ae386d86577afd7fe18bff2`  
		Last Modified: Fri, 22 Apr 2022 01:52:26 GMT  
		Size: 3.8 MB (3762548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180de86e618c8fc39d78e6a529def6060d5678aeffff45b6b51b39b98b666d09`  
		Last Modified: Fri, 22 Apr 2022 01:52:26 GMT  
		Size: 4.0 MB (3963649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
