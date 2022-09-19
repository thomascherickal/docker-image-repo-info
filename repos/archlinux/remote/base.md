## `archlinux:base`

```console
$ docker pull archlinux@sha256:48806dfa92c35733e3d60435448fc8aa3fedf0cba96fcbad7afc47b2b1fc20e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:2cc0c392d7d9df6a437b3e43f2588ee3692dc73b001d2c552b8e47c74c0d93ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138556957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f1632cc0df0f34b2c43f46c8798bc99be0651b1e783a7c7b9f1fb3fd28193d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:42:30 GMT
COPY dir:05a4953f90b0a55224fcfdf93d3ce965c2fac9bc38dd813d3eb3086b3ea9a5b6 in / 
# Mon, 19 Sep 2022 17:42:32 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:42:32 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:42:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c3298b3c36558f264f05f3c3b6308bcd7c89967eba2693dcaa52604b182f6db7`  
		Last Modified: Mon, 19 Sep 2022 17:44:15 GMT  
		Size: 138.5 MB (138548856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8518d59169bdd707ed1114bf9c4e7a0ff58862d147068bacd203d80588bb7bd1`  
		Last Modified: Mon, 19 Sep 2022 17:43:54 GMT  
		Size: 8.1 KB (8101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
