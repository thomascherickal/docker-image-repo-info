## `archlinux:base-devel-20220703.0.65849`

```console
$ docker pull archlinux@sha256:9d872e87b4c95a68690cca5059b7f94c21e85012588ee6747b81e1ea086a511c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220703.0.65849` - linux; amd64

```console
$ docker pull archlinux@sha256:53049d399a91434ca5e585628dbf61d5c16358f9072f6c19e82d592d3db0f4b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224953713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29399e094af8ce947149d1ab035a6b2dd7cbfdc63d3f0da3386f8d0e7a67956`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 05 Jul 2022 18:20:58 GMT
COPY dir:06e36920efdb794e87772824db6f663ce963a4cc4a4e1591fc000929c0c321bc in / 
# Tue, 05 Jul 2022 18:21:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 05 Jul 2022 18:21:01 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jul 2022 18:21:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:6f0704604a867486a68967c83322de257831b3f21a8c242940b5a8a88058e9dd`  
		Last Modified: Tue, 05 Jul 2022 18:22:20 GMT  
		Size: 224.9 MB (224945551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2577663b002bdddfbd1f2c069daeb57e9c9e0a477f46e4a329e1fd1370d32bc1`  
		Last Modified: Tue, 05 Jul 2022 18:21:47 GMT  
		Size: 8.2 KB (8162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
