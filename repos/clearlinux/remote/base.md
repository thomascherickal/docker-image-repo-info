## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:1b6c771b2230117b6532959f5a2f5e6692a5d4e21bfb2f45e4dbace9898bdbe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:69d1869e836fcf29f01826ef8ea0e0b8e7d7cff06faeada6d8b96ed9c25df0d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88134218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ec4828e5a40f472b5598b8653d028debd2b483dd3a556306cb8099db159fa3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 13 Jun 2022 17:23:32 GMT
ADD file:e90c09906f362da7ec541d5733aa9c69b0498bb6fef08e62c8f0bffa392f4e6e in / 
# Mon, 13 Jun 2022 17:23:33 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 13 Jun 2022 17:23:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89429f98229f47d0e86a326c2bab485a5a0dfc81de3567589d60db1e5d9125a9`  
		Last Modified: Mon, 13 Jun 2022 17:23:55 GMT  
		Size: 88.1 MB (88134001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d05c1aedf7dc6d5c25068ae503395cc7e8c3a205347ff8c47e449fdb0f46a`  
		Last Modified: Mon, 13 Jun 2022 17:23:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
