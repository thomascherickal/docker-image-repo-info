## `archlinux:latest`

```console
$ docker pull archlinux@sha256:564cc0589ff36eda2fe49ba2087969bdf9504ed40e0caf4af3ce32792dfe2e08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:776985751d713b98847a12b92445d5c20cb0f3bf2f1006138c846910e893e309
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140307573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ba039072fc36cc356b8c264c53742a2d2ad32cb99a9d22f4a0816e1a177c59`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 17 Oct 2022 20:20:20 GMT
COPY dir:c7456ecf6cf7f091adcad437eebf10aacb77b315c46b0c599c375ef5973f1fdb in / 
# Mon, 17 Oct 2022 20:20:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 17 Oct 2022 20:20:22 GMT
ENV LANG=C.UTF-8
# Mon, 17 Oct 2022 20:20:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:792a03d1e3adb11813c97728231cd52b50bd237143c2a491bc0754f12d1a3921`  
		Last Modified: Mon, 17 Oct 2022 20:22:06 GMT  
		Size: 140.3 MB (140299657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b7c4f5d0d4bdb93625d3c69f9e7883ac252629a2364d224a0b8406bf830c10`  
		Last Modified: Mon, 17 Oct 2022 20:21:45 GMT  
		Size: 7.9 KB (7916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
