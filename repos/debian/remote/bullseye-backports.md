## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:a3404886f765a573988e83a1cbbe4c97c617f22c393be387217c5c85fd58eaf9
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
$ docker pull debian@sha256:8e537bd87ce1db0283e6574577bdc61ef57fb7ce73f178fdbb69a90c569d0502
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54942004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ad039cec8f1ebcec7fa8036d1aed21a1d17ee0bddf6cd7987384b1521ff2c6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:43:19 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e039d6f4a08015070e85a9abf46f6133f47a35b90d5cbf3d61c0979e9abe41a`  
		Last Modified: Wed, 20 Apr 2022 04:48:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ae7bd4fd8ea079a3179eb6f18d2e6b95ab6692b4bf69a35c83151283804cad7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52475094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0524ddfeae4b0c149381d12265722125def01788f3664b50b70ed6cc08943c6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:16:05 GMT
ADD file:d668b425e22c8042fc04ca031d5034b01d7488f8b7adf54485b4025fcb8eea77 in / 
# Wed, 20 Apr 2022 07:16:06 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:16:22 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:625ca11644bb62d8db7c0b110e4fd87d4b2b14a21e09653f8ea20ef89a5d2663`  
		Last Modified: Wed, 20 Apr 2022 07:31:39 GMT  
		Size: 52.5 MB (52474869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f95d1ade54dd023eeba89f509dcc07b1a15511885d4ec602f297354021f74`  
		Last Modified: Wed, 20 Apr 2022 07:32:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:63f71f177b81effa8428fe9b48705f49fa6c16205e3e58f1bd54b216c6f06c1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50133923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f327f0aa4e3c1b28d39808f65ae0e9727d6626c1dc4533193f1b30b809306d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:26:39 GMT
ADD file:1c05c50014bbd32a4cf1edd085996a8c62abc3c8969b64d2355475827a07475e in / 
# Wed, 20 Apr 2022 13:26:40 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:26:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0a2c02101ee4340d4a9ebb962e9331486e417a3835c9adefb9badd2f0c116ab6`  
		Last Modified: Wed, 20 Apr 2022 13:42:55 GMT  
		Size: 50.1 MB (50133696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c506110af71156f1de46457aeb7eba0cb5a54241438a1fbefb3bce94f3d6a4`  
		Last Modified: Wed, 20 Apr 2022 13:43:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e0e73ebac447b048749639ffcd4f53e4cd8bb4a2f9abe5b6c259ce7012cf563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53633319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88661b991c2e33f8c52c0e286923f37dba092523a95fa42ae3a5adf650d5db4f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:29:02 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f62352badf9a0f962790e6fd7f921e93911eb5643361b1ea3a73cccca6237d`  
		Last Modified: Wed, 20 Apr 2022 04:35:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:c4398e1e88771afea7eeb7600945a6ebc03d94b3a88e856cc8a739ed26002f18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55940945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16d46e42a5abb2035bd0575ab59df147257b0632d41ba6c3c15a458e3d642cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:18 GMT
ADD file:81b79bac6ad02f2b0e2d30c005dac5f38d58fc7e12d7466c6704bc8a8980a0ef in / 
# Wed, 20 Apr 2022 07:37:19 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:37:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:03830d6b0d2ecb0a7f823997ff6629d0ff36a821ec317f6d5644d08b1870d936`  
		Last Modified: Wed, 20 Apr 2022 07:44:23 GMT  
		Size: 55.9 MB (55940721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91216565f5b55f1eb08576cd574486baf91f11d004c2a1222ebedc6774a1373f`  
		Last Modified: Wed, 20 Apr 2022 07:44:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:466f0188e3d62ca9f4d8afc375904f5697300a3ed5714414d6e22ab952d87018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53203532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81741c5037ee255f9785ab7d629ebb76f617df61fb08dde8d219b4bba41b5f98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 14:27:54 GMT
ADD file:8150012d71535a0807e6b7f0bb9f31dcef864730e1df2362a20fb269ccc902a2 in / 
# Wed, 20 Apr 2022 14:27:59 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:28:13 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:774a3fd0175393ffcac86ec5a65f3f57dfe09f9c38a55812cb69c85281394d6a`  
		Last Modified: Wed, 20 Apr 2022 14:38:35 GMT  
		Size: 53.2 MB (53203304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b7943a35743fe22953e86f5476c1b72df3da509dde09fa503a38585a1d2327`  
		Last Modified: Wed, 20 Apr 2022 14:38:51 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:6bd5a0b038824a8795dafd8534ee276c63404305aedf8d272116900093ba3751
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58835561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8128369f787c43a816682088c9f00ae949837a14a328fb9b53f543a5e94332cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:45:51 GMT
ADD file:2fff7021563ff08bee97c626d3c91410f8f8dc3213b548a7e8b0c351557c7f1d in / 
# Wed, 20 Apr 2022 09:46:01 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:46:19 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:09c77622a2c385ed83fadca4a945b0065fdeaaac427ce2b1a9e795ce2007f8c3`  
		Last Modified: Wed, 20 Apr 2022 09:56:19 GMT  
		Size: 58.8 MB (58835334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a790d78cda5f995ef3d7cf2b6a40d50b0ca5da573801bb9c2b7f1d2d0ceca`  
		Last Modified: Wed, 20 Apr 2022 09:56:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:c952d0601045d64b602ca80b027613c236c033b661f6de05f7783b24553e8ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccd90758145f47e4b42c7e35b3c6b87d49c40eb82fa7bd3d2d46fe2f61576318`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:00 GMT
ADD file:82d4840cdb4b0211b2191ba71ea2698d8dc1b05554d7ed1499aca9cbafaa3fc8 in / 
# Wed, 20 Apr 2022 08:39:07 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:39:18 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bec7f58dd40ec15934a767db84e5e9b88704cefe60ebe4d7f5abc1583f6c060c`  
		Last Modified: Wed, 20 Apr 2022 08:49:18 GMT  
		Size: 53.2 MB (53207374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d829b9e4f82b4e1f88df842c36d133c1290c6e2f5794f518006a93b2d0d5ddb`  
		Last Modified: Wed, 20 Apr 2022 08:49:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
