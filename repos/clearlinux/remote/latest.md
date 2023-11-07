## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:41c996dd143d65e23f81441cad5305798c16f89ea74728714a9419beb25b3314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:171e4b54165192d887d65b6e3185a35b33f3698aae2546bd5108da8bce0de43c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68006523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb72699ebf336ee89b7c4cb5966f0aa991a4c15d6be77f8d91d0b48227d9f59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 06 Nov 2023 23:25:08 GMT
ADD file:a06b676a3833f3d8a6ebdf2b73fc58a7832bbe17c9c132eaad14222e2f4f96c7 in / 
# Mon, 06 Nov 2023 23:25:09 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Mon, 06 Nov 2023 23:25:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee66878453822f522cfb445061e94b403690f6a3950e9970abc0cb497a7b5a1e`  
		Last Modified: Mon, 06 Nov 2023 23:25:27 GMT  
		Size: 68.0 MB (68006310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889fe8b9b433ce52aefe58d1530e1fc8f4cb54584c60ee168c606cda217e883a`  
		Last Modified: Mon, 06 Nov 2023 23:25:18 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
