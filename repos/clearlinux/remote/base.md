## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:0fc2c04444a8e86a9467be7e420dff380ef3df611892cc19b43bba98d4209b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:979c1bdafcefd82cec5d7d764943782e37b7ffc9f76f39ebee3a8aef9627bebc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67526593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d373c194441e4f5b69c55ebbb8d4e88b6374888296230da34d96264612ec528`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 21 Aug 2023 19:22:23 GMT
ADD file:dd9dc5dac68201693a1f3091beaaac7029f4af9f09b77d3a7270819df1c05662 in / 
# Mon, 21 Aug 2023 19:22:24 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 21 Aug 2023 19:22:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a92498f4cf2743d3ab55993038322203445f86703cbee2fcc9baf8c890b44d84`  
		Last Modified: Mon, 21 Aug 2023 19:22:42 GMT  
		Size: 67.5 MB (67526376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cb9dfa065d7cd5586f7affb7813076a49c9f4b6b5652e02d659436ea3d76c`  
		Last Modified: Mon, 21 Aug 2023 19:22:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
