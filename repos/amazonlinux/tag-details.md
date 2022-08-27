<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220805.0`](#amazonlinux20202208050)
-	[`amazonlinux:2.0.20220805.0-with-sources`](#amazonlinux20202208050-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220802.0`](#amazonlinux2018030202208020)
-	[`amazonlinux:2018.03.0.20220802.0-with-sources`](#amazonlinux2018030202208020-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220824.0`](#amazonlinux20220202208240)
-	[`amazonlinux:2022.0.20220824.0-with-sources`](#amazonlinux20220202208240-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:cc88d1da2efe66faa3b86ef71e70e8b7b52822f1bebdd1dd7b56c7f0e3cbc978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba0ec71b51f66eeb3c2a808f463fa79dffa362de472e3e6c1650b0953471b227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62346886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a9b43a329751b9a765fb6d1e788afb43419119cb4946c578832fb43fb8a84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:4cc664bb668e2e073fb39df0fee7e85317f34850ac7b117fb832a1a3c7b47e06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e904f4b8c4ac1bd2ee165c00d8c0854558b9a799a31c0a265433f1ed453c2970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232eb238b33b7e870dd055314fe8ca6e936ad5f353e199a4f203ec82ca7fe5de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
# Thu, 25 Aug 2022 18:20:10 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-77f3d99b447b0774a1bbba85498486869e097db4118c05994ac137d64f0f07bb.tar.gz"     && echo "c428ed82c12be347f1150a419dc16d997020583bda0f076e10a0f34b88df6363  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb07ac98d11436de390efdab7fd63c37b7afabc8b88176ca190a39ba9a6cb12`  
		Last Modified: Thu, 25 Aug 2022 18:21:18 GMT  
		Size: 452.7 MB (452687867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:cb8a67164376ecca3b9993e6bb7d81dd868b7836d2631582becd140c8edf27bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba4ab64a757797930ebb0cf40a41da433cb0531877a3a2376f5427e3fdf93694
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62326701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc3c7c96b1d69f2b9020171c7e70a15f593badacfc228681fe444bf6a91ba31`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ab12022e1a7cd318058af138291d638b1024dcb9844799e8014e6e37d0b35831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63938765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c59c262be8ebd1b4918c0709fa529587d5205204a85c86be6c30b2ac224d19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:727b7a8805501dc38648a16431d2d4c6136ab77e60b7f7cb49e15f9ba7475573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ebc7a9ebb2ba9656d6920f56a073180deedb98a1dd29ea610c23031b4e3675d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486386311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26271b4deed179429c8424f71f5dbdd8eb43b3b6dcb2dd1c3445c88965a2973`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:19:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7044045b0dc596262fa74890fc28afbae5fd0b30081b116d13cffa87ee29041b`  
		Last Modified: Fri, 26 Aug 2022 01:21:05 GMT  
		Size: 424.1 MB (424059610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c91344e903d6bea0fb98c8df86886491a013958ab957eb55a08e4a898727543f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487998330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e17a9a6ede56b90857d5d422629dfecd2d2153eb3bf752bb71ae038541217232`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 00:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6532db54d15f6c38e8c6535dea038b0e4354712e588e1424d2f035a863896`  
		Last Modified: Fri, 26 Aug 2022 00:41:14 GMT  
		Size: 424.1 MB (424059565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220805.0`

```console
$ docker pull amazonlinux@sha256:cb8a67164376ecca3b9993e6bb7d81dd868b7836d2631582becd140c8edf27bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220805.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba4ab64a757797930ebb0cf40a41da433cb0531877a3a2376f5427e3fdf93694
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62326701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc3c7c96b1d69f2b9020171c7e70a15f593badacfc228681fe444bf6a91ba31`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220805.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ab12022e1a7cd318058af138291d638b1024dcb9844799e8014e6e37d0b35831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63938765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c59c262be8ebd1b4918c0709fa529587d5205204a85c86be6c30b2ac224d19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220805.0-with-sources`

```console
$ docker pull amazonlinux@sha256:727b7a8805501dc38648a16431d2d4c6136ab77e60b7f7cb49e15f9ba7475573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220805.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ebc7a9ebb2ba9656d6920f56a073180deedb98a1dd29ea610c23031b4e3675d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486386311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26271b4deed179429c8424f71f5dbdd8eb43b3b6dcb2dd1c3445c88965a2973`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:19:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7044045b0dc596262fa74890fc28afbae5fd0b30081b116d13cffa87ee29041b`  
		Last Modified: Fri, 26 Aug 2022 01:21:05 GMT  
		Size: 424.1 MB (424059610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220805.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c91344e903d6bea0fb98c8df86886491a013958ab957eb55a08e4a898727543f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487998330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e17a9a6ede56b90857d5d422629dfecd2d2153eb3bf752bb71ae038541217232`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 00:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6532db54d15f6c38e8c6535dea038b0e4354712e588e1424d2f035a863896`  
		Last Modified: Fri, 26 Aug 2022 00:41:14 GMT  
		Size: 424.1 MB (424059565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:cc88d1da2efe66faa3b86ef71e70e8b7b52822f1bebdd1dd7b56c7f0e3cbc978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba0ec71b51f66eeb3c2a808f463fa79dffa362de472e3e6c1650b0953471b227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62346886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a9b43a329751b9a765fb6d1e788afb43419119cb4946c578832fb43fb8a84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:4cc664bb668e2e073fb39df0fee7e85317f34850ac7b117fb832a1a3c7b47e06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e904f4b8c4ac1bd2ee165c00d8c0854558b9a799a31c0a265433f1ed453c2970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232eb238b33b7e870dd055314fe8ca6e936ad5f353e199a4f203ec82ca7fe5de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
# Thu, 25 Aug 2022 18:20:10 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-77f3d99b447b0774a1bbba85498486869e097db4118c05994ac137d64f0f07bb.tar.gz"     && echo "c428ed82c12be347f1150a419dc16d997020583bda0f076e10a0f34b88df6363  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb07ac98d11436de390efdab7fd63c37b7afabc8b88176ca190a39ba9a6cb12`  
		Last Modified: Thu, 25 Aug 2022 18:21:18 GMT  
		Size: 452.7 MB (452687867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220802.0`

```console
$ docker pull amazonlinux@sha256:cc88d1da2efe66faa3b86ef71e70e8b7b52822f1bebdd1dd7b56c7f0e3cbc978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220802.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba0ec71b51f66eeb3c2a808f463fa79dffa362de472e3e6c1650b0953471b227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62346886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a9b43a329751b9a765fb6d1e788afb43419119cb4946c578832fb43fb8a84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220802.0-with-sources`

```console
$ docker pull amazonlinux@sha256:4cc664bb668e2e073fb39df0fee7e85317f34850ac7b117fb832a1a3c7b47e06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220802.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e904f4b8c4ac1bd2ee165c00d8c0854558b9a799a31c0a265433f1ed453c2970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232eb238b33b7e870dd055314fe8ca6e936ad5f353e199a4f203ec82ca7fe5de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
# Thu, 25 Aug 2022 18:20:10 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-77f3d99b447b0774a1bbba85498486869e097db4118c05994ac137d64f0f07bb.tar.gz"     && echo "c428ed82c12be347f1150a419dc16d997020583bda0f076e10a0f34b88df6363  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb07ac98d11436de390efdab7fd63c37b7afabc8b88176ca190a39ba9a6cb12`  
		Last Modified: Thu, 25 Aug 2022 18:21:18 GMT  
		Size: 452.7 MB (452687867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:da0503b195a86a22590490b43fceaf5d084e2fdf5a60f93601ac1110c0745b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9465edead9ce0b43ed345bb644d366b86f319489a959eb49ba82d69819d23e96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57847954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09619965f1eaa32ffc4f45daccfab155d54877122d5db43fcd070a0afe380eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4926ef5cb139d826b412559e3f4315f151c1a880aaa0897bb17af1d2d0a20d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56655810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b06fe2608cd55d0b5fdca91110499f96e16458074d657327683d884f74d0c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:61d64e5da27768b5a126323c21ab45af592b97b9059379e161ee65b518e7a1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:09f68631d352dbbc0ef6e000377d5e56a27dc75dd951f60725d2a79e77ea9365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392639400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f59eb1c10d8578a73d0c3b21bf56d2d5ab5bf75fd6ea9af919e56fbf326b95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 01:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baebcc8b083ea162e526e6e92edcd212831d90f52aaa1a55a963ae53f6c3643c`  
		Last Modified: Sat, 27 Aug 2022 01:21:06 GMT  
		Size: 334.8 MB (334791446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:75d78c546e422833cc587faeed08e7b7b3093f00a235b48c3bf22b05edacd83f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391447216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d033487b80a7f4a4527c99ed7d9e3de7c993e76844a884637194c8715d59078b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 00:39:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5819d824cb1301917d1bccc4ae20350f28fbdfd2a5ff6087ba1d61b7692790f9`  
		Last Modified: Sat, 27 Aug 2022 00:41:20 GMT  
		Size: 334.8 MB (334791406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220824.0`

```console
$ docker pull amazonlinux@sha256:da0503b195a86a22590490b43fceaf5d084e2fdf5a60f93601ac1110c0745b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220824.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9465edead9ce0b43ed345bb644d366b86f319489a959eb49ba82d69819d23e96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57847954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09619965f1eaa32ffc4f45daccfab155d54877122d5db43fcd070a0afe380eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220824.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4926ef5cb139d826b412559e3f4315f151c1a880aaa0897bb17af1d2d0a20d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56655810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b06fe2608cd55d0b5fdca91110499f96e16458074d657327683d884f74d0c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220824.0-with-sources`

```console
$ docker pull amazonlinux@sha256:61d64e5da27768b5a126323c21ab45af592b97b9059379e161ee65b518e7a1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220824.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:09f68631d352dbbc0ef6e000377d5e56a27dc75dd951f60725d2a79e77ea9365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392639400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f59eb1c10d8578a73d0c3b21bf56d2d5ab5bf75fd6ea9af919e56fbf326b95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 01:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baebcc8b083ea162e526e6e92edcd212831d90f52aaa1a55a963ae53f6c3643c`  
		Last Modified: Sat, 27 Aug 2022 01:21:06 GMT  
		Size: 334.8 MB (334791446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220824.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:75d78c546e422833cc587faeed08e7b7b3093f00a235b48c3bf22b05edacd83f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391447216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d033487b80a7f4a4527c99ed7d9e3de7c993e76844a884637194c8715d59078b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 00:39:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5819d824cb1301917d1bccc4ae20350f28fbdfd2a5ff6087ba1d61b7692790f9`  
		Last Modified: Sat, 27 Aug 2022 00:41:20 GMT  
		Size: 334.8 MB (334791406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:da0503b195a86a22590490b43fceaf5d084e2fdf5a60f93601ac1110c0745b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9465edead9ce0b43ed345bb644d366b86f319489a959eb49ba82d69819d23e96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57847954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09619965f1eaa32ffc4f45daccfab155d54877122d5db43fcd070a0afe380eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4926ef5cb139d826b412559e3f4315f151c1a880aaa0897bb17af1d2d0a20d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56655810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b06fe2608cd55d0b5fdca91110499f96e16458074d657327683d884f74d0c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:61d64e5da27768b5a126323c21ab45af592b97b9059379e161ee65b518e7a1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:09f68631d352dbbc0ef6e000377d5e56a27dc75dd951f60725d2a79e77ea9365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392639400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f59eb1c10d8578a73d0c3b21bf56d2d5ab5bf75fd6ea9af919e56fbf326b95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 01:19:45 GMT
ADD file:f5bcad77eda3a4fadcae22e9ddef7f11b6665c9d548c132115c9cb8ddf830460 in / 
# Sat, 27 Aug 2022 01:19:45 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 01:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:69a4baeea4272987d1da3c7f3dcd3779118775ad2dea75d0a4cab21cf1c6dd39`  
		Last Modified: Sat, 27 Aug 2022 01:20:41 GMT  
		Size: 57.8 MB (57847954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baebcc8b083ea162e526e6e92edcd212831d90f52aaa1a55a963ae53f6c3643c`  
		Last Modified: Sat, 27 Aug 2022 01:21:06 GMT  
		Size: 334.8 MB (334791446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:75d78c546e422833cc587faeed08e7b7b3093f00a235b48c3bf22b05edacd83f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391447216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d033487b80a7f4a4527c99ed7d9e3de7c993e76844a884637194c8715d59078b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 27 Aug 2022 00:39:40 GMT
ADD file:abbc2d3867f56393097d8284ff46e7c9ecc0af52d77d6dd7cb07b70f8763f334 in / 
# Sat, 27 Aug 2022 00:39:41 GMT
CMD ["/bin/bash"]
# Sat, 27 Aug 2022 00:39:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-03a90110fe51837aa1391c5016f1db732ab1cb3f6973b4ff09e803a8c043fe3b.tar.gz"     && echo "38c8a1b5cc33a01c0dd2ae38bbbeb18a71e14b260785e2813dfa5b55b764e002  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a1c72534981534008bf958a3bbdbc5c6f1e1b4b1d93030605165a932c3c882e`  
		Last Modified: Sat, 27 Aug 2022 00:40:42 GMT  
		Size: 56.7 MB (56655810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5819d824cb1301917d1bccc4ae20350f28fbdfd2a5ff6087ba1d61b7692790f9`  
		Last Modified: Sat, 27 Aug 2022 00:41:20 GMT  
		Size: 334.8 MB (334791406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:cb8a67164376ecca3b9993e6bb7d81dd868b7836d2631582becd140c8edf27bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba4ab64a757797930ebb0cf40a41da433cb0531877a3a2376f5427e3fdf93694
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62326701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc3c7c96b1d69f2b9020171c7e70a15f593badacfc228681fe444bf6a91ba31`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ab12022e1a7cd318058af138291d638b1024dcb9844799e8014e6e37d0b35831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63938765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c59c262be8ebd1b4918c0709fa529587d5205204a85c86be6c30b2ac224d19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:727b7a8805501dc38648a16431d2d4c6136ab77e60b7f7cb49e15f9ba7475573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ebc7a9ebb2ba9656d6920f56a073180deedb98a1dd29ea610c23031b4e3675d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486386311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26271b4deed179429c8424f71f5dbdd8eb43b3b6dcb2dd1c3445c88965a2973`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:19:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7044045b0dc596262fa74890fc28afbae5fd0b30081b116d13cffa87ee29041b`  
		Last Modified: Fri, 26 Aug 2022 01:21:05 GMT  
		Size: 424.1 MB (424059610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c91344e903d6bea0fb98c8df86886491a013958ab957eb55a08e4a898727543f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487998330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e17a9a6ede56b90857d5d422629dfecd2d2153eb3bf752bb71ae038541217232`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 00:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ee790ea60c4090ba6e215c0d148c239e7806623b75f6f14930ce7e2f6b07f8.tar.gz"     && echo "8b5abb84b1d279d3c26a9c2721b1daa1317ca4109f56f84b032d756c3fab7368  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6532db54d15f6c38e8c6535dea038b0e4354712e588e1424d2f035a863896`  
		Last Modified: Fri, 26 Aug 2022 00:41:14 GMT  
		Size: 424.1 MB (424059565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
