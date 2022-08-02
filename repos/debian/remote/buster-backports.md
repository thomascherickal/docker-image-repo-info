## `debian:buster-backports`

```console
$ docker pull debian@sha256:2a6d1c3d2f609410defccdb5d3c32893de9e0edb93b5712963bfc096fecb86f0
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:18f0fe0da0fa3a0cb2b4281c3913a3b7d68ae83e54f423cff0c1f04252439d81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50441203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295ece2748cfaa9c7576cddb3f55659f807c539729f74b28f4ae0e99c29c5214`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:14 GMT
ADD file:647206e0e9c1daa306e4ebbdc26c3ef1840dd316ba4ffea905d17b0858e58e34 in / 
# Tue, 02 Aug 2022 01:20:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:17 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e6a53d1988fa8e19db6bcfc96ee6783afb079c38dbe047528e691815d19a9fa`  
		Last Modified: Tue, 02 Aug 2022 01:24:34 GMT  
		Size: 50.4 MB (50440980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a5fc140ac9171f4422d51fc40671f482daaf8a88df678935c2495dcb5867a`  
		Last Modified: Tue, 02 Aug 2022 01:24:49 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:6167d1cf7c45b6b7d0e1374e89a75210745b901a7f2eb95e11d9ffd0fb8b07e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48161123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8ab5239bdc5276576f80d7283a3da87d57c5ac779470e8c4c023228ddb5fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:22 GMT
ADD file:6eb7eae3c77a49928afd356926e1e95fbf200b8e9b6283d3a177e4f165cbb212 in / 
# Tue, 02 Aug 2022 00:49:23 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:49:29 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f14a0b6fcd00792922ff8be006e37d214db8ce1514b4d2d675b1a7490f9c070`  
		Last Modified: Tue, 02 Aug 2022 00:56:35 GMT  
		Size: 48.2 MB (48160901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2c0f5b54a7f8f45bb7e68076d2dc7b8023b982f93ed8258b71809b84072a6c`  
		Last Modified: Tue, 02 Aug 2022 00:56:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:010b00b994017d1c4e1fcb47595412860317c52943b7c91b3254aaa0e7883033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4eacd71b15238fccaf985bfd5f84962980b9646eb51009bedcc2ce7a72618f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:59:20 GMT
ADD file:a2513870e4a875b6ed767406fe446e1a8548d12329dac6681bf0c22b728d7759 in / 
# Tue, 02 Aug 2022 00:59:20 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:59:29 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25546c90dbccc03d19518f394bfd5bd231736bccd81adbc4903a9df5d94722b0`  
		Last Modified: Tue, 02 Aug 2022 01:07:16 GMT  
		Size: 45.9 MB (45915820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28b1ea75be11b49c46a39ebcf59c60185ef077d26a44847c8f68c82b7addeec`  
		Last Modified: Tue, 02 Aug 2022 01:07:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:383f3b30fcae9e314efd79313c69a485601bdee13648da2499731e917591fa65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4779c7889b0e167a5e86d62bc523d9b5ce610170f046423b2f724b89d75ca70c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:40:56 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d21acc4ec7f01836cddccc7bb60f543c395e7d92cb59322a1470c7f2d4f9126`  
		Last Modified: Tue, 02 Aug 2022 00:46:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:270b4b3129c41648ab52d87d626bcee0bc544db048c36f552b241ce9691139f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51204490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6783fc43fb1dd9a8fcd68db9c9b66a54d37d534ab0e7064e9e2ff6f00b7c1fdf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:39:39 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad03746b7e160bc76ca8b78ea72dca4504ec476c0d2246df4c7ef8eef81e89`  
		Last Modified: Tue, 02 Aug 2022 00:46:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:27368670de9babb7f768adb77ff97d0c04084024eb42c563aef327fe4a2f6958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49073411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7658d0e67714be11d7b5e39d3c04cd677bd6dab9259e3a707e12fcc0870fc38a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:11:05 GMT
ADD file:1996972faf38963e8a06898c563fb32f079aa343d24607da2a0803efae84b184 in / 
# Tue, 02 Aug 2022 01:11:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:11:19 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2c64b7f6b71e68178c319218ccefaa5441dc9a6676a6167ac77e662cd2c1ed1d`  
		Last Modified: Tue, 02 Aug 2022 01:21:47 GMT  
		Size: 49.1 MB (49073186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80765c7b9473e3f861c77777b12b72777ad76f6f40de64d6acd990541f0281b2`  
		Last Modified: Tue, 02 Aug 2022 01:22:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:41d1cfffbeaa8b6fddbaebe870a689be607bfe484aa7ff742880b9a14395a919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54177495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885a2091066d5a4eb9a7c864cc15ebbb5862b95ded5d6eeb4ea0104373bb5471`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:45 GMT
ADD file:da978c3b779d7a2f173b2d4e34c1802f3e91a04a2ed19d59bb2f3aa00330e7ef in / 
# Tue, 02 Aug 2022 01:17:48 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:17:55 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a1cfed4a4c5f34287e40a12fceea48d304fea529f815ddc5aba7c54511afe708`  
		Last Modified: Tue, 02 Aug 2022 01:25:10 GMT  
		Size: 54.2 MB (54177273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668713a81517e84e305d6b83d57d6ac15f3c3cecb580d5e72d48a8f347cd150c`  
		Last Modified: Tue, 02 Aug 2022 01:25:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:fd0141519fbf7d5617ebb9dc3a272f2e0009e28b505b7805d9eb25b7558d0c75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49007501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e108777939e018d4b5089e533dafd85e8e789a70ddf0f07be3426d7bbf0ffae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:39 GMT
ADD file:d4184c5029732fe05023927be89b0c768483920c072c2069f92b3f4912c1c09b in / 
# Tue, 02 Aug 2022 00:42:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:48 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8031e15331a0dfcc3509ff9e409d7bbbf567a40367f9eff78effb21b904d39ba`  
		Last Modified: Tue, 02 Aug 2022 00:48:16 GMT  
		Size: 49.0 MB (49007278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6220b50ae985fc9db97d58d223b723819c3c1f2ed6886c09732bd2f7b85b9`  
		Last Modified: Tue, 02 Aug 2022 00:48:26 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
