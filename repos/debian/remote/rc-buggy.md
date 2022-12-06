## `debian:rc-buggy`

```console
$ docker pull debian@sha256:d06ff63ea77c5df143bb5870b67c24ce73b393d8056bacc377f7b3840482eaf6
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
$ docker pull debian@sha256:71029589e69069f24a8665268b424f4e9b1509bc21f72d0de9eab428aac45270
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50320062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e659d4871bb263bff4be2d16c2d19678fb07f7eb970e13bd117f3df08350d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:56:07 GMT
ADD file:f0c5ebbf2aa59cd4e0996c808ed4d378c47b86ca4c00f63fa5de02b4cb838334 in / 
# Tue, 06 Dec 2022 01:56:12 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:00:41 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dfb5e33f7f324b83c5e49e84922c9f448eace01382dd0e6ac683debf1a61eb39`  
		Last Modified: Tue, 06 Dec 2022 02:04:23 GMT  
		Size: 50.3 MB (50319836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a793a0afba1cf58ce7858b20f117f3187e6158d9c606a0bcf5e8d5bb87dc5b`  
		Last Modified: Tue, 06 Dec 2022 02:08:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:b392c508867d3e2cc8cad874b6bf66acb8749c10054faf8425fa7c012c609eff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54361384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b661fe7a1df6e294a50b03d6a5e8ef1d63aae06ad1968adb295efcbc56b685e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:26 GMT
ADD file:bdb06f846e6364870996f9ac20fb236d99a0ac4e61f11a82dda8599bbd6ea354 in / 
# Tue, 06 Dec 2022 01:18:29 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:21:05 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7e30927c2af9840769d712ec0a0e33b7ccaba3ec9a715660e8c1b04953084dec`  
		Last Modified: Tue, 06 Dec 2022 01:24:47 GMT  
		Size: 54.4 MB (54361158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566d31afea92658fe57ae15421094eab54da5fcdaba5697fca941bb3d2d44b26`  
		Last Modified: Tue, 06 Dec 2022 01:27:50 GMT  
		Size: 226.0 B  
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
