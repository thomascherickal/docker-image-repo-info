## `archlinux:base-devel-20230312.0.133040`

```console
$ docker pull archlinux@sha256:a1a2a043d8da23e7b5dc4ed317eb347fdba2bbfb1ef16a0f4a3b11af079fe4fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230312.0.133040` - linux; amd64

```console
$ docker pull archlinux@sha256:22c7ac88ee00e5be95c044b4dae7776e02d695399556ed7c3496384a49c6d8d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245231648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c348c74f0463466776cfe512ee909b9f9ab937eb3a0fbd9954379db7ba06f`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:21:07 GMT
COPY dir:6cd30a0c7a3ffa597ef65b4f3d914b13d51c8e2a70299f0eec09c6804be58e74 in / 
# Mon, 13 Mar 2023 20:21:10 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:21:11 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:21:11 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1c7df861908c5cdc63525ce742a3331ef82e3d297ab2950091737a8bdd823c1a`  
		Last Modified: Mon, 13 Mar 2023 20:22:25 GMT  
		Size: 245.2 MB (245222932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae8051f50ebcbcea2f4dd988a67851d02e9ddbe134e3539dbe69ef14416256`  
		Last Modified: Mon, 13 Mar 2023 20:21:52 GMT  
		Size: 8.7 KB (8716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
