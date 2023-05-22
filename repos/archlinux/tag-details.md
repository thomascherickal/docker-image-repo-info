<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230521.0.152478`](#archlinuxbase-202305210152478)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230521.0.152478`](#archlinuxbase-devel-202305210152478)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:7f9fe7f705b36b2b9c9e4d12b8cfd984bd2aaf4f89029be304bfcab78e6744b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:f081f7f60b83cfeaff651e4ca03e4d23bf6ce6a5045594ea9b983aa686acb817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145657366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da2f9fedb6608e0b68459568585b041791d8afcede52eee1deb7be0ccbdf2b9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 15 May 2023 18:20:14 GMT
COPY dir:07ae38beef41ac44181106d746e6dc9a8a3a667d9da2a7657cf41efa58c2c7e0 in / 
# Mon, 15 May 2023 18:20:15 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 15 May 2023 18:20:15 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2023 18:20:16 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:23851f282a340aee1fcb3541debfbc6453385bd908e1c1c7562bf5e95e02e9d4`  
		Last Modified: Mon, 15 May 2023 18:22:01 GMT  
		Size: 145.6 MB (145649340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23ea749df6e4027a67faebc6edd140de6e265575887909ef472fbe08679154`  
		Last Modified: Mon, 15 May 2023 18:21:42 GMT  
		Size: 8.0 KB (8026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230521.0.152478`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:fbe1c6eb72d53b6dcab5f21e2f3ff9a8e161947f677464f5f551cfb8660d51e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:c5cf194585df076f634333e340f0bb9497fff1868b9f483e60bede0c3f13c7a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252697506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ada122f6f0952bf55e7f2d83885775b9f96bd207e87958feb7acd4c5cdc806`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 15 May 2023 18:21:19 GMT
COPY dir:c02b8f09109baf4f4a31b7fb42640130ba55889dab1f86cbfb753a71f307b006 in / 
# Mon, 15 May 2023 18:21:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 15 May 2023 18:21:22 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2023 18:21:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:0c59d588f65cf0ea6aa402842acb749ed3db5cf32fbf6707f5882c20733612e4`  
		Last Modified: Mon, 15 May 2023 18:22:46 GMT  
		Size: 252.7 MB (252688786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83094b84f99886a3a59257eaf2678efcf715a556109cdc8f27835091a4f5be1f`  
		Last Modified: Mon, 15 May 2023 18:22:12 GMT  
		Size: 8.7 KB (8720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230521.0.152478`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:7f9fe7f705b36b2b9c9e4d12b8cfd984bd2aaf4f89029be304bfcab78e6744b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:f081f7f60b83cfeaff651e4ca03e4d23bf6ce6a5045594ea9b983aa686acb817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145657366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da2f9fedb6608e0b68459568585b041791d8afcede52eee1deb7be0ccbdf2b9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 15 May 2023 18:20:14 GMT
COPY dir:07ae38beef41ac44181106d746e6dc9a8a3a667d9da2a7657cf41efa58c2c7e0 in / 
# Mon, 15 May 2023 18:20:15 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 15 May 2023 18:20:15 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2023 18:20:16 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:23851f282a340aee1fcb3541debfbc6453385bd908e1c1c7562bf5e95e02e9d4`  
		Last Modified: Mon, 15 May 2023 18:22:01 GMT  
		Size: 145.6 MB (145649340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23ea749df6e4027a67faebc6edd140de6e265575887909ef472fbe08679154`  
		Last Modified: Mon, 15 May 2023 18:21:42 GMT  
		Size: 8.0 KB (8026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
