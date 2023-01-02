## `archlinux:base-devel-20230101.0.115167`

```console
$ docker pull archlinux@sha256:20f1ad0d1e75fcfd8b541de0f519d343430f30cb3f963b5adc8676c6091dd407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230101.0.115167` - linux; amd64

```console
$ docker pull archlinux@sha256:3a64011140ee44f1c11c62abdb0426b04791db4c342e7d092932ca9a583e75b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.2 MB (243227812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2e09c7919211f6c26a8aa57ca8aba7cd99ec53002b959087ac9581ce8dc7be`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:20:54 GMT
COPY dir:677ff053e258db1091a13c2e0d19dfb63a89c574c24c57260b5b72921ec06ee8 in / 
# Mon, 02 Jan 2023 18:20:57 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:20:57 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:20:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:62eaba580f07c2f8b6125f83da13ef8687865016ba06a46064202023afdf74f8`  
		Last Modified: Mon, 02 Jan 2023 18:22:25 GMT  
		Size: 243.2 MB (243219199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76e32eee8a9098df21fcc9166844129c4afc058df8515af76a22738c5829177`  
		Last Modified: Mon, 02 Jan 2023 18:21:49 GMT  
		Size: 8.6 KB (8613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
