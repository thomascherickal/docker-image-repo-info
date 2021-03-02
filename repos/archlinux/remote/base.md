## `archlinux:base`

```console
$ docker pull archlinux@sha256:d0b6814e395dcec2848613f4e3189db2d8bb70a94d03a960a9ad538486133f77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:852ffb99e14fc23b5f7bd9791c60bb47ffc2525f5f6e490f768b96db38a16672
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134162872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4967f6f37d8afaa35d9cf8fa64c98f112c04cc812591978da56dc450aadd19c9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Mar 2021 23:20:12 GMT
COPY dir:d5c75862066a89075e4599d7295c7c34de5f4f3e543783ac0833f6cb874ae09f in / 
# Mon, 01 Mar 2021 23:20:13 GMT
RUN ldconfig
# Mon, 01 Mar 2021 23:20:13 GMT
ENV LANG=en_US.UTF-8
# Mon, 01 Mar 2021 23:20:14 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5b0038b368fd7ff840977d427f412a5d2f25cebc0dadd8220b01e37e2a7be2cf`  
		Last Modified: Mon, 01 Mar 2021 23:22:13 GMT  
		Size: 134.2 MB (134156249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8e774cc55a687275f7b26b1242c3931c641582ae7f2cee3a0300ab49d74c62`  
		Last Modified: Mon, 01 Mar 2021 23:21:47 GMT  
		Size: 6.6 KB (6623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
