## `debian:buster-backports`

```console
$ docker pull debian@sha256:4982136ca605758ec2f9a35406897ff51b8a7b4dc2d425aa1ba09d21aaf6f141
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:d4268a709e6e617162956af83b9c39bc40865e63d24a2244456b3a05d0e0665c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50390547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b48824d2f04558bad6d11fbb532f45883c938ff3716b3aff0ba494b1a4ab93f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:03:22 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936de6e8858a96e95847ceab43868e6502d40d78e6098ba3d250f5dde0aba5f0`  
		Last Modified: Wed, 22 Jul 2020 02:09:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f6a061056098f30a1dbfaf2a35baa46f6a2bac3338945fbc7112046a85f2f67b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48107503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35cccaf382e06cd022cc69e4b649eefc06958b1eb5d7c8ae35865ef8d932bfb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:50:16 GMT
ADD file:0431730a3850ee2a710a03ba04d05224938cf2f5318e1f73ed74677c70d09b78 in / 
# Wed, 22 Jul 2020 00:50:20 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:50:34 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:71cf5632cfeb30dc5a7a7ccd4742a02af636cd970ef3a45bebc17d3f20b3662d`  
		Last Modified: Wed, 22 Jul 2020 00:58:30 GMT  
		Size: 48.1 MB (48107278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d01dc7347f9660078962454783ef449ed4a7d5bbe114be1efede66dcf70a87`  
		Last Modified: Wed, 22 Jul 2020 00:58:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:59a1c662902ca947a81aece34c99a7d198b86d407e846caf20a1483524219072
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45868939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585434e4c562b4fa69b05f4135e8beb583879273f882819744946aa77b06d2de`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:18:19 GMT
ADD file:38965defa0df84392a8ff562c2fa6393fe8d42f65f85591c07a581d694eebc30 in / 
# Wed, 22 Jul 2020 01:18:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:19:10 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f890282b0ef00faf11d62374bcdfc54ca574d085127c66977d9a08ab80978a98`  
		Last Modified: Wed, 22 Jul 2020 01:40:13 GMT  
		Size: 45.9 MB (45868714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de4fc60eecb564517114f86d8ade92a26a7c277be3755cf0abc8fd9b63beaf4`  
		Last Modified: Wed, 22 Jul 2020 01:40:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:81a4fa1730fa593405393d4cad7bb09408a2982bcf43c5e9af35c08112d54376
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49168697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74a87f380287b1507356e08f6624cc0017b3e17438f15791263aa01f9e78bb04`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:40:37 GMT
ADD file:14b8dca0bc0e6dae2f0bdb018a3a4e6d8d041abd03d118ae27cf7a72668f4970 in / 
# Wed, 22 Jul 2020 00:40:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:40:52 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e2b2cb832ad58353bcc4edbdd16023beb64ec7856b469d202975f8de836c6906`  
		Last Modified: Wed, 22 Jul 2020 00:47:20 GMT  
		Size: 49.2 MB (49168473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d933e084432f1193630a87f9027318925c63338de97da3a41fd6dcc2a70247cc`  
		Last Modified: Wed, 22 Jul 2020 00:47:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:0b4f0193ae742848ee80522dd4ac3d7dc2493b6417e02af596d532e74f30670b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51157421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c94f445ecf76e3f86b510417676c6f511533157f56b82817d5fd95ed1a734`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:08:55 GMT
ADD file:2f4b8d9ab41b6e158f5926883b6bffdab1757086d903f3f0244f75bafc2e4876 in / 
# Wed, 22 Jul 2020 02:08:56 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:09:02 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:88151d2519867746e4945a0a06b45430b9ddc2ae4be7e7f927cc00e3f640290d`  
		Last Modified: Wed, 22 Jul 2020 02:15:24 GMT  
		Size: 51.2 MB (51157197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da41a66b70bc55969b90c121b33a3ce095d5dfab44726f83ffa5977c5ddea3ed`  
		Last Modified: Wed, 22 Jul 2020 02:15:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:0fa76a3087d9b65ca64f2c1229b868c0298f5eaf6db70f521c2ebd517f92e168
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49019706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:272ed119a322046a5c934a546ee5d87a7c672e977dc0e6f2c446c515bf34549f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:26 GMT
ADD file:977c467052f70f2e12137d029c9b03878551b1d47fabd10269bb0eefa21dfcf8 in / 
# Wed, 22 Jul 2020 01:09:27 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:09:33 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7c04e94f82f3062ec5b60ae7bab01bf211a4a344fd83f7a014cfce0dea431fe8`  
		Last Modified: Wed, 22 Jul 2020 01:16:02 GMT  
		Size: 49.0 MB (49019482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471ffe6ded478ada975ef12fc7df5095f4c00894b533317b9e5de50f1fb36e5e`  
		Last Modified: Wed, 22 Jul 2020 01:16:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:8b46577265c27d111eb9d2e233c120cdb6de31d368ea988822ecb7ed4275d613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54144129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed54028250e33a930f70ffcfaf32506839e63675d66d0326d2a5f068bca468f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:15:14 GMT
ADD file:3e8bf6319c2535d9da6756a6f316eac0a488312c1297fdd54c9e064959e50da8 in / 
# Wed, 22 Jul 2020 02:15:27 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:47 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c8685784756ef2cf52bfd7aa4cf826bd407c500b8402bd2b5b799a2e734e133`  
		Last Modified: Wed, 22 Jul 2020 02:24:38 GMT  
		Size: 54.1 MB (54143905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0048b93fc049801656899af16405ed3b24c8be97cac43814833b68e6390104`  
		Last Modified: Wed, 22 Jul 2020 02:24:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:672ecf5a0ad5678df90066beca7c5aa61433cb7666a8b7d00daef15dbfa296a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9abaac754f2621df0e777ddfe7219df87d7041b96285a2840ca4fd871f0eead7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:24 GMT
ADD file:e5fcdcbbd996899922beac57e202b7e0895321e07263147e96c6e3b7b811d8a2 in / 
# Wed, 22 Jul 2020 00:42:26 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:42:33 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7ecdd8436fd4d951f4ca002a2aa8b01d427a7c4b535083e3ef0792444053154d`  
		Last Modified: Wed, 22 Jul 2020 00:45:30 GMT  
		Size: 49.0 MB (48966422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0824312526c0b4454fa10d1fd6020094b59cc6db54d40e0ff03b6aa2e4039`  
		Last Modified: Wed, 22 Jul 2020 00:45:40 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
