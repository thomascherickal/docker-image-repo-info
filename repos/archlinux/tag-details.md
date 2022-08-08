<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220807.0.72894`](#archlinuxbase-20220807072894)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220807.0.72894`](#archlinuxbase-devel-20220807072894)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:bc94045c514c3ef084f9f184709f176343ae3d716af35f1b905945cd37d8a8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:2be884e04ef462104d7d39a8df45f6bc6440154f7e73a7f58dc64b4384a63bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136491314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59532bb094c08b2b5d328913a438de426ed1afe0307f5d8bce2ecacbbe328d0f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 08 Aug 2022 19:19:58 GMT
COPY dir:b7306b39bc57f56723a14dceeba21088d69594a0e4dc5ff4ace2313a168b5b01 in / 
# Mon, 08 Aug 2022 19:20:00 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 08 Aug 2022 19:20:00 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 19:20:00 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:e3a0690c6df16bafd78749f5f49cc915cd897ca5acfbc9b1e95788eab51bae2e`  
		Last Modified: Mon, 08 Aug 2022 19:21:43 GMT  
		Size: 136.5 MB (136483224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94422751e6b6ebb9ee0f94689bbc84d80f09dedbfd7984b01c6481b1386af34`  
		Last Modified: Mon, 08 Aug 2022 19:21:22 GMT  
		Size: 8.1 KB (8090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220807.0.72894`

```console
$ docker pull archlinux@sha256:bc94045c514c3ef084f9f184709f176343ae3d716af35f1b905945cd37d8a8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220807.0.72894` - linux; amd64

```console
$ docker pull archlinux@sha256:2be884e04ef462104d7d39a8df45f6bc6440154f7e73a7f58dc64b4384a63bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136491314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59532bb094c08b2b5d328913a438de426ed1afe0307f5d8bce2ecacbbe328d0f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 08 Aug 2022 19:19:58 GMT
COPY dir:b7306b39bc57f56723a14dceeba21088d69594a0e4dc5ff4ace2313a168b5b01 in / 
# Mon, 08 Aug 2022 19:20:00 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 08 Aug 2022 19:20:00 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 19:20:00 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:e3a0690c6df16bafd78749f5f49cc915cd897ca5acfbc9b1e95788eab51bae2e`  
		Last Modified: Mon, 08 Aug 2022 19:21:43 GMT  
		Size: 136.5 MB (136483224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94422751e6b6ebb9ee0f94689bbc84d80f09dedbfd7984b01c6481b1386af34`  
		Last Modified: Mon, 08 Aug 2022 19:21:22 GMT  
		Size: 8.1 KB (8090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:455d986f191b0cbc94ec18c239ffea28c3948551ae913af7833888147d7b4698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:2780002c464ca8c385991964dc0743b6c870bcc0795d238dfe9449ca2641333e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.1 MB (233063441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4726a34f4ee0f6df8b17eb1e23693c4c2523dcc993c7fe5e16eb9fd4584207`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 08 Aug 2022 19:20:59 GMT
COPY dir:ca26dff4bae4ee29b673c82644b4d5989359724e02def94779605099697ebfa3 in / 
# Mon, 08 Aug 2022 19:21:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 08 Aug 2022 19:21:02 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 19:21:03 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:3a2c417f7370328ec484b88675c78e1ac21f4db6d41eea8df64ad327c349cb6f`  
		Last Modified: Mon, 08 Aug 2022 19:22:31 GMT  
		Size: 233.1 MB (233054727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1727f232bf90241e441670fc7268e801ce01c038ac5e98940e72a29b4a08cdf`  
		Last Modified: Mon, 08 Aug 2022 19:21:56 GMT  
		Size: 8.7 KB (8714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220807.0.72894`

```console
$ docker pull archlinux@sha256:455d986f191b0cbc94ec18c239ffea28c3948551ae913af7833888147d7b4698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220807.0.72894` - linux; amd64

```console
$ docker pull archlinux@sha256:2780002c464ca8c385991964dc0743b6c870bcc0795d238dfe9449ca2641333e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.1 MB (233063441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4726a34f4ee0f6df8b17eb1e23693c4c2523dcc993c7fe5e16eb9fd4584207`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 08 Aug 2022 19:20:59 GMT
COPY dir:ca26dff4bae4ee29b673c82644b4d5989359724e02def94779605099697ebfa3 in / 
# Mon, 08 Aug 2022 19:21:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 08 Aug 2022 19:21:02 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 19:21:03 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:3a2c417f7370328ec484b88675c78e1ac21f4db6d41eea8df64ad327c349cb6f`  
		Last Modified: Mon, 08 Aug 2022 19:22:31 GMT  
		Size: 233.1 MB (233054727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1727f232bf90241e441670fc7268e801ce01c038ac5e98940e72a29b4a08cdf`  
		Last Modified: Mon, 08 Aug 2022 19:21:56 GMT  
		Size: 8.7 KB (8714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:bc94045c514c3ef084f9f184709f176343ae3d716af35f1b905945cd37d8a8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:2be884e04ef462104d7d39a8df45f6bc6440154f7e73a7f58dc64b4384a63bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136491314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59532bb094c08b2b5d328913a438de426ed1afe0307f5d8bce2ecacbbe328d0f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 08 Aug 2022 19:19:58 GMT
COPY dir:b7306b39bc57f56723a14dceeba21088d69594a0e4dc5ff4ace2313a168b5b01 in / 
# Mon, 08 Aug 2022 19:20:00 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 08 Aug 2022 19:20:00 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 19:20:00 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:e3a0690c6df16bafd78749f5f49cc915cd897ca5acfbc9b1e95788eab51bae2e`  
		Last Modified: Mon, 08 Aug 2022 19:21:43 GMT  
		Size: 136.5 MB (136483224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94422751e6b6ebb9ee0f94689bbc84d80f09dedbfd7984b01c6481b1386af34`  
		Last Modified: Mon, 08 Aug 2022 19:21:22 GMT  
		Size: 8.1 KB (8090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
