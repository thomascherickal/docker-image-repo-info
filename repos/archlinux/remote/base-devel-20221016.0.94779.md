## `archlinux:base-devel-20221016.0.94779`

```console
$ docker pull archlinux@sha256:9cf91027670400f2bb433099b169f0e66043bd1b36cb862ca8c93f5477f33e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221016.0.94779` - linux; amd64

```console
$ docker pull archlinux@sha256:23263bd573bd261aad1ef48f46cdd48f5c4dbb518d36aa6141451f33f1a193dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238588435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4762d526bd3e4f3d8530af5e527e2e08a38b561b228cdb1cf26b3d438a3977a1`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 17 Oct 2022 20:21:28 GMT
COPY dir:72f21198543403a33df8736c6971475109291aa93c981332933cba43d775a7e9 in / 
# Mon, 17 Oct 2022 20:21:32 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 17 Oct 2022 20:21:32 GMT
ENV LANG=C.UTF-8
# Mon, 17 Oct 2022 20:21:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:3a14fbd7ccbab6a976f52ef45034377241ac73a5fdc7751c4f5911c4e5c96e5b`  
		Last Modified: Mon, 17 Oct 2022 20:22:56 GMT  
		Size: 238.6 MB (238579869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbd28d763d5a3fe3506d9c0a400614cf50b831e1cea1173e9af0a9d3f54c250`  
		Last Modified: Mon, 17 Oct 2022 20:22:20 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
