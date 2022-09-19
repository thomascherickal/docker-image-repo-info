## `archlinux:base-devel-20220918.0.86346`

```console
$ docker pull archlinux@sha256:61d07c024369c0d66ad1fdb1a72849f401cc1d06e997800b50a84d9998ee517a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220918.0.86346` - linux; amd64

```console
$ docker pull archlinux@sha256:c94a2633b402d2cf07343564a44b852b7ef1758af70d53edd13b697bac022a05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236824083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edad53189e9ee56eb28443e3c7fe9b7d7e68cf423a3af5ec58a66f70bd688f85`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:43:31 GMT
COPY dir:7a9f55aa3b47cf7267a8485c8101c9aa85637105151f39346dcfe8a465dd9744 in / 
# Mon, 19 Sep 2022 17:43:34 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:43:34 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:43:34 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:16a106e71ce5d7f920ae07e9d1d92e3b2da4ce2eada6f9df3f8839c1e3ca7679`  
		Last Modified: Mon, 19 Sep 2022 17:45:02 GMT  
		Size: 236.8 MB (236815311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e970fddd4fb5debb710a45d3dc67b8b425b7deb760c33292817d6f6e2c0140c8`  
		Last Modified: Mon, 19 Sep 2022 17:44:26 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
