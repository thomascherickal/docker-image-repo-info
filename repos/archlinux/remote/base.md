## `archlinux:base`

```console
$ docker pull archlinux@sha256:324d260803fa37bc2ff878a17fc13c49cb6352b023b64e58defa9d9fd5fdb792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:3a02e52d5d972230c491b102c3ac586f5299b558b1c501cb181c595e8ba7a40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4f097fbe6457d8905a5fb6cfb565c48b34f81a2c7d77479220d80937c17863`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:19:56 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Mon, 03 Oct 2022 21:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b75e13f2371cc7455e28feb7fbaf61bb6c038765c9de103decd343232f5259`  
		Last Modified: Mon, 03 Oct 2022 21:21:22 GMT  
		Size: 7.9 KB (7910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
