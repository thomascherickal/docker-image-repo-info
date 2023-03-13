<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230312.0.133040`](#archlinuxbase-202303120133040)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230312.0.133040`](#archlinuxbase-devel-202303120133040)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:979eb993b12e665fcf0c7e454c406ed68e596f3669844f66a56ca859225e7058
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:4a1f1f983df03a1cee7bc7813f79889cd4386c71f8590397d283f925c0a7422d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142242227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff75e574221db7a20bc04e1d20d5d5151b20b30f5ad85f97758859613f92a3b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:20:05 GMT
COPY dir:afee26977378a8da2f08119e932279bd8af167ac19027b4b157f1d10cf254fab in / 
# Mon, 13 Mar 2023 20:20:06 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:20:06 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:d24ecaff127acda26655a6338c1604a6b28e6fd6e8fc8fd33b75437fe51f078e`  
		Last Modified: Mon, 13 Mar 2023 20:21:41 GMT  
		Size: 142.2 MB (142234280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024146e6ccb67f2e2267f1ecc87275ff2283583ac0feab1395bd6fd0abd5c026`  
		Last Modified: Mon, 13 Mar 2023 20:21:22 GMT  
		Size: 7.9 KB (7947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230312.0.133040`

```console
$ docker pull archlinux@sha256:979eb993b12e665fcf0c7e454c406ed68e596f3669844f66a56ca859225e7058
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230312.0.133040` - linux; amd64

```console
$ docker pull archlinux@sha256:4a1f1f983df03a1cee7bc7813f79889cd4386c71f8590397d283f925c0a7422d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142242227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff75e574221db7a20bc04e1d20d5d5151b20b30f5ad85f97758859613f92a3b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:20:05 GMT
COPY dir:afee26977378a8da2f08119e932279bd8af167ac19027b4b157f1d10cf254fab in / 
# Mon, 13 Mar 2023 20:20:06 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:20:06 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:d24ecaff127acda26655a6338c1604a6b28e6fd6e8fc8fd33b75437fe51f078e`  
		Last Modified: Mon, 13 Mar 2023 20:21:41 GMT  
		Size: 142.2 MB (142234280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024146e6ccb67f2e2267f1ecc87275ff2283583ac0feab1395bd6fd0abd5c026`  
		Last Modified: Mon, 13 Mar 2023 20:21:22 GMT  
		Size: 7.9 KB (7947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:a1a2a043d8da23e7b5dc4ed317eb347fdba2bbfb1ef16a0f4a3b11af079fe4fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:22c7ac88ee00e5be95c044b4dae7776e02d695399556ed7c3496384a49c6d8d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245231648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c348c74f0463466776cfe512ee909b9f9ab937eb3a0fbd9954379db7ba06f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:21:07 GMT
COPY dir:6cd30a0c7a3ffa597ef65b4f3d914b13d51c8e2a70299f0eec09c6804be58e74 in / 
# Mon, 13 Mar 2023 20:21:10 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:21:11 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:21:11 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1c7df861908c5cdc63525ce742a3331ef82e3d297ab2950091737a8bdd823c1a`  
		Last Modified: Mon, 13 Mar 2023 20:22:25 GMT  
		Size: 245.2 MB (245222932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae8051f50ebcbcea2f4dd988a67851d02e9ddbe134e3539dbe69ef14416256`  
		Last Modified: Mon, 13 Mar 2023 20:21:52 GMT  
		Size: 8.7 KB (8716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230312.0.133040`

```console
$ docker pull archlinux@sha256:a1a2a043d8da23e7b5dc4ed317eb347fdba2bbfb1ef16a0f4a3b11af079fe4fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230312.0.133040` - linux; amd64

```console
$ docker pull archlinux@sha256:22c7ac88ee00e5be95c044b4dae7776e02d695399556ed7c3496384a49c6d8d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245231648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c348c74f0463466776cfe512ee909b9f9ab937eb3a0fbd9954379db7ba06f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:21:07 GMT
COPY dir:6cd30a0c7a3ffa597ef65b4f3d914b13d51c8e2a70299f0eec09c6804be58e74 in / 
# Mon, 13 Mar 2023 20:21:10 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:21:11 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:21:11 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1c7df861908c5cdc63525ce742a3331ef82e3d297ab2950091737a8bdd823c1a`  
		Last Modified: Mon, 13 Mar 2023 20:22:25 GMT  
		Size: 245.2 MB (245222932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae8051f50ebcbcea2f4dd988a67851d02e9ddbe134e3539dbe69ef14416256`  
		Last Modified: Mon, 13 Mar 2023 20:21:52 GMT  
		Size: 8.7 KB (8716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:979eb993b12e665fcf0c7e454c406ed68e596f3669844f66a56ca859225e7058
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:4a1f1f983df03a1cee7bc7813f79889cd4386c71f8590397d283f925c0a7422d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142242227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff75e574221db7a20bc04e1d20d5d5151b20b30f5ad85f97758859613f92a3b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:20:05 GMT
COPY dir:afee26977378a8da2f08119e932279bd8af167ac19027b4b157f1d10cf254fab in / 
# Mon, 13 Mar 2023 20:20:06 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:20:06 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:d24ecaff127acda26655a6338c1604a6b28e6fd6e8fc8fd33b75437fe51f078e`  
		Last Modified: Mon, 13 Mar 2023 20:21:41 GMT  
		Size: 142.2 MB (142234280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024146e6ccb67f2e2267f1ecc87275ff2283583ac0feab1395bd6fd0abd5c026`  
		Last Modified: Mon, 13 Mar 2023 20:21:22 GMT  
		Size: 7.9 KB (7947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
