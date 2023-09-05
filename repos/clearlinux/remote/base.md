## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:eb85be3a3a60a6290e7fec32368d34a2700cf235f24584f748152fb5189cdc51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:b0647ddcdcf5608737e27944651e3c23ed6dc4f8a812885ed974edea59627eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67524474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0fc6c3aa8499bbf2113831d95e7ccbef73e43decdd81bf8841e5a15e59b54f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 05 Sep 2023 22:19:31 GMT
ADD file:c0f2681e1db75b7114782d7428076a81705638252309b88e741a1d640d3e320e in / 
# Tue, 05 Sep 2023 22:19:32 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 05 Sep 2023 22:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2eb858ec6089a6af3472f949df7678cd3335498a266c911c41b034f19cab6c99`  
		Last Modified: Tue, 05 Sep 2023 22:19:48 GMT  
		Size: 67.5 MB (67524257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8abd17f62ccc5c0415b6339bf7f0f610c211c6af98c517d29549b97450b00`  
		Last Modified: Tue, 05 Sep 2023 22:19:40 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
