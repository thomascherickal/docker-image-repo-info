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
-	[`amazonlinux:2022.0.20220831.1`](#amazonlinux20220202208311)
-	[`amazonlinux:2022.0.20220831.1-with-sources`](#amazonlinux20220202208311-with-sources)
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
$ docker pull amazonlinux@sha256:d26e31b5b4bb811a12cb868453a980a9ae53338020130521b67068cec9cabcc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7301b45cf224105e4892bd17af6830ee84bd0d526a422dc6b3d383016fc3883b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af53369432b6a25196be571d33443209d8d94bdb440a378273eebc3262e3ba3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:5a12fea5a2f227cd2abb0dca3227e3aab5d8685b301a291334bfff984057ee86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56647188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33ed3691d9394a4bc76c2dbb71ea8b2b65e6e0d1cef0ed5f537f5e89f501718`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:c4e634a38404c34ac9f4b284bb68641df5c67ea6ff176f9022b06ceef2274a0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:71644fe2ef5416f8ceabf402da7c4174fe750599076e106d9e9e6a4f89f52892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392646533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ceb4a4a8fb4917a472d3255b0b9f526a6523ad4a66219e31d1aa9ad902bebc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b64e073109e8601db92af4778785b74981d0a66bb35ed640af8a8425ce28e`  
		Last Modified: Wed, 07 Sep 2022 19:21:07 GMT  
		Size: 334.8 MB (334805788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:53c32bc4a8fea84710fbfe1933b1b84db108eb76ee3c20b3b673e6bf9e331ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391452945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e68a8cd162c06fc4c4bc68291eb191aadd029d78a8e0dec6b8652231c5775f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:40:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b245692459684d75b294e1d16f2407220fe53f4ae799e5a91d34fe73061cd`  
		Last Modified: Wed, 07 Sep 2022 19:41:38 GMT  
		Size: 334.8 MB (334805757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220831.1`

```console
$ docker pull amazonlinux@sha256:d26e31b5b4bb811a12cb868453a980a9ae53338020130521b67068cec9cabcc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220831.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7301b45cf224105e4892bd17af6830ee84bd0d526a422dc6b3d383016fc3883b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af53369432b6a25196be571d33443209d8d94bdb440a378273eebc3262e3ba3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220831.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:5a12fea5a2f227cd2abb0dca3227e3aab5d8685b301a291334bfff984057ee86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56647188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33ed3691d9394a4bc76c2dbb71ea8b2b65e6e0d1cef0ed5f537f5e89f501718`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220831.1-with-sources`

```console
$ docker pull amazonlinux@sha256:c4e634a38404c34ac9f4b284bb68641df5c67ea6ff176f9022b06ceef2274a0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220831.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:71644fe2ef5416f8ceabf402da7c4174fe750599076e106d9e9e6a4f89f52892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392646533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ceb4a4a8fb4917a472d3255b0b9f526a6523ad4a66219e31d1aa9ad902bebc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b64e073109e8601db92af4778785b74981d0a66bb35ed640af8a8425ce28e`  
		Last Modified: Wed, 07 Sep 2022 19:21:07 GMT  
		Size: 334.8 MB (334805788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220831.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:53c32bc4a8fea84710fbfe1933b1b84db108eb76ee3c20b3b673e6bf9e331ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391452945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e68a8cd162c06fc4c4bc68291eb191aadd029d78a8e0dec6b8652231c5775f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:40:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b245692459684d75b294e1d16f2407220fe53f4ae799e5a91d34fe73061cd`  
		Last Modified: Wed, 07 Sep 2022 19:41:38 GMT  
		Size: 334.8 MB (334805757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:d26e31b5b4bb811a12cb868453a980a9ae53338020130521b67068cec9cabcc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7301b45cf224105e4892bd17af6830ee84bd0d526a422dc6b3d383016fc3883b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af53369432b6a25196be571d33443209d8d94bdb440a378273eebc3262e3ba3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:5a12fea5a2f227cd2abb0dca3227e3aab5d8685b301a291334bfff984057ee86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56647188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33ed3691d9394a4bc76c2dbb71ea8b2b65e6e0d1cef0ed5f537f5e89f501718`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:c4e634a38404c34ac9f4b284bb68641df5c67ea6ff176f9022b06ceef2274a0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:71644fe2ef5416f8ceabf402da7c4174fe750599076e106d9e9e6a4f89f52892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392646533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ceb4a4a8fb4917a472d3255b0b9f526a6523ad4a66219e31d1aa9ad902bebc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b64e073109e8601db92af4778785b74981d0a66bb35ed640af8a8425ce28e`  
		Last Modified: Wed, 07 Sep 2022 19:21:07 GMT  
		Size: 334.8 MB (334805788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:53c32bc4a8fea84710fbfe1933b1b84db108eb76ee3c20b3b673e6bf9e331ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391452945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e68a8cd162c06fc4c4bc68291eb191aadd029d78a8e0dec6b8652231c5775f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:40:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b245692459684d75b294e1d16f2407220fe53f4ae799e5a91d34fe73061cd`  
		Last Modified: Wed, 07 Sep 2022 19:41:38 GMT  
		Size: 334.8 MB (334805757 bytes)  
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
