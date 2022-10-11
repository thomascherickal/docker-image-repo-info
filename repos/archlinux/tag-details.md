<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221009.0.92802`](#archlinuxbase-20221009092802)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221009.0.92802`](#archlinuxbase-devel-20221009092802)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:df3968bf4cc3b56c870fc3687d9c217ebc7a9b47ab66a66961217317ef372622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:a5337390f41961a1c18115935cc6ac5b8dfa7714cde2704ab86a5110df4420fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b17a3e650d6b974b7166a01f45ea55cae189018ee0d57b58864a289567aa873`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Thu, 06 Oct 2022 19:54:50 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Thu, 06 Oct 2022 19:54:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Thu, 06 Oct 2022 19:54:51 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:54:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0021011b66e354f66e0fa5dbef713d683cf71ddeaaeaa718c4e1da551f9929`  
		Last Modified: Thu, 06 Oct 2022 19:56:15 GMT  
		Size: 7.9 KB (7907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221009.0.92802`

```console
$ docker pull archlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:33787b7abe685e0343c022b23bc0d54be281c60fc7d73f75b13e15085b6d7a2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:552467000569cfe052f535fe31fd66cb2bcd749f73d36255d6a777ff86b06798
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238593146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd00261ea299c70e6bfdde761a4b33e4e104a19a4f4b69cc05c42085522ea7ee`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Thu, 06 Oct 2022 19:55:51 GMT
COPY dir:18fea0b266ee182d9d39f5c46c96dce2236a702069f997545d0df7b9c4099d49 in / 
# Thu, 06 Oct 2022 19:55:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Thu, 06 Oct 2022 19:55:54 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:55:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:a64de180eba4662e4ee754ae56002a9e7471e8f9a44f207562a29b6beacd97aa`  
		Last Modified: Mon, 03 Oct 2022 21:22:29 GMT  
		Size: 238.6 MB (238584575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb010f01c1e989914c006a49bb84bf8863e524a38a93b14e9f4e3340a82eadc3`  
		Last Modified: Thu, 06 Oct 2022 19:56:26 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221009.0.92802`

```console
$ docker pull archlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:df3968bf4cc3b56c870fc3687d9c217ebc7a9b47ab66a66961217317ef372622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:a5337390f41961a1c18115935cc6ac5b8dfa7714cde2704ab86a5110df4420fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b17a3e650d6b974b7166a01f45ea55cae189018ee0d57b58864a289567aa873`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Thu, 06 Oct 2022 19:54:50 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Thu, 06 Oct 2022 19:54:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Thu, 06 Oct 2022 19:54:51 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:54:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0021011b66e354f66e0fa5dbef713d683cf71ddeaaeaa718c4e1da551f9929`  
		Last Modified: Thu, 06 Oct 2022 19:56:15 GMT  
		Size: 7.9 KB (7907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
