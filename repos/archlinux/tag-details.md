<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220731.0.71623`](#archlinuxbase-20220731071623)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220731.0.71623`](#archlinuxbase-devel-20220731071623)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:987e9f0dc87e596282abd59b07b497f5e42af04853a71a41d851082adf1d9358
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:b7b1c48f4b7f3ba7ea210b9b51ffad46a6b2009cc960780e0402c4ae1b5f0f5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136660838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7470802a2f70e4ddb93d4d1c6a1c44910eb5fca8af6bbbf3be5e2fd79c7e65a6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:20:00 GMT
COPY dir:2652c111ee5e5b940348d5945df9b1de4b4d470f2d7d6b70eae18a6e67e19d94 in / 
# Mon, 01 Aug 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c6add17ebd6e9578ca074920c4a8fcd5d317dc306ff8ffcee4a0c303f81bdf6e`  
		Last Modified: Mon, 01 Aug 2022 21:21:47 GMT  
		Size: 136.7 MB (136653202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20911f3936b1751f40d2c7c0f4cb42a6b15a3bc4f8c202d12fe93dba528d39e0`  
		Last Modified: Mon, 01 Aug 2022 21:21:27 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220731.0.71623`

```console
$ docker pull archlinux@sha256:987e9f0dc87e596282abd59b07b497f5e42af04853a71a41d851082adf1d9358
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220731.0.71623` - linux; amd64

```console
$ docker pull archlinux@sha256:b7b1c48f4b7f3ba7ea210b9b51ffad46a6b2009cc960780e0402c4ae1b5f0f5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136660838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7470802a2f70e4ddb93d4d1c6a1c44910eb5fca8af6bbbf3be5e2fd79c7e65a6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:20:00 GMT
COPY dir:2652c111ee5e5b940348d5945df9b1de4b4d470f2d7d6b70eae18a6e67e19d94 in / 
# Mon, 01 Aug 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c6add17ebd6e9578ca074920c4a8fcd5d317dc306ff8ffcee4a0c303f81bdf6e`  
		Last Modified: Mon, 01 Aug 2022 21:21:47 GMT  
		Size: 136.7 MB (136653202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20911f3936b1751f40d2c7c0f4cb42a6b15a3bc4f8c202d12fe93dba528d39e0`  
		Last Modified: Mon, 01 Aug 2022 21:21:27 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:cc55357b6cf01d60f91a417792aa3c831459db75a7857f0dd5eed24fcd0e8f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:45b95804a26d39e706d1e87e661ad0c04fad7ec819df3b68eb09a6b74c013b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233201131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbd1af5cfa4904d181710f3e108817790e9a3550e1968e837046b6502111d6c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:21:01 GMT
COPY dir:58a775097c874727e6051dd7db3731e2f793cf5d33eac5c1a1d77eb0ae8ba115 in / 
# Mon, 01 Aug 2022 21:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:38cab039087fda714a03dcc8dbec451c5ed355ef11295a2c869545704aa47296`  
		Last Modified: Mon, 01 Aug 2022 21:22:35 GMT  
		Size: 233.2 MB (233192885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0519f846669778458a919d19c0391a93edfb1295a3bee866711e9e346be359f3`  
		Last Modified: Mon, 01 Aug 2022 21:22:00 GMT  
		Size: 8.2 KB (8246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220731.0.71623`

```console
$ docker pull archlinux@sha256:cc55357b6cf01d60f91a417792aa3c831459db75a7857f0dd5eed24fcd0e8f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220731.0.71623` - linux; amd64

```console
$ docker pull archlinux@sha256:45b95804a26d39e706d1e87e661ad0c04fad7ec819df3b68eb09a6b74c013b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233201131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbd1af5cfa4904d181710f3e108817790e9a3550e1968e837046b6502111d6c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:21:01 GMT
COPY dir:58a775097c874727e6051dd7db3731e2f793cf5d33eac5c1a1d77eb0ae8ba115 in / 
# Mon, 01 Aug 2022 21:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:38cab039087fda714a03dcc8dbec451c5ed355ef11295a2c869545704aa47296`  
		Last Modified: Mon, 01 Aug 2022 21:22:35 GMT  
		Size: 233.2 MB (233192885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0519f846669778458a919d19c0391a93edfb1295a3bee866711e9e346be359f3`  
		Last Modified: Mon, 01 Aug 2022 21:22:00 GMT  
		Size: 8.2 KB (8246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:987e9f0dc87e596282abd59b07b497f5e42af04853a71a41d851082adf1d9358
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:b7b1c48f4b7f3ba7ea210b9b51ffad46a6b2009cc960780e0402c4ae1b5f0f5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136660838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7470802a2f70e4ddb93d4d1c6a1c44910eb5fca8af6bbbf3be5e2fd79c7e65a6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:20:00 GMT
COPY dir:2652c111ee5e5b940348d5945df9b1de4b4d470f2d7d6b70eae18a6e67e19d94 in / 
# Mon, 01 Aug 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c6add17ebd6e9578ca074920c4a8fcd5d317dc306ff8ffcee4a0c303f81bdf6e`  
		Last Modified: Mon, 01 Aug 2022 21:21:47 GMT  
		Size: 136.7 MB (136653202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20911f3936b1751f40d2c7c0f4cb42a6b15a3bc4f8c202d12fe93dba528d39e0`  
		Last Modified: Mon, 01 Aug 2022 21:21:27 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
