<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20231112.0.191179`](#archlinuxbase-202311120191179)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20231112.0.191179`](#archlinuxbase-devel-202311120191179)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:1f83ba0580a15cd6ad1d02d62ad432ddc940f53f07d0e39c8982d6c9c74e53e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:6d4096442644ee6d7f71f3b60ff79d605098f7bdb4467f41d0608894e25a7ee8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147069744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e73f0f3a7ab45c7f43cd2b53dc7d86376505a8ae116a58b33abac4a257e093d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.title=Arch Linux base Image
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Tue, 14 Nov 2023 00:29:34 GMT
LABEL org.opencontainers.image.version=20231112.0.191179
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.revision=49b83e2f5501273bb46fde02768ab2064b88c8f0
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.created=2023-11-12T00:07:22+00:00
# Tue, 14 Nov 2023 00:29:41 GMT
COPY dir:326e2e0244e2e1c327280e9778a484a786b9b9e6a2714cd83ab5e297b89945bd in / 
# Tue, 14 Nov 2023 00:29:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231112.0.191179' /etc/os-release
# Tue, 14 Nov 2023 00:29:43 GMT
ENV LANG=C.UTF-8
# Tue, 14 Nov 2023 00:29:43 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:455582f1306491ad2d8a6ac4475020ad953d50f499850ebafb08e0222bbcc914`  
		Last Modified: Tue, 14 Nov 2023 00:31:24 GMT  
		Size: 147.1 MB (147061615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf0cec5055ad0de6e32a3a567d0d2df42fdf3517493daad0887502a27f516d9`  
		Last Modified: Tue, 14 Nov 2023 00:31:04 GMT  
		Size: 8.1 KB (8129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20231112.0.191179`

```console
$ docker pull archlinux@sha256:1f83ba0580a15cd6ad1d02d62ad432ddc940f53f07d0e39c8982d6c9c74e53e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20231112.0.191179` - linux; amd64

```console
$ docker pull archlinux@sha256:6d4096442644ee6d7f71f3b60ff79d605098f7bdb4467f41d0608894e25a7ee8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147069744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e73f0f3a7ab45c7f43cd2b53dc7d86376505a8ae116a58b33abac4a257e093d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.title=Arch Linux base Image
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Tue, 14 Nov 2023 00:29:34 GMT
LABEL org.opencontainers.image.version=20231112.0.191179
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.revision=49b83e2f5501273bb46fde02768ab2064b88c8f0
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.created=2023-11-12T00:07:22+00:00
# Tue, 14 Nov 2023 00:29:41 GMT
COPY dir:326e2e0244e2e1c327280e9778a484a786b9b9e6a2714cd83ab5e297b89945bd in / 
# Tue, 14 Nov 2023 00:29:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231112.0.191179' /etc/os-release
# Tue, 14 Nov 2023 00:29:43 GMT
ENV LANG=C.UTF-8
# Tue, 14 Nov 2023 00:29:43 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:455582f1306491ad2d8a6ac4475020ad953d50f499850ebafb08e0222bbcc914`  
		Last Modified: Tue, 14 Nov 2023 00:31:24 GMT  
		Size: 147.1 MB (147061615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf0cec5055ad0de6e32a3a567d0d2df42fdf3517493daad0887502a27f516d9`  
		Last Modified: Tue, 14 Nov 2023 00:31:04 GMT  
		Size: 8.1 KB (8129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:6bcfe7dee58e56aa5f2066b4bb18f5e931c3131ead1d6697b8b41d2d4c725126
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:19cbb2b7e11cc9f3a3f0ed2dc13236f8d21ff8f0a967e17dad2cec9474b247f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.3 MB (265331768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a09b9d2e2fa3bd50fc8eb07a8757ccc8f2d0ffe7a368ace6b6e1d8dca5bf3c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Arch Linux base-devel Image
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Tue, 17 Oct 2023 00:23:33 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Tue, 17 Oct 2023 00:23:33 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.version=20231112.0.191179
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.revision=49b83e2f5501273bb46fde02768ab2064b88c8f0
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.created=2023-11-12T00:07:25+00:00
# Tue, 14 Nov 2023 00:30:44 GMT
COPY dir:926bc882e0a5e3f415f607407730914623c4aa43f43ae9801e45d39a7f44d0cb in / 
# Tue, 14 Nov 2023 00:30:47 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231112.0.191179' /etc/os-release
# Tue, 14 Nov 2023 00:30:47 GMT
ENV LANG=C.UTF-8
# Tue, 14 Nov 2023 00:30:47 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:bf08203b209668ace47a378e13d623ace4bb5eaf983591b519b1f9be9ac8e214`  
		Last Modified: Tue, 14 Nov 2023 00:32:10 GMT  
		Size: 265.3 MB (265322849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f217216617a7dd0cf1e2b9a6f1396c0562c099cb49048f51dcfefe84a718ed`  
		Last Modified: Tue, 14 Nov 2023 00:31:35 GMT  
		Size: 8.9 KB (8919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20231112.0.191179`

```console
$ docker pull archlinux@sha256:6bcfe7dee58e56aa5f2066b4bb18f5e931c3131ead1d6697b8b41d2d4c725126
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20231112.0.191179` - linux; amd64

```console
$ docker pull archlinux@sha256:19cbb2b7e11cc9f3a3f0ed2dc13236f8d21ff8f0a967e17dad2cec9474b247f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.3 MB (265331768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a09b9d2e2fa3bd50fc8eb07a8757ccc8f2d0ffe7a368ace6b6e1d8dca5bf3c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Arch Linux base-devel Image
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Tue, 17 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Tue, 17 Oct 2023 00:23:33 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Tue, 17 Oct 2023 00:23:33 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.version=20231112.0.191179
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.revision=49b83e2f5501273bb46fde02768ab2064b88c8f0
# Tue, 14 Nov 2023 00:30:33 GMT
LABEL org.opencontainers.image.created=2023-11-12T00:07:25+00:00
# Tue, 14 Nov 2023 00:30:44 GMT
COPY dir:926bc882e0a5e3f415f607407730914623c4aa43f43ae9801e45d39a7f44d0cb in / 
# Tue, 14 Nov 2023 00:30:47 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231112.0.191179' /etc/os-release
# Tue, 14 Nov 2023 00:30:47 GMT
ENV LANG=C.UTF-8
# Tue, 14 Nov 2023 00:30:47 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:bf08203b209668ace47a378e13d623ace4bb5eaf983591b519b1f9be9ac8e214`  
		Last Modified: Tue, 14 Nov 2023 00:32:10 GMT  
		Size: 265.3 MB (265322849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f217216617a7dd0cf1e2b9a6f1396c0562c099cb49048f51dcfefe84a718ed`  
		Last Modified: Tue, 14 Nov 2023 00:31:35 GMT  
		Size: 8.9 KB (8919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:1f83ba0580a15cd6ad1d02d62ad432ddc940f53f07d0e39c8982d6c9c74e53e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:6d4096442644ee6d7f71f3b60ff79d605098f7bdb4467f41d0608894e25a7ee8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147069744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e73f0f3a7ab45c7f43cd2b53dc7d86376505a8ae116a58b33abac4a257e093d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.title=Arch Linux base Image
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.description=Official containerd image of Arch Linux, a simple, lightweight Linux distribution aimed for flexibility.
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.authors=Santiago Torres-Arias <santiago@archlinux.org> (@SantiagoTorres), Christian Rebischke <Chris.Rebischke@archlinux.org> (@shibumi), Justin Kromlinger <hashworks@archlinux.org> (@hashworks)
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.url=https://gitlab.archlinux.org/archlinux/archlinux-docker/-/blob/master/README.md
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.documentation=https://wiki.archlinux.org/title/Docker#Arch_Linux
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.source=https://gitlab.archlinux.org/archlinux/archlinux-docker
# Tue, 17 Oct 2023 00:22:35 GMT
LABEL org.opencontainers.image.licenses=GPL-3.0-or-later
# Tue, 14 Nov 2023 00:29:34 GMT
LABEL org.opencontainers.image.version=20231112.0.191179
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.revision=49b83e2f5501273bb46fde02768ab2064b88c8f0
# Tue, 14 Nov 2023 00:29:35 GMT
LABEL org.opencontainers.image.created=2023-11-12T00:07:22+00:00
# Tue, 14 Nov 2023 00:29:41 GMT
COPY dir:326e2e0244e2e1c327280e9778a484a786b9b9e6a2714cd83ab5e297b89945bd in / 
# Tue, 14 Nov 2023 00:29:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231112.0.191179' /etc/os-release
# Tue, 14 Nov 2023 00:29:43 GMT
ENV LANG=C.UTF-8
# Tue, 14 Nov 2023 00:29:43 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:455582f1306491ad2d8a6ac4475020ad953d50f499850ebafb08e0222bbcc914`  
		Last Modified: Tue, 14 Nov 2023 00:31:24 GMT  
		Size: 147.1 MB (147061615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf0cec5055ad0de6e32a3a567d0d2df42fdf3517493daad0887502a27f516d9`  
		Last Modified: Tue, 14 Nov 2023 00:31:04 GMT  
		Size: 8.1 KB (8129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
