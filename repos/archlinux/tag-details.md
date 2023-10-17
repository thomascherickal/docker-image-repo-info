<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20231015.0.185077`](#archlinuxbase-202310150185077)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20231015.0.185077`](#archlinuxbase-devel-202310150185077)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:99807b5ce1017b5072f5c028d0209e97e3ab0341368880c05f3e4438ed1be5f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:9fd8ecd55ffde0f0b3f9802a2ab7b20fadeae7ed3b6882c77dc180d78ee2f50c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (146952420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2453f16847591dc207580fbab7ae626626f9d3ab347f7efd66eb2ee25c8969b7`
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
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.version=20231001.0.182270
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.revision=e688cede58b6771ce1117271551c1f0c57113614
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.created=2023-10-01T00:06:45+00:00
# Tue, 03 Oct 2023 01:14:12 GMT
COPY dir:47eb5c099872cf9f85ab952aa5de3ecf0c5cede8c0eddc06b0c460b68bf7ff17 in / 
# Tue, 03 Oct 2023 01:14:14 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231001.0.182270' /etc/os-release
# Tue, 03 Oct 2023 01:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 01:14:14 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:3d369cd697ab33fc51e0cba697fd0b4ed2e9c8913c6fca98e87c80ff330de30d`  
		Last Modified: Tue, 03 Oct 2023 01:15:55 GMT  
		Size: 146.9 MB (146944276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f5aeab7b5277ea14d595921d8a83fcdf291fb361090fdb5999a606f3aa0b1`  
		Last Modified: Tue, 03 Oct 2023 01:15:36 GMT  
		Size: 8.1 KB (8144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20231015.0.185077`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:fa74cfcb8aabe2cb876a1a60820cd034f5a414b13007af1baacada18bb4c3812
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:fa057a84079f77e3c6b1ad5dbfbf746e142a17ab41628efc4de96e20068c5678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (265017541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1202c4d3d894a9fef928c732658e4edff7c4f7c9d85166264b13ff2fbcf8f515`
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
# Tue, 03 Oct 2023 01:15:03 GMT
LABEL org.opencontainers.image.version=20231001.0.182270
# Tue, 03 Oct 2023 01:15:04 GMT
LABEL org.opencontainers.image.revision=e688cede58b6771ce1117271551c1f0c57113614
# Tue, 03 Oct 2023 01:15:04 GMT
LABEL org.opencontainers.image.created=2023-10-01T00:06:48+00:00
# Tue, 03 Oct 2023 01:15:15 GMT
COPY dir:df7a84e075b266176c1b425cffe2c107d700d5324f557b2192206d3496188524 in / 
# Tue, 03 Oct 2023 01:15:18 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231001.0.182270' /etc/os-release
# Tue, 03 Oct 2023 01:15:18 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 01:15:18 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4ad7f20d327af7b5423d91e6ad5705aeee891dd6dfbd41738cf3a60e59266462`  
		Last Modified: Tue, 03 Oct 2023 01:16:43 GMT  
		Size: 265.0 MB (265008607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59193466dab11fed768f5b6ac93b36771ff10b49c8c2cd6c34b81c88bff18e9e`  
		Last Modified: Tue, 03 Oct 2023 01:16:07 GMT  
		Size: 8.9 KB (8934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20231015.0.185077`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:99807b5ce1017b5072f5c028d0209e97e3ab0341368880c05f3e4438ed1be5f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:9fd8ecd55ffde0f0b3f9802a2ab7b20fadeae7ed3b6882c77dc180d78ee2f50c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (146952420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2453f16847591dc207580fbab7ae626626f9d3ab347f7efd66eb2ee25c8969b7`
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
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.version=20231001.0.182270
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.revision=e688cede58b6771ce1117271551c1f0c57113614
# Tue, 03 Oct 2023 01:14:05 GMT
LABEL org.opencontainers.image.created=2023-10-01T00:06:45+00:00
# Tue, 03 Oct 2023 01:14:12 GMT
COPY dir:47eb5c099872cf9f85ab952aa5de3ecf0c5cede8c0eddc06b0c460b68bf7ff17 in / 
# Tue, 03 Oct 2023 01:14:14 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231001.0.182270' /etc/os-release
# Tue, 03 Oct 2023 01:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 01:14:14 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:3d369cd697ab33fc51e0cba697fd0b4ed2e9c8913c6fca98e87c80ff330de30d`  
		Last Modified: Tue, 03 Oct 2023 01:15:55 GMT  
		Size: 146.9 MB (146944276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f5aeab7b5277ea14d595921d8a83fcdf291fb361090fdb5999a606f3aa0b1`  
		Last Modified: Tue, 03 Oct 2023 01:15:36 GMT  
		Size: 8.1 KB (8144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
