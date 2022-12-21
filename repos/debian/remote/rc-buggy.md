## `debian:rc-buggy`

```console
$ docker pull debian@sha256:a1e2ca831bc0960bfe3173f842f6c8d96338c79202206b7c8a247bbbef985a03
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:beed1bc40f3a42cc835967f902024f96b77a63130fe3d301e61ce93570f7fcf4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50309842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0065aa53d6e64371638b26bc2e0f4342972997abc9be0d740b8db5f9596342f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:52 GMT
ADD file:643fde45a6d11f36b1178a022667e74288e58a263ac7999c7cb023cb3fcde3a8 in / 
# Tue, 06 Dec 2022 01:21:53 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:23:17 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f8db6e5cd5802a750fd04af4eb64a857f779b9c2333d2d830a50d7b2983365c1`  
		Last Modified: Tue, 06 Dec 2022 01:26:42 GMT  
		Size: 50.3 MB (50309617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bd79a09b54a4468803a36d923e1be394841a689300dc97531f4bb2199dcbc8`  
		Last Modified: Tue, 06 Dec 2022 01:28:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:3f73dbe6d0b746dce7afa9d2052b1b877500251e2e947cf2551fed4f2c349d2f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49284036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d73d6c06e2cee934662c0a5ac0e51325c34ca839e0a7b11ae82eef572d67ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:41 GMT
ADD file:2ae6125a895056caf86a0ea412a141fc00bb6485fece6b14db7232b3e06e9849 in / 
# Tue, 06 Dec 2022 01:49:42 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:51:29 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:597e07fd6304947f2f5075e2d3adcf596e2fc483cd39c89bb38d405526e7277b`  
		Last Modified: Tue, 06 Dec 2022 01:55:00 GMT  
		Size: 49.3 MB (49283811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059e3b956241afb9169acea2e0d6dff56eb8358fa3e2bbe308afd9387ec01258`  
		Last Modified: Tue, 06 Dec 2022 01:57:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:ffb7ff70350244e1c96f5a4576a3b43898ae6cd198c9e21734fd0de8989d99da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47097256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827b9845683cd2eb266e4749910390fddf63f59c929364fce7578b9de162a0fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:00:16 GMT
ADD file:093cea1a330b5b622916fc88f1590ffa3550c325a154b1252e373bcc62c2d8f8 in / 
# Tue, 06 Dec 2022 01:00:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:02:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8d49421b71b8e5160d614ec1ebf9631e35648ff6ac4faf9dea1dd1f58c66a799`  
		Last Modified: Tue, 06 Dec 2022 01:07:59 GMT  
		Size: 47.1 MB (47097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a412fd05e57ce5a9ac918db70b6a0b53b9211faaef3ad6b8eb1a113f8257ef6b`  
		Last Modified: Tue, 06 Dec 2022 01:10:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7df4c00a58d3fd475050e1ddf7b52578189636bdcc5ef3fac2dbf227ee74fc14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50356951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea4bd4d7bd04ca587ee2193aae83ce52f96e803c238872d19fe542873733065`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:58 GMT
ADD file:465db2e68facfda9a8a0c90d74ca46eaa4c6678539ba23e8b95ed5245b4c014b in / 
# Tue, 06 Dec 2022 01:40:59 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:41:59 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4eadaf994967069fdc4c6fb0c34ba7ff8466eb883bc166d386d6891cfde0d540`  
		Last Modified: Tue, 06 Dec 2022 01:45:23 GMT  
		Size: 50.4 MB (50356726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d79f227f057d92fe5434ed1859befb3b0a5ab0ff32775ba87d5ff4a82d792a`  
		Last Modified: Tue, 06 Dec 2022 01:47:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:6748858e520c7835a7ad2151cfa74d064eaad1d5bd0633a8e59caeb1737e027a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51359198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5603dac89e88087ba1b105c1d3157d45732ef8325c9fdc53c4d3256574b2dd37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:02 GMT
ADD file:0909d182d8916b1b37783d0c3582c9d3f3edddf6cd27e90100343ed0462c9c75 in / 
# Tue, 06 Dec 2022 01:41:03 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:42:47 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1cd5a2a4c5902ff854cd1178702a69271f9bf768ae5b99124c16b51e5c2d42a1`  
		Last Modified: Tue, 06 Dec 2022 01:47:24 GMT  
		Size: 51.4 MB (51358972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10755fb2b693d55110d4f6237bc34b882556451a9cb97b5c6d945b060f9af53b`  
		Last Modified: Tue, 06 Dec 2022 01:49:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:4784b4da74e5ecd7649c797bcd5566fc636793e2863c92cd68c8459bd1099858
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50293174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f39fd58d2a9059103f0965bf008d54f6129deae35b424bc4f1e9bc33d0026f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:11:07 GMT
ADD file:bc4f0f717f54bc1982dd6d104f684f180c7b8da660351e5be4853a56b38e374f in / 
# Wed, 21 Dec 2022 01:11:13 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:15:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:22a773956e0933f1a01038ae977c7c99f46cd5ce02f672c66be9a1c837de4eac`  
		Last Modified: Wed, 21 Dec 2022 01:19:25 GMT  
		Size: 50.3 MB (50292945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbac5846049f646e00726b2427a9325410332fa41ecad99b2ef194b4565aa11`  
		Last Modified: Wed, 21 Dec 2022 01:23:57 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:bdebc967c838bdeb57625c533682f1c4b07277a81911761b391378876b6d0b58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54333215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798b316c2494544076a927932f48584f1da97a100633e960dda0196e47496a3b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:58 GMT
ADD file:4af1feaa33ee2a3c1112b5ed0efbcccec637c4dc23a5af7d55343f6ab7005920 in / 
# Wed, 21 Dec 2022 01:18:01 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:20:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:47dc200f753ddc67a9fec80382c7c2b6f164cb907748c309862373fa8d94c504`  
		Last Modified: Wed, 21 Dec 2022 01:23:50 GMT  
		Size: 54.3 MB (54332986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56334aaa76047ddce75ea1b17b7bc1c38062b9c34153037287836794ea5eb5d5`  
		Last Modified: Wed, 21 Dec 2022 01:26:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:cb7d8b71ed0a8cbf7c433d1b7c0045fdf467197ede026c6ad9efc55a382f431e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48699856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e4b319dd4f03a8c1ba0670af9e62141bf503b41063592706b1760b7a7bb914e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:23 GMT
ADD file:9c101517ec1598b49e898a5a60ee79d12ae039f3da76a37f4b9ecc5211ece070 in / 
# Tue, 06 Dec 2022 01:43:30 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:46:24 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:377056d01f15b8c008b4b2d5e74aef86cd1b3c25771df79e7a3d4592cbbee6d3`  
		Last Modified: Tue, 06 Dec 2022 01:49:02 GMT  
		Size: 48.7 MB (48699631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9075a7c2d4b4ea2fcb0d198c6763f6079f15c528955942da00b46b0122fb30b2`  
		Last Modified: Tue, 06 Dec 2022 01:50:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
