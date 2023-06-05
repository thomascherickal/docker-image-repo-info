## `archlinux:latest`

```console
$ docker pull archlinux@sha256:90ac8e1075a9e2a4bd2fc657afccd05ce9626d627fdfb24a0108a4a2998319e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:5af2b0f645075a73bcb19e8c0f24b6b0d86a4305e1a84f9a53f9fd5e7bc0f648
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145896888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc56b88e36b9e33677b1ebf65bc238b80988c858ead662fe4b68249410fdf0c`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:22:42 GMT
COPY dir:592dbcf24bea6fe3bdd66c3cfbaf8792b7e8c2db39bf0c457b13a189d768bdfe in / 
# Mon, 05 Jun 2023 19:22:43 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:22:44 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:22:44 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f917b72a30c8e0ac2d82975c49979594120b14a17a5658078e43e438aa9d477e`  
		Last Modified: Mon, 05 Jun 2023 19:24:14 GMT  
		Size: 145.9 MB (145888851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ab89f191e8f779829d7535540fd66b8778a9f9241082933fdf59d9989490a3`  
		Last Modified: Mon, 05 Jun 2023 19:23:55 GMT  
		Size: 8.0 KB (8037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
