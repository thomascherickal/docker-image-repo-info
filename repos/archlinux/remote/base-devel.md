## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:3683088c11c40a3e6958e1f57451cd70e50bee379327a6dc51a2d52990e9389a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:8734c79fdf12c2f2fff9b84b956206b53bc9c635ab3a39d7959a1eb8ae4cbb46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245353458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36842c45cfb121c045c9d768f7d265878b3338262889a0d5b54828d3ef4c8721`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 20 Mar 2023 23:28:52 GMT
COPY dir:c59c7a69f5d4c27fcd3f871aa78a03d141f6be13ec1cb78c292d7b4cd5ebde15 in / 
# Mon, 20 Mar 2023 23:28:55 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 20 Mar 2023 23:28:55 GMT
ENV LANG=C.UTF-8
# Mon, 20 Mar 2023 23:28:55 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:147eb476785b20920ffcf09ebbaa213e0bbd9220a7f9608a87411b521a49e739`  
		Last Modified: Mon, 20 Mar 2023 23:30:09 GMT  
		Size: 245.3 MB (245344740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635d85a76f3903b23e4d023dc6c521310ffc530cdd383eee32e7f40087b4622`  
		Last Modified: Mon, 20 Mar 2023 23:29:37 GMT  
		Size: 8.7 KB (8718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
