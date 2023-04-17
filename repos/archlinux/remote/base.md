## `archlinux:base`

```console
$ docker pull archlinux@sha256:0376f7766d553ea977189af55c1ace9f6678ceb11169b4d043197f252f41bc05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:fb43c930391cd5a85b1ac2e52284869b959e7bd94b028be7291fa20eecbaf7c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143109436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69316df6e84a856f5e586dbc009ab9ea61227a7f70fc68864feb72728df318ba`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 17 Apr 2023 19:20:44 GMT
COPY dir:a1b7299db54d48d85622f03c82636d895e1f7c49ff486cb8dd06f16963ee62f6 in / 
# Mon, 17 Apr 2023 19:20:45 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 17 Apr 2023 19:20:45 GMT
ENV LANG=C.UTF-8
# Mon, 17 Apr 2023 19:20:45 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:413993b4ae12f0af2de5c7ae744744c4073f7250fe016fe5fde18ecd4e865a33`  
		Last Modified: Mon, 17 Apr 2023 19:22:35 GMT  
		Size: 143.1 MB (143101465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13192c5fb17674c6624f7674528976e9435e7a26f2cfaa82afd1099ad62b786b`  
		Last Modified: Mon, 17 Apr 2023 19:22:16 GMT  
		Size: 8.0 KB (7971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
