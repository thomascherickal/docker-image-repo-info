## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:f3d0a802aafe83a020fa2674c52b4f2dde064833ec583a17d5ae91419560cc2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:e0d68cc44bb4471517c6e03c6152fb965f8608c8adbec959decf46415a7b7737
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265142917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668348447a0e17ab1181c56ccfe21c9c170754e98a3ad99085b7e7647a9af131`
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
# Tue, 31 Oct 2023 18:23:12 GMT
LABEL org.opencontainers.image.version=20231029.0.188123
# Tue, 31 Oct 2023 18:23:12 GMT
LABEL org.opencontainers.image.revision=0ba93e3ec97e1d44ef9fd23f85ed4190a76aae20
# Tue, 31 Oct 2023 18:23:12 GMT
LABEL org.opencontainers.image.created=2023-10-29T00:07:14+00:00
# Tue, 31 Oct 2023 18:23:23 GMT
COPY dir:b801cbd9815b9bc72ac3d04b4776906534e7fb691bbd6f0718e9d501c16bb4ee in / 
# Tue, 31 Oct 2023 18:23:26 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=20231029.0.188123' /etc/os-release
# Tue, 31 Oct 2023 18:23:26 GMT
ENV LANG=C.UTF-8
# Tue, 31 Oct 2023 18:23:26 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b372719b3243ce3bc862a4c8c9c601a21d242a6a2ffb4ce2076f2294083081ff`  
		Last Modified: Tue, 31 Oct 2023 18:24:54 GMT  
		Size: 265.1 MB (265133968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5cacb95c9d87cab97e09dba064a5932c571bbcfd47b979d426ae203b4bebde`  
		Last Modified: Tue, 31 Oct 2023 18:24:14 GMT  
		Size: 8.9 KB (8949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
