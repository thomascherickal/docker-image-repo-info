## `archlinux:latest`

```console
$ docker pull archlinux@sha256:c104009b470ee7866c42cbfc491aba018efe5e157184302ed5dcffda569adbda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:5d9d438364f5d53dab435509b2805aa5133c5e28194a1bfdd270e2589540e297
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (146951791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176850dc38ba578ead5ed3776f05021aba41b216e29a115c0193c2684c2f5d69`
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
# Tue, 31 Oct 2023 18:22:13 GMT
LABEL org.opencontainers.image.version=20231029.0.188123
# Tue, 31 Oct 2023 18:22:14 GMT
LABEL org.opencontainers.image.revision=0ba93e3ec97e1d44ef9fd23f85ed4190a76aae20
# Tue, 31 Oct 2023 18:22:14 GMT
LABEL org.opencontainers.image.created=2023-10-29T00:07:11+00:00
# Tue, 31 Oct 2023 18:22:20 GMT
COPY dir:8d6eef4eb658a992332b3e9e29acb94cc520fb0cc46e5ab857a7a0c3e01bd6cd in / 
# Tue, 31 Oct 2023 18:22:21 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231029.0.188123' /etc/os-release
# Tue, 31 Oct 2023 18:22:21 GMT
ENV LANG=C.UTF-8
# Tue, 31 Oct 2023 18:22:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5f77560258b9b5438402ee09c41da08762396a0c7817bc146a72a67593b462ec`  
		Last Modified: Tue, 31 Oct 2023 18:24:03 GMT  
		Size: 146.9 MB (146943671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45fbe0d533b1753c8521565a9e7b659a5c95c80c769eb86bcc5538fbb23a30a`  
		Last Modified: Tue, 31 Oct 2023 18:23:44 GMT  
		Size: 8.1 KB (8120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
