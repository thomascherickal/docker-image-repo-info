## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:b63a3b7ba6722c4b0327ce00d87d72c12c5d5570f3654820067a68ff8bde24b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:87c8950d8f9b03cda2edf198a9f27b3a318bccf9681a54bbbee3fd0cf64cb47e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88166171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcadc17efe993171155c590e5440a1f2455f509fede80972cd7acd708005ac6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 02 May 2022 18:23:08 GMT
ADD file:c908a9851ebde915b77f479c358da1708b962086a24fe81aa2728f9e0a4114a8 in / 
# Mon, 02 May 2022 18:23:09 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 02 May 2022 18:23:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b8f3c44ccafc0ee63b66f5fa61c0b5a2b266ae407c2077af0bd64cdf3f38d41`  
		Last Modified: Mon, 02 May 2022 18:23:31 GMT  
		Size: 88.2 MB (88165953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3078e5cbc9c4ddd825929ee80b524bc3c9d36879d4b6d6956c015e1f1c5186cd`  
		Last Modified: Mon, 02 May 2022 18:23:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
