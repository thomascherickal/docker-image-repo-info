## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:2ce8d0a1dbbb25c81271943c6b475739fbf85572af909e05b5440f55e2f19008
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:4392e93bcf34f6dd22e4340b5e48ade1269c3f44b634a3e4ec87c03094cac545
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49557441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768b465e67365ea9504b3a87416a869209cfca1eecabbd336b9e86d407a0f09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:39 GMT
ADD file:8415eb847ca46ed1aa1695965af86f1a0f09e8859a7b3c07b2f719404b665102 in / 
# Thu, 07 Sep 2023 00:20:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:20:43 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:012c0b3e998c1a0c0bedcf712eaaafb188580529dd026a04aa1ce13fdb39e42b`  
		Last Modified: Thu, 07 Sep 2023 00:24:59 GMT  
		Size: 49.6 MB (49557216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ddb185f1735b8a6cf336691c0688153abfe60fc2a0835aae4d146fae62d4ba`  
		Last Modified: Thu, 07 Sep 2023 00:25:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b2aa4b1129bee20867b7d53cb1ced49043a307bed5746cb8e8f88f4deb8fa75d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47415144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e706c95d2533f09fcd570ec7b35fcb92b5c00087434100ae2732517abdc582`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:22 GMT
ADD file:a521640a9f8215118db986479d0ac7e8fae5d186fe5d1c069c166217e63c45a0 in / 
# Thu, 07 Sep 2023 00:48:23 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:48:25 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:665aaf2dc96ac62bc1e5597eccfa5152d16607f9b620eb4b87b2bb76f0c58104`  
		Last Modified: Thu, 07 Sep 2023 00:51:04 GMT  
		Size: 47.4 MB (47414921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b64d6342ccee9704700058f97bc2b29b8d712470c878f1e2c2b29a24893e4d4`  
		Last Modified: Thu, 07 Sep 2023 00:51:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:263d22c0c87a44ad97643ced460b73e56af34c6ad202cfa7c95bacb217271afe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45233428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f0e21a3f727ec10742ea42cfa4bd464469eceaa0d62f76d9f5a89972b5fd2d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:31 GMT
ADD file:33a39c01d7e209fab46b54083ee271e3bdd3d4dccc3a6e8635cbe0989c92c53e in / 
# Thu, 07 Sep 2023 00:57:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:57:39 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4e1ef44b7a1dc38ec98ec01f961a48844fdf07e1ff182d55daae1c01406302a9`  
		Last Modified: Thu, 07 Sep 2023 01:02:04 GMT  
		Size: 45.2 MB (45233200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583885465d66d57fa996caafb06b9b522539ae5abf6e217ff107248de3c42a17`  
		Last Modified: Thu, 07 Sep 2023 01:02:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:aa50c5f0a592d68bb24e34256c982db20542d5575e6f8a990e712175cfd8aa4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49591008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e071f9e05cd05d74a56e98cb7e1fc1d9c938d2732cd6eff487524abc96611d3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:31 GMT
ADD file:f9dd2b1cc0ba261acd8a3e500c54f6b6e0a46131a32988bfd71cf3c6fc5a7d13 in / 
# Thu, 07 Sep 2023 00:39:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:39:34 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fa34261389f3dee2ecffe9bfe38ae7fd05a1908e98a7486354905aee0f648a6e`  
		Last Modified: Thu, 07 Sep 2023 00:42:39 GMT  
		Size: 49.6 MB (49590783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dbadcbcf9b5ac155c53da1ef010715222277e7c1a41193ed1e2afa7fb7871`  
		Last Modified: Thu, 07 Sep 2023 00:42:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:25df26a7eb5cb7bcd5f280c15291722102895ee1833467805258f3627d5c7d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50567483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a08cf61adc01354d724ccdb71c96aa48a7e5af44b562910719ce612bbe84b7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:38:49 GMT
ADD file:8f184a190a3b39f8a44c9c20af46dd27ea11f07138459893b113592302f90a40 in / 
# Thu, 07 Sep 2023 00:38:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:38:53 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:28e9e767fc740145a9fd9e593c7ed9b1ab1ed746324049bf58752d28fa197e5d`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 50.6 MB (50567259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a5144e571763e636e0d55ca4ce624f3661970d36747022b1bde8b0c6e5aa3`  
		Last Modified: Thu, 07 Sep 2023 00:43:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:45224158dc5b1fe786c5a4f81d52553030c64ecc12ad3aab8fa6cee9ee7ecac0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0742d9a6139c31c9fb698acf1ec816416e55bd6a6ae439f2e52cc16ae2319b9b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:08:33 GMT
ADD file:b12d5f9bfd6066e8e4df916aff636c5fc50b1cbd9011b061f050f9616c5a4700 in / 
# Thu, 07 Sep 2023 01:08:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:08:50 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5432e7fe6622506d41a4904c6c8f24ffc691cc53e107e3188eb4e22c6a42f952`  
		Last Modified: Thu, 07 Sep 2023 01:19:30 GMT  
		Size: 49.5 MB (49542026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d469156c84e9265c9c5e4cb8f9bcb32b2432a1250ca3c38a66567894b685435`  
		Last Modified: Thu, 07 Sep 2023 01:19:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1530dc43197d8c1a8b06a5013c99ebaeea25c912559cbc63a74da6a0954dc562
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53543018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a671b0789ec3c17180ca82bd3cf968b720c9d318c6cfa08f30a9669dfe43b0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:05 GMT
ADD file:6b551a78d2b6f2d4f084d05918af6122d7f74823ce34abf0cf00e86cc06e6745 in / 
# Thu, 07 Sep 2023 00:17:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:17:19 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0087e59a1d2f549a5e65d871eac329d942a8b2b458212039d53f135168196e0d`  
		Last Modified: Thu, 07 Sep 2023 00:22:54 GMT  
		Size: 53.5 MB (53542790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5926906929fd1138328d79eacdf080ca8121109b8a8010a06ae140e83c2dab`  
		Last Modified: Thu, 07 Sep 2023 00:23:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:5d3f6c7f67ca88f64f46d9895ee05827d8d584058dcf3ec88f515fd5ddc03ecd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47922214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bdb7f6de8739c37334cbbb676af32b29ff0341c4d9e7e0d495a97b01432a050`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:43:05 GMT
ADD file:b24f18eeabdca57806be7cfa8dd6a173a7448efe4c914018c8f2b2f11f973a75 in / 
# Thu, 07 Sep 2023 00:43:16 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:43:25 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:057281f9e836e5a46ec8be5758de3606940b3a68408826bb8ce7a512f3cb0e70`  
		Last Modified: Thu, 07 Sep 2023 00:49:22 GMT  
		Size: 47.9 MB (47921986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aae2e4fff81ab823349380cbbf73b5e79af43b00d88a317a94418ff8805da4`  
		Last Modified: Thu, 07 Sep 2023 00:49:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
