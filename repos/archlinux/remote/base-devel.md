## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:da2cfd0975150f4fa2091141e6362e9630e0bb8fb20840c47fd6fa9bf0f0122b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:9988f99b27c40c82c00ff138c9541d3bbbb8d05bfbe678211c5a6923a4e84772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245230845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97342c4da63f8760b15bb7ad2028f7ede20591bdff0d1048974e6ec8f202f7bc`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:21:05 GMT
COPY dir:85e801d5104e24925c4ba0a585ff1227475b04c7885fc0d6a7b36658158629f6 in / 
# Mon, 06 Mar 2023 20:21:09 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:21:09 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:21:09 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:6df10e147b58b3665928d52d81decc4a5f82594edb43f401e10cdc3f33b8e778`  
		Last Modified: Mon, 06 Mar 2023 20:22:24 GMT  
		Size: 245.2 MB (245222117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a5e71ef32dcb7dbb34eb6268fc2fa886886227cd4a7f461151e750440b8c7b`  
		Last Modified: Mon, 06 Mar 2023 20:21:49 GMT  
		Size: 8.7 KB (8728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
