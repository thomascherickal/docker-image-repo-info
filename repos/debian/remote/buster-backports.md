## `debian:buster-backports`

```console
$ docker pull debian@sha256:1f892a53f2d5d7f9fdc089ecda5689c194c86d9488aec5fd2043a1613dea279d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:f1c841f010fb4b92574498ef3cf1c1517372cd58ef50fade038ab8b67c4fceee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50449118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c95cb7424b265d8f6428a4830cf5d8ff15fc68bc95ca13c2b02521c09cbfdd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:20:45 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683ee599e8123b9a35ffb7411ebd349afd9da427124a5dca2da6a35eae012b6e`  
		Last Modified: Wed, 21 Dec 2022 01:25:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a564114b5685a1ecae78ad6ae5e9062fb2dcb984856618de792e072ab4e0ade1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f619026b2b4ab16f482d97c66c212048ffa6db6d8572003fafe30cb2e60f278`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:59:07 GMT
ADD file:ee219183e8f6a070cc7dfe54397117bf655fa7e49d4a4bdf4263def0bf115d26 in / 
# Tue, 06 Dec 2022 00:59:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 00:59:16 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9b267c960f47219a48e4194e0bb9cf819bb30aeae42c7f03732421b84855f2d3`  
		Last Modified: Tue, 06 Dec 2022 01:06:29 GMT  
		Size: 45.9 MB (45915455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daecaf52883e99cfc8ebb5a7a0ef9c38cae3f674f52286c5d6ae7a238fcf580c`  
		Last Modified: Tue, 06 Dec 2022 01:06:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:347ff713eca13f916ad2a4af19659d31ea4a0097e02757b7a93e0aec4f3dde77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49233962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109b66fde36e354bf683e127f3d63643f49297d4384d8db0c64978212c249f2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:24 GMT
ADD file:2deba7c04e28d01997b865f366cdc8d38a80aa39720c4e4d1fc581ac17e8ce4a in / 
# Tue, 06 Dec 2022 01:40:25 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:28 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:47d0ec2abdb05569eada58143acd16d47ee4b07a33535544cf5bf267bde20cc3`  
		Last Modified: Tue, 06 Dec 2022 01:44:13 GMT  
		Size: 49.2 MB (49233737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959e6b03d1c9dd1ba642fd9a93dbd9e870e939c455c910317ac5f87c2f6a2941`  
		Last Modified: Tue, 06 Dec 2022 01:44:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:c5dce69b2596878b84756cfbc16a7f1f55a393a09f9578dd0861e8355bdc6584
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6333da1d6c1a183c96bc475f3a08432839eb1c15aa988833e9703a3669a71e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:05 GMT
ADD file:0688532a537bb23756917f3d062da18668cd55041d0ae6610cff386043ffbdd3 in / 
# Tue, 06 Dec 2022 01:40:05 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:12 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54f3d93b8ab6f3a5195d99724d5bc911156006687d577448bd8e94d2fe049d4a`  
		Last Modified: Tue, 06 Dec 2022 01:46:02 GMT  
		Size: 51.2 MB (51207714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665433890a98af151c524b8eca3cca8277ef010587edc0a06eecffac864673d5`  
		Last Modified: Tue, 06 Dec 2022 01:46:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
