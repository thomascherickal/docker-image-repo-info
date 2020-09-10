## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:a43d15baca73b82f3dffa04c5d7ae8f31a7c19fbf47946fcf9774fabf92e6131
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d747b8b27fe09d1892fbdbddd8406a70c2a2117415e129321c623a7deb3a712b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70340974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7f6bcd9536cb109beb0445bdfa0e83c1060ea01cf071a171706d39f98c0d7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:00 GMT
ADD file:91c81aa3735ab11fcf7db3eb2dc51c94759276e7d3657f0fe81829c133f7c8dc in / 
# Tue, 04 Aug 2020 15:42:00 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:24:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:25:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a7bda3d6de74128f57cc726f2172127887e010c6a291320273a9c9eb8ad29209`  
		Last Modified: Tue, 04 Aug 2020 15:48:28 GMT  
		Size: 51.8 MB (51838182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8231f0c7125cafbd1f958df6356c90a0dc3947e50ede3c176820814176b1318`  
		Last Modified: Tue, 04 Aug 2020 23:38:27 GMT  
		Size: 7.9 MB (7921995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4f23b97ad1b9a745be0f1e7dc1856f9a233a25a83f51b22fce0c16759de05`  
		Last Modified: Tue, 04 Aug 2020 23:38:27 GMT  
		Size: 10.6 MB (10580797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d52db08dedc8d348ecaa4b2730622076d24183747fe343272d7b3a50e6411e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67553496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2625b8336db20cfd2f354e1ed19dc93789302d94a07370c45e641f9a09ba12ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:08:44 GMT
ADD file:2b581429c7fee51f5899cbb76a5d9c36cf7223edcbb473fbe2f8db3a53a82263 in / 
# Tue, 04 Aug 2020 03:08:52 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:07:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:07:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a2a8e3d684f3a7d5eba8b8ba267ffcbcf9d2089c1f803e105113f8b34f8991e`  
		Last Modified: Tue, 04 Aug 2020 03:32:48 GMT  
		Size: 49.8 MB (49784523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa91b4ecc0f372adaedd757806f1b23aee559777f06d525ee224f6f2911c31f`  
		Last Modified: Tue, 04 Aug 2020 06:35:19 GMT  
		Size: 7.5 MB (7501685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9150d7965ec842da0721c1a458d2f16e78d852da4190dd6c46b4d82e38e27476`  
		Last Modified: Tue, 04 Aug 2020 06:35:20 GMT  
		Size: 10.3 MB (10267288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0a907fb47131937e9dfd3693343bed868ae85ebcfba365df3f397e4455fe4b40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64730062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85a0034c1b8bce09a56db1727fdb1d02615f462bbb5f0c988f284028f972accb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:55:34 GMT
ADD file:8d817c9168a8bfbddda5007f76443d27203cb5bf02ec609cd277ddc327736b10 in / 
# Tue, 04 Aug 2020 04:55:36 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:45:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:984ab044320fbabd5c060737e15adfea7aa109893b7f68f41abc04f445d3440f`  
		Last Modified: Tue, 04 Aug 2020 05:04:18 GMT  
		Size: 47.6 MB (47570419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93473ce552fd633dff0ed8a7eba4610e368b271c6582de1c474472a31cc7340c`  
		Last Modified: Tue, 04 Aug 2020 08:24:12 GMT  
		Size: 7.2 MB (7243678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9559bb2ff9f55098d0aae9e6210eb73fdb47f91e0b6fff535ae21fcbbfa54dea`  
		Last Modified: Tue, 04 Aug 2020 08:24:13 GMT  
		Size: 9.9 MB (9915965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:35a5885329a6dbbb07c536a70010845ea21cc1b981b64dcfb67adcbc8623afe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69204517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987a312453e6e6a41af020dae3c276409466979d39b116d218e63e5704a0980d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:49:11 GMT
ADD file:82c33a26fb9be3ddaf17956539af2b205bdb6e28fe5ff1c7304ae8f294fe9581 in / 
# Wed, 09 Sep 2020 23:49:14 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a65667356fa05b061c6733c879afab36ec44c6877341c2527e321b7206a26b2`  
		Last Modified: Wed, 09 Sep 2020 23:58:05 GMT  
		Size: 50.8 MB (50825395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730279b4ebb859065c90bbf90b3ac77059bd7d1e6cdc143106e0994dca9f4c59`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 7.7 MB (7743447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2c8b657c8d1b22dc8f6d15821f7035a315a0900f84b26ef36c86803feb02c`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 10.6 MB (10635675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7d9dbfdffda026db4f4bc6992a7f5ba0a9736a3b91e67d06a5db3d75b468022a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71969620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5450c90d662e44d72885e2bfb547b02d950e88634d8c1961584aa9e3dfdff24a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:36:50 GMT
ADD file:e3f476fccb15ccc08c3c8c26ac23f1909e7c0f79bc060289f35fc37bb4483f80 in / 
# Tue, 04 Aug 2020 03:36:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:04:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:04:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:308ce7c38ffec8ca43e219653810c298ee87abfaaa068ff112f1e8003b108546`  
		Last Modified: Tue, 04 Aug 2020 03:41:50 GMT  
		Size: 52.9 MB (52909727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429c636a1f75410c98b200faef3ff9f568a242579e0d885a7b7c70d771f96e9a`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 8.1 MB (8099324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e845809b7e141a8bd0e85748582037ea1e08bcb9ca449097624dfc315d876d2e`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 11.0 MB (10960569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7f7605f9ca2196625517871a1ba2d0dc6f3731a0512c3a3c5d88caa761828051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68600344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7792a320a2fc82afeca15f8d402bf74a3d0798c1e1dacc45d652f72015973dfd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:41:13 GMT
ADD file:9e3d31545fae8b44e8aa3ad24629d2336276c01e23dfbdde9885d01e61a54298 in / 
# Tue, 04 Aug 2020 06:41:14 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:33:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:34:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:249c58d6beef4ec2d380f0e2adf7ea99a80c295cddcf6f6bc3d6b463dfe44a05`  
		Last Modified: Tue, 04 Aug 2020 06:46:35 GMT  
		Size: 50.6 MB (50550783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049f809de28cc8d8e169ab9ee5721613f58fafdc670bbe6d66a1058fe998ee06`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 7.5 MB (7450522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557e2093dc94091a8f931745b728c83f35ad977f14de65f1ec5db00bedf8580`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 10.6 MB (10599039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:67ad1dced6dc489dd9af29c4fc5e5c94d219703bd8cd2f641fbfd2acdde2cceb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f2a92fff074c72572dfb53df34eafb1c31dbfb6d766ce865358c6e740d8163`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:43:52 GMT
ADD file:a1065b5d1a75daf3153a753a23c630c5a77451644b83418dd23b2c1d046c970d in / 
# Tue, 04 Aug 2020 04:44:00 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:01:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:02:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:26d0cc426ef5200b8e12941b37f3b65f8de8a01be463ecfef94be00ae56f5596`  
		Last Modified: Tue, 04 Aug 2020 04:50:57 GMT  
		Size: 55.7 MB (55655910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aadce00449a8701783ecb72b8dce872a06609d7a90a69b4dfa29a8727a1bc3`  
		Last Modified: Tue, 04 Aug 2020 07:42:12 GMT  
		Size: 8.3 MB (8347825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f8213614f8c61ad803c5be08bb2ca48b08b0b8111551a50801c69e31afcf4b`  
		Last Modified: Tue, 04 Aug 2020 07:42:13 GMT  
		Size: 11.3 MB (11327020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ee809f5a4ba794419fb939755e2dfb26f2ce6c345fde3cab40cad69f4f2f0e26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68511194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8de6252a44f4d8218e1512a21cfb7b7a6fc7c263a743bb9c1e071dfdd1de03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:41:38 GMT
ADD file:d30705fcc57734260b517d32c4d610f1fe18e7d5faa78a22754774f5bf15eb9a in / 
# Wed, 09 Sep 2020 23:41:41 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:04:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b7fac0c9089d6ff39f6a7de3af657a8d580a7b074b45118b115539fd90213654`  
		Last Modified: Wed, 09 Sep 2020 23:45:45 GMT  
		Size: 50.5 MB (50468550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e4abf36c400373c14e1dc03dc7d41c9bb01249ef118a39b67294471b0cea9d`  
		Last Modified: Thu, 10 Sep 2020 00:11:24 GMT  
		Size: 7.5 MB (7537717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c291ff634945f7dc165f540d95c5d3958483aba31d45fbae0ee30d37ef13ca7`  
		Last Modified: Thu, 10 Sep 2020 00:11:25 GMT  
		Size: 10.5 MB (10504927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
