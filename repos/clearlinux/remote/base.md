## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:e9c21be402a48391ee1266fd562ffebb23d91b176bea4fe3bdd6d0a4fe3841cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:a503b193b4fe9c0063b9947024896093150d452974e88594d14209141e022991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94788501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b969b866dcbffb6b1d4d53dd4acdb31febc6c4506e6fe1b2da709934681292cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 11 Jul 2022 22:23:13 GMT
ADD file:1dabf212e4ad6716e9e5d9de34dd67dfacaf8579e1c292d3997e043540f8d02c in / 
# Mon, 11 Jul 2022 22:23:15 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 11 Jul 2022 22:23:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:88d47bfda9982c6574c43d0bb82a39272468808652e493bf73130aa762c0c71d`  
		Last Modified: Mon, 11 Jul 2022 22:23:38 GMT  
		Size: 94.8 MB (94788283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a2dad3e122fc815606ab2dcbc0120a62f4e664d89b8b07b08df640e55ccf3d`  
		Last Modified: Mon, 11 Jul 2022 22:23:24 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
