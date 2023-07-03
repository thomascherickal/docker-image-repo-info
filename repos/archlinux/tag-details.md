<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230702.0.161694`](#archlinuxbase-202307020161694)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230702.0.161694`](#archlinuxbase-devel-202307020161694)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:6568d3f1f278827a4a7d8537f80c2ae36982829a0c6bccff4cec081774025472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:f08cf3f1884b455dee7d6af9ffb24918609badf96334c859ef8dd135d486d382
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146657836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6038e9f9308080e7d0696ecd1397e29337e5d41aa090559f81c40c165f324a4f`
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
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.version=20230702.0.161694
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.created=2023-07-02T00:07:57+00:00
# Mon, 03 Jul 2023 19:18:45 GMT
COPY dir:3e5aa2ec061d72c12fc642d448a846a35043e0221c9e3d42f473b5ae7dcb7dc5 in / 
# Mon, 03 Jul 2023 19:18:47 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230702.0.161694' /etc/os-release
# Mon, 03 Jul 2023 19:18:47 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 19:18:47 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8afbd7dc1c1db9d85116124f9c3cd55960dd8d50eb3b5f906281a36aaa2e0f76`  
		Last Modified: Mon, 03 Jul 2023 19:20:29 GMT  
		Size: 146.6 MB (146649747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3910bd92483c4f36a41cf3948d9e36596e1d3918efcc1b9cf98e394b3be227d`  
		Last Modified: Mon, 03 Jul 2023 19:20:09 GMT  
		Size: 8.1 KB (8089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230702.0.161694`

```console
$ docker pull archlinux@sha256:6568d3f1f278827a4a7d8537f80c2ae36982829a0c6bccff4cec081774025472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230702.0.161694` - linux; amd64

```console
$ docker pull archlinux@sha256:f08cf3f1884b455dee7d6af9ffb24918609badf96334c859ef8dd135d486d382
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146657836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6038e9f9308080e7d0696ecd1397e29337e5d41aa090559f81c40c165f324a4f`
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
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.version=20230702.0.161694
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.created=2023-07-02T00:07:57+00:00
# Mon, 03 Jul 2023 19:18:45 GMT
COPY dir:3e5aa2ec061d72c12fc642d448a846a35043e0221c9e3d42f473b5ae7dcb7dc5 in / 
# Mon, 03 Jul 2023 19:18:47 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230702.0.161694' /etc/os-release
# Mon, 03 Jul 2023 19:18:47 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 19:18:47 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8afbd7dc1c1db9d85116124f9c3cd55960dd8d50eb3b5f906281a36aaa2e0f76`  
		Last Modified: Mon, 03 Jul 2023 19:20:29 GMT  
		Size: 146.6 MB (146649747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3910bd92483c4f36a41cf3948d9e36596e1d3918efcc1b9cf98e394b3be227d`  
		Last Modified: Mon, 03 Jul 2023 19:20:09 GMT  
		Size: 8.1 KB (8089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:100638d64bf2fea01277c24ca93eecc0ffcce7bac17b39cdaad278a1bcb0907e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:0335bec3fb92997fcb416e3ee370a6f904a01931753fd8a42b58b117581cbe8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263467034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc75670fc6d2b6d24cac17e0248270899047e79f8a37f3a9366ce4de4ba9e6d`
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
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.version=20230702.0.161694
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.created=2023-07-02T00:08:00+00:00
# Mon, 03 Jul 2023 19:19:49 GMT
COPY dir:237e0652b40ee6ad57dbab5012a67a578b9640e748113daa6b62d6bde6d5ce6a in / 
# Mon, 03 Jul 2023 19:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230702.0.161694' /etc/os-release
# Mon, 03 Jul 2023 19:19:52 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 19:19:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:0049f4cadd706ce3a3877bcc732ebbc18e87a54c674506a57e3a57f6568c652a`  
		Last Modified: Mon, 03 Jul 2023 19:21:16 GMT  
		Size: 263.5 MB (263458156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04ca77e72839263b0ad71d0310f0411b8e2207e86c31fb7cc9a6ccd0930ea20`  
		Last Modified: Mon, 03 Jul 2023 19:20:40 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230702.0.161694`

```console
$ docker pull archlinux@sha256:100638d64bf2fea01277c24ca93eecc0ffcce7bac17b39cdaad278a1bcb0907e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230702.0.161694` - linux; amd64

```console
$ docker pull archlinux@sha256:0335bec3fb92997fcb416e3ee370a6f904a01931753fd8a42b58b117581cbe8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263467034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc75670fc6d2b6d24cac17e0248270899047e79f8a37f3a9366ce4de4ba9e6d`
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
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.version=20230702.0.161694
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 03 Jul 2023 19:19:38 GMT
LABEL org.opencontainers.image.created=2023-07-02T00:08:00+00:00
# Mon, 03 Jul 2023 19:19:49 GMT
COPY dir:237e0652b40ee6ad57dbab5012a67a578b9640e748113daa6b62d6bde6d5ce6a in / 
# Mon, 03 Jul 2023 19:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230702.0.161694' /etc/os-release
# Mon, 03 Jul 2023 19:19:52 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 19:19:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:0049f4cadd706ce3a3877bcc732ebbc18e87a54c674506a57e3a57f6568c652a`  
		Last Modified: Mon, 03 Jul 2023 19:21:16 GMT  
		Size: 263.5 MB (263458156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04ca77e72839263b0ad71d0310f0411b8e2207e86c31fb7cc9a6ccd0930ea20`  
		Last Modified: Mon, 03 Jul 2023 19:20:40 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:6568d3f1f278827a4a7d8537f80c2ae36982829a0c6bccff4cec081774025472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:f08cf3f1884b455dee7d6af9ffb24918609badf96334c859ef8dd135d486d382
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146657836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6038e9f9308080e7d0696ecd1397e29337e5d41aa090559f81c40c165f324a4f`
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
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.version=20230702.0.161694
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.revision=301942f9e5995770cb5e4dedb4fe9166afa4806d
# Mon, 03 Jul 2023 19:18:39 GMT
LABEL org.opencontainers.image.created=2023-07-02T00:07:57+00:00
# Mon, 03 Jul 2023 19:18:45 GMT
COPY dir:3e5aa2ec061d72c12fc642d448a846a35043e0221c9e3d42f473b5ae7dcb7dc5 in / 
# Mon, 03 Jul 2023 19:18:47 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20230702.0.161694' /etc/os-release
# Mon, 03 Jul 2023 19:18:47 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 19:18:47 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8afbd7dc1c1db9d85116124f9c3cd55960dd8d50eb3b5f906281a36aaa2e0f76`  
		Last Modified: Mon, 03 Jul 2023 19:20:29 GMT  
		Size: 146.6 MB (146649747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3910bd92483c4f36a41cf3948d9e36596e1d3918efcc1b9cf98e394b3be227d`  
		Last Modified: Mon, 03 Jul 2023 19:20:09 GMT  
		Size: 8.1 KB (8089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
