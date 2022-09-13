## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:45ddc7b05448e6ee7bdcb0f903530f76bfe18404027c90fc2066f1bb5da3076c
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:ef5a26eeba1a37a94fb912d872f4e6102da2497fa9bc4857604609bd683620cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55029957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f449c6373b7eef32ce094109a9c80fc49aee8a89c7fbc96091ca68586c0388e3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:22 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277a7948fcaf80cd66ef2ed676aeec8749ac17cf7f6e1720aab84ee94d34db99`  
		Last Modified: Tue, 13 Sep 2022 01:00:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:45d9b2be7322fccf40a055e3b6323debabc8719428385b21e6377109ea55621d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52532426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0be3585f97264cef6fc90d90a0dca1a3bd48fbec6eec298bf0abfb2744dabed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:03 GMT
ADD file:ad560226d0aa0be51fbe1d98a8877aeb30110956b3a7c0f849a4331e99477ee4 in / 
# Tue, 13 Sep 2022 00:53:04 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:53:15 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f33103174415e8d15c8ebada62aae8327ecba6afa6035819128965eb1a64966e`  
		Last Modified: Tue, 13 Sep 2022 01:00:25 GMT  
		Size: 52.5 MB (52532200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fd4ba27ace9f0994ba76005fe0ecac48b80f8c2d298bcfab83afbb84c4cf35`  
		Last Modified: Tue, 13 Sep 2022 01:00:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c3bf7f366e40fd5d141be6f946019e5eb7b1c0db03fd851fb230aba4f0293756
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50205157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5396e1790210500f28f2b52bd8d04b4d56de78b3ffa66513eb4b58f52c7c69b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:42:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b3fee3ad4cec12be12dbd5654a88627c421f9119d001163e2138a6c381aeaa`  
		Last Modified: Tue, 23 Aug 2022 01:49:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0915b773c2252e793901875e0beffcd7d995515559dbc3da51f5091f9722c98d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53691054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23c0f222ed7ce68b2c2aec54a7b13f80abb48a3b021fa862a5ab426fd858aa7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954eba47fa362dbd171b61147b60d3ff85e9c16ebee6ef8d9cebead61424448f`  
		Last Modified: Tue, 23 Aug 2022 01:57:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:35e091bb7e6991373992b4ed898b50364048a60a33a172d84ab4b10fa3d883f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56012847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08126e8eb23fe5f52031c20b662efb3d473b09721b63b5ef7326111014309f21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:02:32 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08596d09b7ec28d9055e03ed251e68db7a4d43fb8843b0f4df1f77c5b9f9b01`  
		Last Modified: Tue, 23 Aug 2022 01:08:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:06c3a87d4a0993b85824b0149ddd020f3df8868715ef1f21c5591537062a4f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3407dc326b6d00851501a0ac2bcfe6394932451a103953b94316aad28ba9210d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:10:38 GMT
ADD file:a55d19f262e8338f932ce871c1cbc1718f9f74a5002212f38fea74f3858460a9 in / 
# Tue, 23 Aug 2022 00:10:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:10:57 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ce438ccc597187e8a0dab5cc8906e6a0ec75a9320e55225ad2ec24765f7c0b4`  
		Last Modified: Tue, 23 Aug 2022 00:18:51 GMT  
		Size: 53.3 MB (53272999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da963443d7b69c70e9fc774a93fd7d904e556caffca03acbf6cf21cae6a86eb`  
		Last Modified: Tue, 23 Aug 2022 00:19:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a06346f504708d03b5217e1408cbbba53b1b508abe0d05241c886a98b3da1ac4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58909401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:984f49c2645e80d7805801e29d56eb21b1f6c70058796d6f4d9c7be573652663`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:24:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91236e88cb9d5129870955ef5057bd0782cf061738f9d1f94acfd710fbc9d4a8`  
		Last Modified: Tue, 23 Aug 2022 01:30:19 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:c54ec6772696632063206b22a0eebe38723fcd9d4fa09712430ee4d6adddcbd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53265048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313e38eec430b633564f143c4b3d9edb18976f6dac029afbe049d9c29d88f487`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:47:47 GMT
ADD file:2965b342d27ea25d073bb5f216362150cb8ec0e05df43fae8e4ee6251006d17d in / 
# Tue, 13 Sep 2022 00:47:50 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:47:58 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf58bfabf9fb5ab735277c32678e319fed106496e2f1070ac6bcf35a57d3870e`  
		Last Modified: Tue, 13 Sep 2022 00:52:18 GMT  
		Size: 53.3 MB (53264823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dfb8df822f861a1e4de9fa828064417e1e175dbbdc1a87abef55a8215b3033`  
		Last Modified: Tue, 13 Sep 2022 00:52:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
