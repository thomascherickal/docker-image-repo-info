## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ecba82d77702d2e6a821187a1ca6c2920fd45d07cb8ad0f26ceacee9e1a1839d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:fcb51d97b47e7ec84f6c288d85f4f8e68ec767b9a5870c774ad950d0e419c2d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234741351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f80c77eff27fe15137ecd13d9a4f76632e9b62e1dd054176518a177d752ec9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 29 Aug 2022 18:23:21 GMT
COPY dir:ed2fc1c49ba037e42524baf0eda8f8cd554273562d224b67632edd6be6937b3f in / 
# Mon, 29 Aug 2022 18:23:24 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 29 Aug 2022 18:23:24 GMT
ENV LANG=C.UTF-8
# Mon, 29 Aug 2022 18:23:24 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ccd1bf5def59f67059c64dfda047e597a6317aa3c2af90f80f1982d00f6b3332`  
		Last Modified: Mon, 29 Aug 2022 18:25:15 GMT  
		Size: 234.7 MB (234732582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a660ba1fd0faf46937f17df91a0dce51ee00aa29282232fad4b32879d87511c8`  
		Last Modified: Mon, 29 Aug 2022 18:24:38 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
