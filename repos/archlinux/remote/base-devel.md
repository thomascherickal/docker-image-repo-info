## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ac93e93490a71b30bd8d272ea32071f5380cdc6cf49a8a3fb44b67454b33ce3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:1b89c35fa7e0edc4ed863dc0556a84579bf82e57a5cb4993f2840d7400c09273
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223785056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0472ed96157702bff6dda67efefff6ab38abe7603735ccff692291eeab7d5543`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:21:01 GMT
COPY dir:e63c09bfc3564481675b4d0a42923874135b9e688f480a88b73952d1456308b4 in / 
# Mon, 25 Jul 2022 18:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1b64ff134606a0a90a5a5d9a291a36c4d715d2a0e87a57c916e0245cacf1c079`  
		Last Modified: Mon, 25 Jul 2022 18:22:31 GMT  
		Size: 223.8 MB (223776883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8f2ee8107d38684c0fb84f8613cc7a60b28d73653f0d9aba1caab716baa7f3`  
		Last Modified: Mon, 25 Jul 2022 18:21:56 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
