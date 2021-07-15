## `archlinux:base`

```console
$ docker pull archlinux@sha256:f89922ba60f7f19fc82ed1b23f6d701a9c8fccf38e077623f7f5009d23870fe5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:35fc5090fb0be52698eeb31202c4073746b2977a5f169722dd54c9914b1f38f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134529272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f583c742842d4f49b1a3a91efbe746dd58f52a3f088fbf76ac8338f8ada6ff`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Jul 2021 19:20:05 GMT
COPY dir:ecf75594c53765f49889df8cf066d25691cad36fac448bc2f0b8688bc4be24db in / 
# Mon, 12 Jul 2021 19:20:07 GMT
RUN ldconfig
# Mon, 12 Jul 2021 19:20:07 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Jul 2021 19:20:08 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:bfd5ce7f960bebec3db2fe578fce377b8bd7895486e43d32a9b6a29e88013d89`  
		Last Modified: Mon, 12 Jul 2021 19:21:59 GMT  
		Size: 134.5 MB (134522610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d67c964d81a6cd3a5f68e87c287805e56eb69b7bfb6a6752aa07bbadeff834f`  
		Last Modified: Mon, 12 Jul 2021 19:21:39 GMT  
		Size: 6.7 KB (6662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
