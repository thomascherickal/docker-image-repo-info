## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:b1cb12b97986535ba9a3b549df05b427ee6f7f1abc572c368596c0e04603b642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:e9ba00eef89b23dc7c0a4ee3cb301ca5313b2b6f8a9a4b2ab6fadfe80822d412
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.1 MB (89142699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37acd76082b93c72b65b30c7bc7417f4a952e84b715b87c94ed5cea8b755e64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 02 Jan 2023 18:22:50 GMT
ADD file:0ad5844c71404a7a2e33df368c71efb568b104f44d303d362877a29756e44d97 in / 
# Mon, 02 Jan 2023 18:22:51 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 02 Jan 2023 18:22:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6aa2bda748dd8e58ff4811121d2c70c94f5ed27d4938b820e158b77ef98b7011`  
		Last Modified: Mon, 02 Jan 2023 18:23:10 GMT  
		Size: 89.1 MB (89142481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9be55e36e21559104ac4f341de90ab2caa4736a9035fd4b6688e60a46b522a`  
		Last Modified: Mon, 02 Jan 2023 18:22:59 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
