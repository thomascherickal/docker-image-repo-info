<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230430.0.146624`](#archlinuxbase-202304300146624)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230430.0.146624`](#archlinuxbase-devel-202304300146624)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:e957ad743c49cb95e55d226c946da7416ff3e7cac70d0131db4bf6110cdd8de0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:7c0c89e6ecb7d815ac03bd3318f8974e8f30b9be321dbaf598e6f6aed8abd245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143110418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939c59cb5ba49b0e5c5373db225b93e163011df28d310e2e15b5e8c2a067bacb`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 02 May 2023 20:26:38 GMT
COPY dir:c712bb6caabd17bc68f6adc4def9d4e0b326e37c2c8996cb736350ec91886595 in / 
# Tue, 02 May 2023 20:26:39 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 02 May 2023 20:26:39 GMT
ENV LANG=C.UTF-8
# Tue, 02 May 2023 20:26:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:05a9396612f13404c7a585cceb964540ec70047e1a3e22b49e3f67f575d162f8`  
		Last Modified: Tue, 02 May 2023 20:28:09 GMT  
		Size: 143.1 MB (143102470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd78d2d560350a0a03264bdd6876d985c59e54b717d036e1a1b2883d8021dab`  
		Last Modified: Tue, 02 May 2023 20:27:50 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230430.0.146624`

```console
$ docker pull archlinux@sha256:e957ad743c49cb95e55d226c946da7416ff3e7cac70d0131db4bf6110cdd8de0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230430.0.146624` - linux; amd64

```console
$ docker pull archlinux@sha256:7c0c89e6ecb7d815ac03bd3318f8974e8f30b9be321dbaf598e6f6aed8abd245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143110418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939c59cb5ba49b0e5c5373db225b93e163011df28d310e2e15b5e8c2a067bacb`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 02 May 2023 20:26:38 GMT
COPY dir:c712bb6caabd17bc68f6adc4def9d4e0b326e37c2c8996cb736350ec91886595 in / 
# Tue, 02 May 2023 20:26:39 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 02 May 2023 20:26:39 GMT
ENV LANG=C.UTF-8
# Tue, 02 May 2023 20:26:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:05a9396612f13404c7a585cceb964540ec70047e1a3e22b49e3f67f575d162f8`  
		Last Modified: Tue, 02 May 2023 20:28:09 GMT  
		Size: 143.1 MB (143102470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd78d2d560350a0a03264bdd6876d985c59e54b717d036e1a1b2883d8021dab`  
		Last Modified: Tue, 02 May 2023 20:27:50 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:e8fdfe665a3e6afae775a83db1a518a0fd4f2cc0fd947aefc6a7479cbde65bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:e662e16b92ce76ad94b01839253b8eb1aa49d2b4994e5352e0c36d7575ca835b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246174656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b7fdbb34962da48968115baa78b31abe205960b6d42acfab27aa5520699cf5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 02 May 2023 20:27:37 GMT
COPY dir:b98671ca80deb4c78c7794caa639f794a6484eabd17c6b07ff3a88678a098994 in / 
# Tue, 02 May 2023 20:27:40 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 02 May 2023 20:27:40 GMT
ENV LANG=C.UTF-8
# Tue, 02 May 2023 20:27:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:848c2c12a62ecdf36b4ed9ad3b19be66f126deb08b858bec6dcab99d1f188344`  
		Last Modified: Tue, 02 May 2023 20:28:52 GMT  
		Size: 246.2 MB (246165956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeead46d365c2bdbaf2757901f27b68aa8ed9a676197c847359c3814608ed87f`  
		Last Modified: Tue, 02 May 2023 20:28:19 GMT  
		Size: 8.7 KB (8700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230430.0.146624`

```console
$ docker pull archlinux@sha256:e8fdfe665a3e6afae775a83db1a518a0fd4f2cc0fd947aefc6a7479cbde65bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230430.0.146624` - linux; amd64

```console
$ docker pull archlinux@sha256:e662e16b92ce76ad94b01839253b8eb1aa49d2b4994e5352e0c36d7575ca835b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246174656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b7fdbb34962da48968115baa78b31abe205960b6d42acfab27aa5520699cf5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 02 May 2023 20:27:37 GMT
COPY dir:b98671ca80deb4c78c7794caa639f794a6484eabd17c6b07ff3a88678a098994 in / 
# Tue, 02 May 2023 20:27:40 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 02 May 2023 20:27:40 GMT
ENV LANG=C.UTF-8
# Tue, 02 May 2023 20:27:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:848c2c12a62ecdf36b4ed9ad3b19be66f126deb08b858bec6dcab99d1f188344`  
		Last Modified: Tue, 02 May 2023 20:28:52 GMT  
		Size: 246.2 MB (246165956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeead46d365c2bdbaf2757901f27b68aa8ed9a676197c847359c3814608ed87f`  
		Last Modified: Tue, 02 May 2023 20:28:19 GMT  
		Size: 8.7 KB (8700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:e957ad743c49cb95e55d226c946da7416ff3e7cac70d0131db4bf6110cdd8de0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:7c0c89e6ecb7d815ac03bd3318f8974e8f30b9be321dbaf598e6f6aed8abd245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143110418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939c59cb5ba49b0e5c5373db225b93e163011df28d310e2e15b5e8c2a067bacb`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 02 May 2023 20:26:38 GMT
COPY dir:c712bb6caabd17bc68f6adc4def9d4e0b326e37c2c8996cb736350ec91886595 in / 
# Tue, 02 May 2023 20:26:39 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 02 May 2023 20:26:39 GMT
ENV LANG=C.UTF-8
# Tue, 02 May 2023 20:26:40 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:05a9396612f13404c7a585cceb964540ec70047e1a3e22b49e3f67f575d162f8`  
		Last Modified: Tue, 02 May 2023 20:28:09 GMT  
		Size: 143.1 MB (143102470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd78d2d560350a0a03264bdd6876d985c59e54b717d036e1a1b2883d8021dab`  
		Last Modified: Tue, 02 May 2023 20:27:50 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
