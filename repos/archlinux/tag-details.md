<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221002.0.91257`](#archlinuxbase-20221002091257)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221002.0.91257`](#archlinuxbase-devel-20221002091257)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:ed624bacb4f52879bb3ae96bb0c00e376ec97eba41b9460cedc4f29475e63923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:46a686dd1ea31011e5827c7e5d67fe3e8b26d572aa1ad92858fffc6c0ca86d83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139584687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff7556904e923dae045e4b119313044e8ef831d0b283c88296910258f804f91`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 26 Sep 2022 19:19:57 GMT
COPY dir:7d974c1185c730242264b42626d76e5989cb512747d6b656b29c591ce2e87286 in / 
# Mon, 26 Sep 2022 19:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 26 Sep 2022 19:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 26 Sep 2022 19:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:66acacc666da4f6a29090ffd83f8270873279605a4c09244f46715e01d456185`  
		Last Modified: Mon, 26 Sep 2022 19:21:41 GMT  
		Size: 139.6 MB (139576780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac47f4c7cddebfeebb09c5275d6bc41975775b451225ee3e73b3e77a456f22`  
		Last Modified: Mon, 26 Sep 2022 19:21:21 GMT  
		Size: 7.9 KB (7907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221002.0.91257`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:3a9e03de9c3d1e95f90e31e591c3b2b11954e24d5c149b7ac205a39704b7782e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:bf5954655c93007d344e7f1a1e196c56e3bedcc0f7825b317a3b689e47181f17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.8 MB (237804461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aaeacc9b994422ee70790a3df869997ccb119694c510ffd37db2e7c03cf9b7a`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 26 Sep 2022 19:20:57 GMT
COPY dir:0c22ac20dabf097b7354470dfb3bf3d77edab31375e144264dd086eba60af762 in / 
# Mon, 26 Sep 2022 19:21:00 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 26 Sep 2022 19:21:00 GMT
ENV LANG=C.UTF-8
# Mon, 26 Sep 2022 19:21:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5b37b91f5c5ff3e99402b7c4ccc8f6651907f8fe5e094690bcb1f643807192e8`  
		Last Modified: Mon, 26 Sep 2022 19:22:27 GMT  
		Size: 237.8 MB (237795869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf30a9abb9eaa4600eeff6f07e1d83b5e70ffd29368364e97cca06f6c8f9a2`  
		Last Modified: Mon, 26 Sep 2022 19:21:53 GMT  
		Size: 8.6 KB (8592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221002.0.91257`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:ed624bacb4f52879bb3ae96bb0c00e376ec97eba41b9460cedc4f29475e63923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:46a686dd1ea31011e5827c7e5d67fe3e8b26d572aa1ad92858fffc6c0ca86d83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139584687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff7556904e923dae045e4b119313044e8ef831d0b283c88296910258f804f91`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 26 Sep 2022 19:19:57 GMT
COPY dir:7d974c1185c730242264b42626d76e5989cb512747d6b656b29c591ce2e87286 in / 
# Mon, 26 Sep 2022 19:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 26 Sep 2022 19:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 26 Sep 2022 19:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:66acacc666da4f6a29090ffd83f8270873279605a4c09244f46715e01d456185`  
		Last Modified: Mon, 26 Sep 2022 19:21:41 GMT  
		Size: 139.6 MB (139576780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac47f4c7cddebfeebb09c5275d6bc41975775b451225ee3e73b3e77a456f22`  
		Last Modified: Mon, 26 Sep 2022 19:21:21 GMT  
		Size: 7.9 KB (7907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
