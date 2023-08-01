## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:efbf3d3f91d260dbc45d7f3a00a3d2ec91582e29ac4372a5f350d962735a0722
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:8c28882f89fee4a07534aa502d95b32d1254f23ffd4fd1ec44a13b3e7657f368
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67392633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8866302d9b65d57de42f5eb80a393dee033de33df4ba3ae7e58a91087803c882`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 31 Jul 2023 23:19:31 GMT
ADD file:509deaf84ba267c46a6df163388c8fac233ee9c1382f7f036c250e1a08f22b6d in / 
# Mon, 31 Jul 2023 23:19:32 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 31 Jul 2023 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b32cc9e70a80c749815b1c5a2a09bfd2ac6cecad3079e84dc2ee4120ab41ef9e`  
		Last Modified: Mon, 31 Jul 2023 23:19:49 GMT  
		Size: 67.4 MB (67392416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355c07bf78510deabd6921b6c88594a33ac968843e8ab623a316c0c033591e67`  
		Last Modified: Mon, 31 Jul 2023 23:19:41 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
