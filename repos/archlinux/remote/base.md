## `archlinux:base`

```console
$ docker pull archlinux@sha256:9a50fe91cbbd5657250398244ef8d41aeb80d17ad3fed0976fd1bdd95b7a8c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:9e06205bd2354044b75f4f4ef2877c00836207f9624aef45e3f7f9376821dd8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133159732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d141e5673e41091597be95eec1e76494f76483704b65a5e80829e16d69e06b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 21 Feb 2022 18:20:24 GMT
COPY dir:06917351dd90005713bb3fe6ff64418ed0b3b853d8496f57c475ba569deb065a in / 
# Mon, 21 Feb 2022 18:20:25 GMT
RUN ldconfig
# Mon, 21 Feb 2022 18:20:25 GMT
ENV LANG=en_US.UTF-8
# Mon, 21 Feb 2022 18:20:26 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9ae2c166397cf2eca6011844d98aaa681676950740665ea763fe27351bd6f8d5`  
		Last Modified: Mon, 21 Feb 2022 18:22:06 GMT  
		Size: 133.2 MB (133152988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca2b2a1f03561a60a1abe7518001671ff207b38575f7e79e0ae8d828f026d4`  
		Last Modified: Mon, 21 Feb 2022 18:21:47 GMT  
		Size: 6.7 KB (6744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
