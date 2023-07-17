<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230716.0.165339`](#archlinuxbase-202307160165339)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230716.0.165339`](#archlinuxbase-devel-202307160165339)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:a816f62c10a68a77df6041efdec165e8638644e8209b21ee27d7ecfd3f83d823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:767743114f4896df1b6cc7cab640f0d003e1a539d4c4a8f68971b727ab3b670c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146717650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c5d6b8a0e68d2ee61099404fb93b5e14713f5dfccbc4f06144104b4b16edfb`
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
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.version=20230709.0.163418
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.created=2023-07-09T00:07:38+00:00
# Mon, 10 Jul 2023 19:20:17 GMT
COPY dir:fc89c665a4bd20bc0a3accd17ce07e339c6baace5f29e702919b21f9f56174a6 in / 
# Mon, 10 Jul 2023 19:20:19 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230709.0.163418' /etc/os-release
# Mon, 10 Jul 2023 19:20:19 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 19:20:19 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5bab4a299671cd53f3098ba6b58094262aed71121d2531c9e3d4d7078397416d`  
		Last Modified: Mon, 10 Jul 2023 19:22:06 GMT  
		Size: 146.7 MB (146709555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c9691c4d84ac4bc563ba9bdf4e6f517801bb3abb07d6d1ec3517543ac4f84`  
		Last Modified: Mon, 10 Jul 2023 19:21:46 GMT  
		Size: 8.1 KB (8095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230716.0.165339`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:1a8b51d165a1399dc6e27b6d5858f22aa7fa5dae0698dd0b9b5ba5a036546867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:1112a0d52c7861c12c5ecf3d469709f81c9b3cb1a5677ced148720825886ff0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263536228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c791540bd070034445f816b4af95073f6d48ef57ef090c1cc356fcb4be2a39`
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
# Mon, 10 Jul 2023 19:21:11 GMT
LABEL org.opencontainers.image.version=20230709.0.163418
# Mon, 10 Jul 2023 19:21:11 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 10 Jul 2023 19:21:11 GMT
LABEL org.opencontainers.image.created=2023-07-09T00:07:41+00:00
# Mon, 10 Jul 2023 19:21:22 GMT
COPY dir:9670216286f6e66bebe90abfae810648a87bbb30d0a82a6178f089c358649605 in / 
# Mon, 10 Jul 2023 19:21:25 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230709.0.163418' /etc/os-release
# Mon, 10 Jul 2023 19:21:25 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 19:21:25 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:18fe72e1619368972afcfeb02bb432ebc7b6497be9e5b2be77f8b08a560a8ada`  
		Last Modified: Mon, 10 Jul 2023 19:22:51 GMT  
		Size: 263.5 MB (263527394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9608a19228d2ba749485d3a79bbcb00423291dc875e007a691b6230122ac7b8`  
		Last Modified: Mon, 10 Jul 2023 19:22:16 GMT  
		Size: 8.8 KB (8834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230716.0.165339`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:a816f62c10a68a77df6041efdec165e8638644e8209b21ee27d7ecfd3f83d823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:767743114f4896df1b6cc7cab640f0d003e1a539d4c4a8f68971b727ab3b670c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146717650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c5d6b8a0e68d2ee61099404fb93b5e14713f5dfccbc4f06144104b4b16edfb`
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
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.version=20230709.0.163418
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 10 Jul 2023 19:20:11 GMT
LABEL org.opencontainers.image.created=2023-07-09T00:07:38+00:00
# Mon, 10 Jul 2023 19:20:17 GMT
COPY dir:fc89c665a4bd20bc0a3accd17ce07e339c6baace5f29e702919b21f9f56174a6 in / 
# Mon, 10 Jul 2023 19:20:19 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230709.0.163418' /etc/os-release
# Mon, 10 Jul 2023 19:20:19 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 19:20:19 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5bab4a299671cd53f3098ba6b58094262aed71121d2531c9e3d4d7078397416d`  
		Last Modified: Mon, 10 Jul 2023 19:22:06 GMT  
		Size: 146.7 MB (146709555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c9691c4d84ac4bc563ba9bdf4e6f517801bb3abb07d6d1ec3517543ac4f84`  
		Last Modified: Mon, 10 Jul 2023 19:21:46 GMT  
		Size: 8.1 KB (8095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
