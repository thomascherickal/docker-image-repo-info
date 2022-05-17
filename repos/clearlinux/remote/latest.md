## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:0a62c93132d124381b57576cf243f4bad259357ef98c46bcf889d2fe3971a5fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:8050be0ed83b56423b9b45bc91c85d965c28ea182caa7c8cb5ee0d25c7dd70e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88126636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e421e45818376b81af180adcae4b624a828a85a701813fc7fcb400ea41737c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 17 May 2022 19:19:40 GMT
ADD file:cd8f85ce17208b91fb3a217d1eb96aa90e4de41f4a3d3e5479351cce3eb4928c in / 
# Tue, 17 May 2022 19:19:41 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 17 May 2022 19:19:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:eb66f477a4431dbb0c97c5127bc0d9f534317b17bc653d59ab0c6be597bbcd44`  
		Last Modified: Tue, 17 May 2022 19:20:03 GMT  
		Size: 88.1 MB (88126420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b64cf8d7cf920c3ac636f1c9e97547cb78cd374c9965f85397c1e8842f3d929`  
		Last Modified: Tue, 17 May 2022 19:19:51 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
