<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221023.0.96685`](#archlinuxbase-20221023096685)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221023.0.96685`](#archlinuxbase-devel-20221023096685)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:71df376dbf28d6eaecbe9de04e394566afeba74e8cac2b2fdf36e05c5ae0b1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:bc4ed3be8c243364fcd35efa1c0453a60656273a503db678bfb539636e9faa64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140617937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07c50d60718b29af087862ef10d0652f308738ba62d3ff0c76fa904c1a75c0e`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:20:00 GMT
COPY dir:4752ae61421385c24c18856c8a2557961ebd3b1a21b1a47b5c4e9b945445c0c9 in / 
# Mon, 24 Oct 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eebb07dfd16c7bf2df5098fe297270d6244a762136b62f00439a1f93b8efd904`  
		Last Modified: Mon, 24 Oct 2022 21:21:46 GMT  
		Size: 140.6 MB (140609989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ee4e22db4ca78665baa96d081d15e1e49bd99bb86a15bd8314535db437b1a`  
		Last Modified: Mon, 24 Oct 2022 21:21:25 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221023.0.96685`

```console
$ docker pull archlinux@sha256:71df376dbf28d6eaecbe9de04e394566afeba74e8cac2b2fdf36e05c5ae0b1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20221023.0.96685` - linux; amd64

```console
$ docker pull archlinux@sha256:bc4ed3be8c243364fcd35efa1c0453a60656273a503db678bfb539636e9faa64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140617937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07c50d60718b29af087862ef10d0652f308738ba62d3ff0c76fa904c1a75c0e`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:20:00 GMT
COPY dir:4752ae61421385c24c18856c8a2557961ebd3b1a21b1a47b5c4e9b945445c0c9 in / 
# Mon, 24 Oct 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eebb07dfd16c7bf2df5098fe297270d6244a762136b62f00439a1f93b8efd904`  
		Last Modified: Mon, 24 Oct 2022 21:21:46 GMT  
		Size: 140.6 MB (140609989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ee4e22db4ca78665baa96d081d15e1e49bd99bb86a15bd8314535db437b1a`  
		Last Modified: Mon, 24 Oct 2022 21:21:25 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:421bd2af7f4853edf180cef0b74d8cadfca72c8c92e29bde90fec931a004d91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:781cbf95c9a6e1331fad7530698c553332f2214d8a90dfc57e917f8f2eeb48ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238885643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827bc94cc055669ac67a8a8fff40dd7cb074580ce84c4daeb7d8666eef4b970b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:21:00 GMT
COPY dir:e2e64ce0c17310fffcad9a034e58b60141f53df9860774b1c80ff4a6af87acae in / 
# Mon, 24 Oct 2022 21:21:03 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9f40941c11469badff128bb105b32a1a5d8e1708e24c266c3ccfae5f1159038f`  
		Last Modified: Mon, 24 Oct 2022 21:22:33 GMT  
		Size: 238.9 MB (238877020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a92820c5bfe8a40e9f3afb6868e83657adcefffcf51198c605e5d4372ad18`  
		Last Modified: Mon, 24 Oct 2022 21:21:58 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221023.0.96685`

```console
$ docker pull archlinux@sha256:421bd2af7f4853edf180cef0b74d8cadfca72c8c92e29bde90fec931a004d91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221023.0.96685` - linux; amd64

```console
$ docker pull archlinux@sha256:781cbf95c9a6e1331fad7530698c553332f2214d8a90dfc57e917f8f2eeb48ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238885643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827bc94cc055669ac67a8a8fff40dd7cb074580ce84c4daeb7d8666eef4b970b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:21:00 GMT
COPY dir:e2e64ce0c17310fffcad9a034e58b60141f53df9860774b1c80ff4a6af87acae in / 
# Mon, 24 Oct 2022 21:21:03 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9f40941c11469badff128bb105b32a1a5d8e1708e24c266c3ccfae5f1159038f`  
		Last Modified: Mon, 24 Oct 2022 21:22:33 GMT  
		Size: 238.9 MB (238877020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a92820c5bfe8a40e9f3afb6868e83657adcefffcf51198c605e5d4372ad18`  
		Last Modified: Mon, 24 Oct 2022 21:21:58 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:71df376dbf28d6eaecbe9de04e394566afeba74e8cac2b2fdf36e05c5ae0b1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:bc4ed3be8c243364fcd35efa1c0453a60656273a503db678bfb539636e9faa64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140617937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07c50d60718b29af087862ef10d0652f308738ba62d3ff0c76fa904c1a75c0e`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:20:00 GMT
COPY dir:4752ae61421385c24c18856c8a2557961ebd3b1a21b1a47b5c4e9b945445c0c9 in / 
# Mon, 24 Oct 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eebb07dfd16c7bf2df5098fe297270d6244a762136b62f00439a1f93b8efd904`  
		Last Modified: Mon, 24 Oct 2022 21:21:46 GMT  
		Size: 140.6 MB (140609989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ee4e22db4ca78665baa96d081d15e1e49bd99bb86a15bd8314535db437b1a`  
		Last Modified: Mon, 24 Oct 2022 21:21:25 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
