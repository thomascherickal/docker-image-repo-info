<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220828.0.78480`](#archlinuxbase-20220828078480)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220828.0.78480`](#archlinuxbase-devel-20220828078480)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:3b02b979275b2e277e0c6385764bd5392c27fb652e3c29ffb964b7b178ddbf4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:261bda260ff523f2065c71b03e2862a3943bd87b07d074f2a4e3e1373c0799b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136503707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4c97123c019536c70a732924b4870467354fc708fc581bb151175523c5fef8`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:22:21 GMT
COPY dir:f054defad7465e3fcab32f09bae7488ef08bc7b7e864ee5ad5bfbc7922969f12 in / 
# Mon, 29 Aug 2022 18:22:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:22:22 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:22:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4f7977a2487ea810b171da6f2bd310aa0df9fa13fdcdcce04b58575c932c5193`  
		Last Modified: Mon, 29 Aug 2022 18:24:18 GMT  
		Size: 136.5 MB (136495597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e3166be9bd64da5e57118f09eecdde2ea3bc966b48cd07e4fae87588766a7d`  
		Last Modified: Mon, 29 Aug 2022 18:23:59 GMT  
		Size: 8.1 KB (8110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220828.0.78480`

```console
$ docker pull archlinux@sha256:3b02b979275b2e277e0c6385764bd5392c27fb652e3c29ffb964b7b178ddbf4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220828.0.78480` - linux; amd64

```console
$ docker pull archlinux@sha256:261bda260ff523f2065c71b03e2862a3943bd87b07d074f2a4e3e1373c0799b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136503707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4c97123c019536c70a732924b4870467354fc708fc581bb151175523c5fef8`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:22:21 GMT
COPY dir:f054defad7465e3fcab32f09bae7488ef08bc7b7e864ee5ad5bfbc7922969f12 in / 
# Mon, 29 Aug 2022 18:22:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:22:22 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:22:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4f7977a2487ea810b171da6f2bd310aa0df9fa13fdcdcce04b58575c932c5193`  
		Last Modified: Mon, 29 Aug 2022 18:24:18 GMT  
		Size: 136.5 MB (136495597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e3166be9bd64da5e57118f09eecdde2ea3bc966b48cd07e4fae87588766a7d`  
		Last Modified: Mon, 29 Aug 2022 18:23:59 GMT  
		Size: 8.1 KB (8110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ecba82d77702d2e6a821187a1ca6c2920fd45d07cb8ad0f26ceacee9e1a1839d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:fcb51d97b47e7ec84f6c288d85f4f8e68ec767b9a5870c774ad950d0e419c2d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234741351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f80c77eff27fe15137ecd13d9a4f76632e9b62e1dd054176518a177d752ec9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:23:21 GMT
COPY dir:ed2fc1c49ba037e42524baf0eda8f8cd554273562d224b67632edd6be6937b3f in / 
# Mon, 29 Aug 2022 18:23:24 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:23:24 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:23:24 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ccd1bf5def59f67059c64dfda047e597a6317aa3c2af90f80f1982d00f6b3332`  
		Last Modified: Mon, 29 Aug 2022 18:25:15 GMT  
		Size: 234.7 MB (234732582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a660ba1fd0faf46937f17df91a0dce51ee00aa29282232fad4b32879d87511c8`  
		Last Modified: Mon, 29 Aug 2022 18:24:38 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220828.0.78480`

```console
$ docker pull archlinux@sha256:ecba82d77702d2e6a821187a1ca6c2920fd45d07cb8ad0f26ceacee9e1a1839d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220828.0.78480` - linux; amd64

```console
$ docker pull archlinux@sha256:fcb51d97b47e7ec84f6c288d85f4f8e68ec767b9a5870c774ad950d0e419c2d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234741351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f80c77eff27fe15137ecd13d9a4f76632e9b62e1dd054176518a177d752ec9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:23:21 GMT
COPY dir:ed2fc1c49ba037e42524baf0eda8f8cd554273562d224b67632edd6be6937b3f in / 
# Mon, 29 Aug 2022 18:23:24 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:23:24 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:23:24 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ccd1bf5def59f67059c64dfda047e597a6317aa3c2af90f80f1982d00f6b3332`  
		Last Modified: Mon, 29 Aug 2022 18:25:15 GMT  
		Size: 234.7 MB (234732582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a660ba1fd0faf46937f17df91a0dce51ee00aa29282232fad4b32879d87511c8`  
		Last Modified: Mon, 29 Aug 2022 18:24:38 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:3b02b979275b2e277e0c6385764bd5392c27fb652e3c29ffb964b7b178ddbf4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:261bda260ff523f2065c71b03e2862a3943bd87b07d074f2a4e3e1373c0799b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136503707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4c97123c019536c70a732924b4870467354fc708fc581bb151175523c5fef8`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:22:21 GMT
COPY dir:f054defad7465e3fcab32f09bae7488ef08bc7b7e864ee5ad5bfbc7922969f12 in / 
# Mon, 29 Aug 2022 18:22:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:22:22 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:22:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4f7977a2487ea810b171da6f2bd310aa0df9fa13fdcdcce04b58575c932c5193`  
		Last Modified: Mon, 29 Aug 2022 18:24:18 GMT  
		Size: 136.5 MB (136495597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e3166be9bd64da5e57118f09eecdde2ea3bc966b48cd07e4fae87588766a7d`  
		Last Modified: Mon, 29 Aug 2022 18:23:59 GMT  
		Size: 8.1 KB (8110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
