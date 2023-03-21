## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:32ed98462e6148e5f051f72452c1a03dc32ca443cec6a9986cabb5121104a8b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:bdc1f495f1a1cfc8a22a6b9b4c1f1e4dd1bf81a805e3fddcf4e74382d35716f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88279054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a411c89bc81a433ad12d34b9230e6cc800aee81c9829d6cfe5c666fc0b5b32fb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 20 Mar 2023 23:31:03 GMT
ADD file:b1f8986b59a1ecd1b315cb1db46dfb93ec95edfe6a5418e1df8fe045f57b107e in / 
# Mon, 20 Mar 2023 23:31:04 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 20 Mar 2023 23:31:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d16d62c79f81b6d3656a02e9f878fc08e74e95910a48ee1660ea18e10c369552`  
		Last Modified: Mon, 20 Mar 2023 23:31:22 GMT  
		Size: 88.3 MB (88278836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a739224896f1ed859de562ea1290408f105be559d27cffbb2563078895f6f671`  
		Last Modified: Mon, 20 Mar 2023 23:31:12 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
