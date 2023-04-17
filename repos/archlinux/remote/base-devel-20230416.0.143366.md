## `archlinux:base-devel-20230416.0.143366`

```console
$ docker pull archlinux@sha256:8ccfd0f5398445f94119e2619c92c5f5ecbbafd930035f3c50da3f4b79d3e30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230416.0.143366` - linux; amd64

```console
$ docker pull archlinux@sha256:4af23da5b5a7f5831a4d3e057262f7076fa40cdb740bb33138f4c0278057367b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246175012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33a093dd92500d5af34badc53551208531564ee08d9365575e612019389d2e94`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 17 Apr 2023 19:21:51 GMT
COPY dir:7f85f195c464c19c5796fd46a1b11b816dae9d6ee1651aa5db7198122aa5f38b in / 
# Mon, 17 Apr 2023 19:21:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 17 Apr 2023 19:21:54 GMT
ENV LANG=C.UTF-8
# Mon, 17 Apr 2023 19:21:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:6933545aab133877e83b1934f12156b21b43615807ae95c83f6f392da8978d7a`  
		Last Modified: Mon, 17 Apr 2023 19:23:22 GMT  
		Size: 246.2 MB (246166308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6abd813b45b8881f59c66702386010a49f937b6fa0f10106e9fab79e3e43a1`  
		Last Modified: Mon, 17 Apr 2023 19:22:46 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
