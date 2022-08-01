## `archlinux:base-devel-20220731.0.71623`

```console
$ docker pull archlinux@sha256:cc55357b6cf01d60f91a417792aa3c831459db75a7857f0dd5eed24fcd0e8f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220731.0.71623` - linux; amd64

```console
$ docker pull archlinux@sha256:45b95804a26d39e706d1e87e661ad0c04fad7ec819df3b68eb09a6b74c013b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233201131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbd1af5cfa4904d181710f3e108817790e9a3550e1968e837046b6502111d6c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 01 Aug 2022 21:21:01 GMT
COPY dir:58a775097c874727e6051dd7db3731e2f793cf5d33eac5c1a1d77eb0ae8ba115 in / 
# Mon, 01 Aug 2022 21:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 01 Aug 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 01 Aug 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:38cab039087fda714a03dcc8dbec451c5ed355ef11295a2c869545704aa47296`  
		Last Modified: Mon, 01 Aug 2022 21:22:35 GMT  
		Size: 233.2 MB (233192885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0519f846669778458a919d19c0391a93edfb1295a3bee866711e9e346be359f3`  
		Last Modified: Mon, 01 Aug 2022 21:22:00 GMT  
		Size: 8.2 KB (8246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
