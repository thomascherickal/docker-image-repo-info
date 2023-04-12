## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:74450789489cdeec1e9ae2a8ce87a37efc80ce095381e058b4723b49b652dd05
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
$ docker pull debian@sha256:3950fa6c3d923f7929c4e08231d72abaee40420cc7798d78c823a161c2cbf0f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55052961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72e890b198a7f9ae8a9907a7f5950cf254bd7c658e9980e88bf9c69c5f74800`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:19:59 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd102085f0f28e20f71187d0f003b7d02edd9a13fdee8001aad360df3ca94df`  
		Last Modified: Wed, 12 Apr 2023 00:23:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:5e2fc48e4bc30f6107c72618457618da37c6dd5ca98ef19fb2254a93ab9c8e98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52549780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f49c82de2b1caa290083ec6019e958d398a23760aba723efcebd8c01b29281`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:37 GMT
ADD file:8419f4bee11379b8aa511da1fe7cdcd6b2cb8c252bc90f76dec672a5b802ea27 in / 
# Thu, 23 Mar 2023 00:48:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:48:39 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a8ea6c28ff9e1b5a437e1e5b168873207139672ec8d755939cad00b23349e22`  
		Last Modified: Thu, 23 Mar 2023 02:21:35 GMT  
		Size: 52.5 MB (52549555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69816ee3daa48201de0a8386cf1501eddf766583836a74d035bd2969bb679ba`  
		Last Modified: Thu, 23 Mar 2023 02:21:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:63e41b11b53d39265994fb5b1b81c43ed0d49320a92f27d5a47ef1ecf4306e0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50217110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a3d84d0562e2dbcdf040560adbc51181885f294e5f6e9a1bff941f68a92814`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 11 Apr 2023 23:59:38 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a1996a22b675eefd3fce9f8b70de051d1433a66b77748d11c2d18115e8a4d`  
		Last Modified: Wed, 12 Apr 2023 00:03:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c8660693dab64baea85b7f953e93c0480f16100ff1ddd7bf40dac2eb3b60b1d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53703325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9177fc6915502ac07e2d3e9950cb3024bae81549d9a4ddd17fb42b1eb09fcac6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:05 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4321f724ec4103a60b8da16d123240593e023dd1ca36e9790676e6575ad7ea`  
		Last Modified: Thu, 23 Mar 2023 00:48:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:9b61749c8b1ee17a4ee71e23e0b31539f16653343af9a2756bcf86b45690d559
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56028136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab32b4bdda8b36bc50d177f322c9fd3ce2a5f84fad78c04322bbc3ffda489c6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:08 GMT
ADD file:f331251c4c21fceff56d13f76442a6334dc355c29ec7450768c1c86a3db1adab in / 
# Thu, 23 Mar 2023 00:39:09 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:39:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c1bb878cff31d37952c5c73ed15c167f599bb7f97b3eeaa1a17352b2473b3394`  
		Last Modified: Thu, 23 Mar 2023 00:42:44 GMT  
		Size: 56.0 MB (56027911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54a68987940f3f6609b73654acb8468ef9df8b07dbbd85d0100cfe346cf541`  
		Last Modified: Thu, 23 Mar 2023 00:42:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:6bba04ef78172e50a76a1adeae6948d95da13d2b10947194a1e133be255246e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53272249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82192e5ae21def8646a916631d34811734eb115466795c16169066406cdb4574`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:26 GMT
ADD file:5d2c839055739fe92d64098c09607e7ec9123101d15f837c54f3688755af0c23 in / 
# Wed, 12 Apr 2023 00:09:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:09:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:80243e355b05bee53c6acc45ace2cde4f7495dafe9f3f8d7d299ed51d04928d2`  
		Last Modified: Wed, 12 Apr 2023 00:16:48 GMT  
		Size: 53.3 MB (53272023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c557479b9edd028d1b34e5256f9070b200d4fce958cf9e84613c83dea79c0`  
		Last Modified: Wed, 12 Apr 2023 00:17:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:0dcf75aa727af3bf39e300f0e936e662682d6243c4e67f3701c9d00501bd3654
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58926827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5edd0906c02fc00f201665e4a5b81026c9c7dec72fca0b3a17050d22791895`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:07:58 GMT
ADD file:c3c2a10473ddaa3d8a30ca99b19ad3599d0e60d826c4e0315bdb7463352ebc09 in / 
# Wed, 12 Apr 2023 00:08:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:08:07 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2d3ffdd4610a019889b845cc82b3d956ad85cca78ad4bff2d5e5522bd02c17e7`  
		Last Modified: Wed, 12 Apr 2023 00:12:37 GMT  
		Size: 58.9 MB (58926600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78baafc7df2db64930490d209b66bee4bd2f7845f03591a93f95be17fe677f1`  
		Last Modified: Wed, 12 Apr 2023 00:12:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:0e4c0a91f063aa664e5393b1c602a2121fef4fdc1b375e6bac354961019eb77c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53286910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55d666fcb5965f2338b94392975cb40f61b7a40d568169be8f119d160f5bca9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:00:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f8ea362068477a4e1f3dc8e71b20734f89fdc76fa216834c78d37b4ff337c`  
		Last Modified: Wed, 12 Apr 2023 00:05:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
