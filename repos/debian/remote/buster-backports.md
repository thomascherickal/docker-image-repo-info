## `debian:buster-backports`

```console
$ docker pull debian@sha256:40cf38f01b7e78a2cda8b4fb5b77d2d3b92d71b183acd57cee4a59e059146d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:2a45c77aaa39f91546f679fb2e21ba76e50a6d9679a2b26e9d3665761772a4f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3572aa58c91d68f52ed0b614fee01a1365a66a3b1d02e1e97dd8236f5aff40`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:47:10 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3ac8075bf8eae0bbd2c0b7b2d32b92957cdd8cb7ff153484ca834084ba7002`  
		Last Modified: Tue, 02 May 2023 23:50:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ad905e12f7eb4d48c0e7b334cc5d5d7ede39267238bd62ce471809b9cf3f978c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1080ce8592f12d40b5dd4e8f55921cd882c53305f5d7f5acbf49adcc5e052a3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:07 GMT
ADD file:74b52d80515b2979b2bff8c2728f69628ac807640a577b25413dc0b78f4beb4a in / 
# Tue, 02 May 2023 23:48:07 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:48:11 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4a27c159ac2b737e1d483c37cee9c17e75a5d0ef0c98efbb30d12bd873bf30b2`  
		Last Modified: Tue, 02 May 2023 23:51:48 GMT  
		Size: 45.9 MB (45916301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5269048bdb884662e54237cac49c8f224375840ef7c7fa501ebea141c46f5c8`  
		Last Modified: Tue, 02 May 2023 23:52:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:38909b012e9e8c35d0eab4f3338c518017fc77e1a777ae2d2b74956c778d6f1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49238857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61f55313c7fd443c984898caf97abcd0259698009e03986fcd18c489f662c39`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:39:58 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891ba131a68a92f4849170a28e165e333c613ec38c29fd8cee9ae4f4a8e85456`  
		Last Modified: Wed, 12 Apr 2023 00:43:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:2ac8f3f0c999451d65508a45164804087bcd1675509905d155c6624790372b75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eaeed5d34f838e91c7299ee4e071340e2bc1941fa6fce3fa487ac5a34dd60d8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:10 GMT
ADD file:d427d53c0d42e21426b53d60a17dd7014d2504084ae758c35f088cee043ff9ed in / 
# Wed, 03 May 2023 00:01:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:01:15 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cc3c764404274f8a6e2edf459bc863892205283aa5069a204e16cce54455cb83`  
		Last Modified: Wed, 03 May 2023 00:05:33 GMT  
		Size: 51.2 MB (51206158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8909d3f97915d934c54147522e9397d42fbaf9b5721e68a028b2dd05589ed698`  
		Last Modified: Wed, 03 May 2023 00:05:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
