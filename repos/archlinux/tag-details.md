<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230219.0.127702`](#archlinuxbase-202302190127702)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230219.0.127702`](#archlinuxbase-devel-202302190127702)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:27f132b602ba42dd597637d716b59f1cc2b31cf3af69325201a2168a288501d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:b0e145cbe10ce4c7ad6a1373b8fcc1ce97b02f8fb9d5450b6796617d01b6e18c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (141993959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067b0bfd114e531542878e636b1bbbd3eec28621bc6737be90a287f4a22849f6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Feb 2023 20:20:38 GMT
COPY dir:f5b23aef4d1612d34ba6b7dc4110aa200b24a6c91c560e209e4ea099f514c2c6 in / 
# Mon, 13 Feb 2023 20:20:40 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Feb 2023 20:20:40 GMT
ENV LANG=C.UTF-8
# Mon, 13 Feb 2023 20:20:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:31236c5f9bf47a34b3d104d8a890cc7fff5bf3cd7e287f2341e6e395482d85da`  
		Last Modified: Mon, 13 Feb 2023 20:22:23 GMT  
		Size: 142.0 MB (141985993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7551fe27d5768b830b411e614a23f491afb0249369c4163f5211df3133e971aa`  
		Last Modified: Mon, 13 Feb 2023 20:22:03 GMT  
		Size: 8.0 KB (7966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230219.0.127702`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:9dd936a5a5358fa2e3515e1daabe4c0e6b4c1e9fcf369528d229955590c93472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:281b8d7a7fb081e97ff77ce51a20fdce6b9e3d4e0dd0eb64f9709e37a5ebacad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.1 MB (245053097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96e8d772c84de9eb63dc7e8a6abb7bb9e667ddd46463a7a0ea661c4cf9ef392`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Feb 2023 20:21:39 GMT
COPY dir:0c01d60dfc09a8bffe3ec055f8f68dcbf61b0711f9cd6afe8d79daf5f83dc738 in / 
# Mon, 13 Feb 2023 20:21:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Feb 2023 20:21:42 GMT
ENV LANG=C.UTF-8
# Mon, 13 Feb 2023 20:21:42 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:04dc004165810067cd038f8b6066e0efd55154b29e57d6154b28a0889a4a5b23`  
		Last Modified: Mon, 13 Feb 2023 20:23:10 GMT  
		Size: 245.0 MB (245044377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353a4755ef87c4a30a4aa03216a34e16e9cb8cafdee1bd9206ab31e7f0c72fa`  
		Last Modified: Mon, 13 Feb 2023 20:22:34 GMT  
		Size: 8.7 KB (8720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230219.0.127702`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:27f132b602ba42dd597637d716b59f1cc2b31cf3af69325201a2168a288501d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:b0e145cbe10ce4c7ad6a1373b8fcc1ce97b02f8fb9d5450b6796617d01b6e18c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (141993959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067b0bfd114e531542878e636b1bbbd3eec28621bc6737be90a287f4a22849f6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Feb 2023 20:20:38 GMT
COPY dir:f5b23aef4d1612d34ba6b7dc4110aa200b24a6c91c560e209e4ea099f514c2c6 in / 
# Mon, 13 Feb 2023 20:20:40 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Feb 2023 20:20:40 GMT
ENV LANG=C.UTF-8
# Mon, 13 Feb 2023 20:20:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:31236c5f9bf47a34b3d104d8a890cc7fff5bf3cd7e287f2341e6e395482d85da`  
		Last Modified: Mon, 13 Feb 2023 20:22:23 GMT  
		Size: 142.0 MB (141985993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7551fe27d5768b830b411e614a23f491afb0249369c4163f5211df3133e971aa`  
		Last Modified: Mon, 13 Feb 2023 20:22:03 GMT  
		Size: 8.0 KB (7966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
