<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230723.0.166908`](#archlinuxbase-202307230166908)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230723.0.166908`](#archlinuxbase-devel-202307230166908)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:fe6b55ecfcfe638aa13560cdc66eb2ad9bd6c4f6684d27d0d2a3816cf2882a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:cf219c9214e840f642076be8eac01509e83fd2ccf540d3f416cd2384c7ebc479
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146733218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83177fd64f444d3690ca73822bb6ad6ab9bb4ad0b9cd250f8b9aa799699d8897`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.title=Arch Linux base Image
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.version=20230716.0.165339
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.created=2023-07-16T00:07:26+00:00
# Mon, 17 Jul 2023 19:20:05 GMT
COPY dir:fec049f813929c8d117fc0b91fbcb51f942d7862d35c7a93f869983773bfe470 in / 
# Mon, 17 Jul 2023 19:20:07 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230716.0.165339' /etc/os-release
# Mon, 17 Jul 2023 19:20:07 GMT
ENV LANG=C.UTF-8
# Mon, 17 Jul 2023 19:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8f0e8ad11b5eaa0bc7045700a7c25289b34e613f54b06c33d70288ece0e8d8a8`  
		Last Modified: Mon, 17 Jul 2023 19:21:53 GMT  
		Size: 146.7 MB (146725130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050b7449698b12238d1c52d4c41cfe36a6cd5bbbd57a727ab4babe84c18dde04`  
		Last Modified: Mon, 17 Jul 2023 19:21:33 GMT  
		Size: 8.1 KB (8088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230723.0.166908`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:b25f2ab6534259c4aca08ee71607ece151bc43f4493c888e2843de0a4711dcc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:4cd31c30eaec0c0ab4b802c17a4404044bac0d8b30d0dbe6fa34de098f6bcc37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.6 MB (263586859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be707d13ec4e63b4280b00941db18e2ed214f9525cc06be06e46a01134a7ce0d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 18:20:54 GMT
LABEL org.opencontainers.image.title=Arch Linux base-devel Image
# Mon, 12 Jun 2023 18:20:54 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Mon, 12 Jun 2023 18:20:54 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Mon, 12 Jun 2023 18:20:55 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Mon, 12 Jun 2023 18:20:55 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Mon, 12 Jun 2023 18:20:55 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Mon, 12 Jun 2023 18:20:55 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Mon, 17 Jul 2023 19:20:55 GMT
LABEL org.opencontainers.image.version=20230716.0.165339
# Mon, 17 Jul 2023 19:20:55 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 17 Jul 2023 19:20:55 GMT
LABEL org.opencontainers.image.created=2023-07-16T00:07:29+00:00
# Mon, 17 Jul 2023 19:21:05 GMT
COPY dir:ae6f35ae120c793c999c63f25712fccc392b9366b012dc50bc8ef002db2fc69e in / 
# Mon, 17 Jul 2023 19:21:09 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230716.0.165339' /etc/os-release
# Mon, 17 Jul 2023 19:21:09 GMT
ENV LANG=C.UTF-8
# Mon, 17 Jul 2023 19:21:09 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9ff50fb8eaef2d124228b0a436d0562bde9027c2c5fe9d95f2a732b23db491fc`  
		Last Modified: Mon, 17 Jul 2023 19:22:39 GMT  
		Size: 263.6 MB (263577971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7d3d4e2e9de83ae79560448b52a14a4b97648ef9243b99b4fad58a370d22a`  
		Last Modified: Mon, 17 Jul 2023 19:22:04 GMT  
		Size: 8.9 KB (8888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230723.0.166908`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:fe6b55ecfcfe638aa13560cdc66eb2ad9bd6c4f6684d27d0d2a3816cf2882a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:cf219c9214e840f642076be8eac01509e83fd2ccf540d3f416cd2384c7ebc479
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146733218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83177fd64f444d3690ca73822bb6ad6ab9bb4ad0b9cd250f8b9aa799699d8897`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.title=Arch Linux base Image
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Mon, 12 Jun 2023 18:19:57 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.version=20230716.0.165339
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 17 Jul 2023 19:19:59 GMT
LABEL org.opencontainers.image.created=2023-07-16T00:07:26+00:00
# Mon, 17 Jul 2023 19:20:05 GMT
COPY dir:fec049f813929c8d117fc0b91fbcb51f942d7862d35c7a93f869983773bfe470 in / 
# Mon, 17 Jul 2023 19:20:07 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230716.0.165339' /etc/os-release
# Mon, 17 Jul 2023 19:20:07 GMT
ENV LANG=C.UTF-8
# Mon, 17 Jul 2023 19:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8f0e8ad11b5eaa0bc7045700a7c25289b34e613f54b06c33d70288ece0e8d8a8`  
		Last Modified: Mon, 17 Jul 2023 19:21:53 GMT  
		Size: 146.7 MB (146725130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050b7449698b12238d1c52d4c41cfe36a6cd5bbbd57a727ab4babe84c18dde04`  
		Last Modified: Mon, 17 Jul 2023 19:21:33 GMT  
		Size: 8.1 KB (8088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
