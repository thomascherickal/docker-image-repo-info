## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:6d9755c3ab4dc9a2a5a15f15488379a6d76380ca7bcd804f15de0a0ba3de20e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:3d48162a6b904323c00855dfe4e3844fff09c773cd28df83a3b0be02e4696da3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.6 MB (88626352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ae3d3ea9ab2dee69b74a5c2ed3678b8f66774de6847650ae2702b18f463ccd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 10 Jan 2022 21:24:29 GMT
ADD file:7b26c9f654ec4bd9e97689bcccdcf2b6c059553c3540febf3530dfc03de7f20e in / 
# Tue, 18 Jan 2022 18:24:19 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 18 Jan 2022 18:24:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:53a8393fabf6eb9e33abe90b2fdccb5b82a33989761ca36bc2473f5a9d538106`  
		Last Modified: Mon, 10 Jan 2022 21:24:50 GMT  
		Size: 88.6 MB (88626135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fce1f27e5a85847887340acea9b37df23d0f0b88f20113de61f5d1b9079f8a5`  
		Last Modified: Tue, 18 Jan 2022 18:24:31 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
