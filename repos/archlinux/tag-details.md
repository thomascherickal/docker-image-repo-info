<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230528.0.154326`](#archlinuxbase-202305280154326)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230528.0.154326`](#archlinuxbase-devel-202305280154326)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:275fb964508b7a2812f43a4dfa2cfa27cb06a4a453d72675270e2222b43f2a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:076c0233d1996165721320957be9a037a760574d6334281354b07b3b3c9440b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145779572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4866169dc4e4f2e7b4df90fe25da927da7f3449631308ce7dcee386efb1aba`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 22 May 2023 19:19:49 GMT
COPY dir:2a2cee4496b10b29beccf62c1cbddb51c8d75fcda0dde03222162678028be8ee in / 
# Mon, 22 May 2023 19:19:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 22 May 2023 19:19:51 GMT
ENV LANG=C.UTF-8
# Mon, 22 May 2023 19:19:51 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:352736306209cb0acfcf56d39f9711d6086388ce7720593490fa00a241130f2d`  
		Last Modified: Mon, 22 May 2023 19:21:31 GMT  
		Size: 145.8 MB (145771544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e04a7b46863cc79a97a92473912a8e039644f962e50fb8a581c5a06b7bf3ff`  
		Last Modified: Mon, 22 May 2023 19:21:12 GMT  
		Size: 8.0 KB (8028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230528.0.154326`

```console
$ docker pull archlinux@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:3ff3ea426aae58c222197972999bfec55871937af57b8d5a083d94906fe8afaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:34e5eff85e35956f4832344161c7e28d3d65a564573623d064d0af8591ed7367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252800803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed89e4f5fecb96251e46a0e28625fdd4df3e1724242b1027690e9c66d802efc`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 22 May 2023 19:20:50 GMT
COPY dir:d02c9573519a7585fb8e77c3d63575e1e947893a113d9ecafc9356fdd2a9518a in / 
# Mon, 22 May 2023 19:20:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 22 May 2023 19:20:54 GMT
ENV LANG=C.UTF-8
# Mon, 22 May 2023 19:20:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:cd4fcb5c4c907b09a037c9f567f24093ebce70585c8cc84b64b16f70a12b8c32`  
		Last Modified: Mon, 22 May 2023 19:22:15 GMT  
		Size: 252.8 MB (252792096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224c0c490b5f8acb56d7c9ea7f259214e77af8d3edd6c4fb1e1db8fe0a35808b`  
		Last Modified: Mon, 22 May 2023 19:21:42 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230528.0.154326`

```console
$ docker pull archlinux@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:275fb964508b7a2812f43a4dfa2cfa27cb06a4a453d72675270e2222b43f2a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:076c0233d1996165721320957be9a037a760574d6334281354b07b3b3c9440b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145779572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4866169dc4e4f2e7b4df90fe25da927da7f3449631308ce7dcee386efb1aba`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 22 May 2023 19:19:49 GMT
COPY dir:2a2cee4496b10b29beccf62c1cbddb51c8d75fcda0dde03222162678028be8ee in / 
# Mon, 22 May 2023 19:19:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 22 May 2023 19:19:51 GMT
ENV LANG=C.UTF-8
# Mon, 22 May 2023 19:19:51 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:352736306209cb0acfcf56d39f9711d6086388ce7720593490fa00a241130f2d`  
		Last Modified: Mon, 22 May 2023 19:21:31 GMT  
		Size: 145.8 MB (145771544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e04a7b46863cc79a97a92473912a8e039644f962e50fb8a581c5a06b7bf3ff`  
		Last Modified: Mon, 22 May 2023 19:21:12 GMT  
		Size: 8.0 KB (8028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
