## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:4afb3c18fdc8ebd3229e98a4901caeb5eb2e8e08037b3f4e81b04aa7520bff82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:30cd70376360b9408e30a1e1b370d156471a1f4cf18cb190bd98e30a471995b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88219041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b887a704990a390ccdcf289f064b06884f823c2d4c2240ba392c717f168bfd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 21 Jun 2022 22:22:51 GMT
ADD file:0eebb8d51d0d09f0adc66f7ecc0e4b4f1c35c9974dcee1c373b3dfd3146d2ceb in / 
# Tue, 21 Jun 2022 22:22:52 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Tue, 21 Jun 2022 22:22:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e0cd4f7562d0c7ee364e9e29d8904304e99f111834c0a252560d591f267e362`  
		Last Modified: Tue, 21 Jun 2022 22:23:15 GMT  
		Size: 88.2 MB (88218824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382cefa97a9e793b016733478d7ec8c379084efa3f66b68a92c34e83447e99ee`  
		Last Modified: Tue, 21 Jun 2022 22:23:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
