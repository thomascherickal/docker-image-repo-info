## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:92252ab2948ab2686358bd725eab2a279fbfa4ac5159bd260fa8a81a4fd301c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:ecc6d1b83c5b45f516ae4fd85c3eace118d8241cfc195bccc77f9237062473da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81829800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f32532c3649dc4ae0d70ffba6ae2f5879cc625d2ec199d9375a52d31a0f36a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 15 May 2023 18:23:14 GMT
ADD file:a1e63f2291b1cfd8936c4fa0b136a84d4df11b73c47ad2108ab196807c1e4345 in / 
# Mon, 15 May 2023 18:23:15 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 15 May 2023 18:23:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f382c1fbba3c801d1cdb2fbc75c35c8fe7252ba96f55c1f55754874e7ff1dd92`  
		Last Modified: Mon, 15 May 2023 18:23:32 GMT  
		Size: 81.8 MB (81829583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da0cc38946b6912b95c46491dcab98c97d963e815a79552adf70c4b70465201`  
		Last Modified: Mon, 15 May 2023 18:23:22 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
