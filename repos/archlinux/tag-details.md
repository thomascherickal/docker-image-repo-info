<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230604.0.155602`](#archlinuxbase-202306040155602)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230604.0.155602`](#archlinuxbase-devel-202306040155602)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:90ac8e1075a9e2a4bd2fc657afccd05ce9626d627fdfb24a0108a4a2998319e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:5af2b0f645075a73bcb19e8c0f24b6b0d86a4305e1a84f9a53f9fd5e7bc0f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145896888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc56b88e36b9e33677b1ebf65bc238b80988c858ead662fe4b68249410fdf0c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:22:42 GMT
COPY dir:592dbcf24bea6fe3bdd66c3cfbaf8792b7e8c2db39bf0c457b13a189d768bdfe in / 
# Mon, 05 Jun 2023 19:22:43 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:22:44 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:22:44 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f917b72a30c8e0ac2d82975c49979594120b14a17a5658078e43e438aa9d477e`  
		Last Modified: Mon, 05 Jun 2023 19:24:14 GMT  
		Size: 145.9 MB (145888851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ab89f191e8f779829d7535540fd66b8778a9f9241082933fdf59d9989490a3`  
		Last Modified: Mon, 05 Jun 2023 19:23:55 GMT  
		Size: 8.0 KB (8037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230604.0.155602`

```console
$ docker pull archlinux@sha256:90ac8e1075a9e2a4bd2fc657afccd05ce9626d627fdfb24a0108a4a2998319e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230604.0.155602` - linux; amd64

```console
$ docker pull archlinux@sha256:5af2b0f645075a73bcb19e8c0f24b6b0d86a4305e1a84f9a53f9fd5e7bc0f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145896888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc56b88e36b9e33677b1ebf65bc238b80988c858ead662fe4b68249410fdf0c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:22:42 GMT
COPY dir:592dbcf24bea6fe3bdd66c3cfbaf8792b7e8c2db39bf0c457b13a189d768bdfe in / 
# Mon, 05 Jun 2023 19:22:43 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:22:44 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:22:44 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f917b72a30c8e0ac2d82975c49979594120b14a17a5658078e43e438aa9d477e`  
		Last Modified: Mon, 05 Jun 2023 19:24:14 GMT  
		Size: 145.9 MB (145888851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ab89f191e8f779829d7535540fd66b8778a9f9241082933fdf59d9989490a3`  
		Last Modified: Mon, 05 Jun 2023 19:23:55 GMT  
		Size: 8.0 KB (8037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:a5dafc2b3423f39b4cc9e189710dad87f538d6394c57d74371e342627361bef8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:77a89e28ddcd59e4f6cd74aa144be5596bc22527255c0bb2a50d5396b28e6407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252925084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ffb784ff04aa8f564e94dca2070164c5415fa13f61a5f132beb6b8296dbe9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:23:42 GMT
COPY dir:83dee47f62aedc3809cee3cb8671c2e3d18eac420969a7d5fa2edf9eed305bf2 in / 
# Mon, 05 Jun 2023 19:23:45 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:23:45 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:23:45 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eb72108021e90da9b83e1a33de6203adf1dc40b5e52134b4330d933755737b63`  
		Last Modified: Mon, 05 Jun 2023 19:24:59 GMT  
		Size: 252.9 MB (252916345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d49bf5cf371455eeb81e9a5b86eb1ca86c1f059caa812b3d68732aa4fbe4e94`  
		Last Modified: Mon, 05 Jun 2023 19:24:25 GMT  
		Size: 8.7 KB (8739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230604.0.155602`

```console
$ docker pull archlinux@sha256:a5dafc2b3423f39b4cc9e189710dad87f538d6394c57d74371e342627361bef8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230604.0.155602` - linux; amd64

```console
$ docker pull archlinux@sha256:77a89e28ddcd59e4f6cd74aa144be5596bc22527255c0bb2a50d5396b28e6407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252925084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ffb784ff04aa8f564e94dca2070164c5415fa13f61a5f132beb6b8296dbe9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:23:42 GMT
COPY dir:83dee47f62aedc3809cee3cb8671c2e3d18eac420969a7d5fa2edf9eed305bf2 in / 
# Mon, 05 Jun 2023 19:23:45 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:23:45 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:23:45 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eb72108021e90da9b83e1a33de6203adf1dc40b5e52134b4330d933755737b63`  
		Last Modified: Mon, 05 Jun 2023 19:24:59 GMT  
		Size: 252.9 MB (252916345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d49bf5cf371455eeb81e9a5b86eb1ca86c1f059caa812b3d68732aa4fbe4e94`  
		Last Modified: Mon, 05 Jun 2023 19:24:25 GMT  
		Size: 8.7 KB (8739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:90ac8e1075a9e2a4bd2fc657afccd05ce9626d627fdfb24a0108a4a2998319e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:5af2b0f645075a73bcb19e8c0f24b6b0d86a4305e1a84f9a53f9fd5e7bc0f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145896888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc56b88e36b9e33677b1ebf65bc238b80988c858ead662fe4b68249410fdf0c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:22:42 GMT
COPY dir:592dbcf24bea6fe3bdd66c3cfbaf8792b7e8c2db39bf0c457b13a189d768bdfe in / 
# Mon, 05 Jun 2023 19:22:43 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:22:44 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:22:44 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f917b72a30c8e0ac2d82975c49979594120b14a17a5658078e43e438aa9d477e`  
		Last Modified: Mon, 05 Jun 2023 19:24:14 GMT  
		Size: 145.9 MB (145888851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ab89f191e8f779829d7535540fd66b8778a9f9241082933fdf59d9989490a3`  
		Last Modified: Mon, 05 Jun 2023 19:23:55 GMT  
		Size: 8.0 KB (8037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
