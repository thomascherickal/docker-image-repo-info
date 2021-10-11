## `archlinux:base`

```console
$ docker pull archlinux@sha256:83e1e3c479d858588949749bd1e70655bf5715cdaa175ddbb3f1eda56502e066
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:ee412d4414d055e3c74ad1d409dbb6c1ec4084ad89776797527241f5eb4e57a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134380326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff43c89971b1498e8dc76cf085aec6eb101f05c161db5d2d76f830a783743fc`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 11 Oct 2021 18:20:27 GMT
COPY dir:f64637a0533e2c6aa4c5a77c7b59b76ae02b5d5fdaa94608e5682835df8dafc2 in / 
# Mon, 11 Oct 2021 18:20:29 GMT
RUN ldconfig
# Mon, 11 Oct 2021 18:20:29 GMT
ENV LANG=en_US.UTF-8
# Mon, 11 Oct 2021 18:20:29 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:43b64d7828da2cacaaf9c24702516e7b2ffdfd328fe847b2a12016d9c4b67f7e`  
		Last Modified: Mon, 11 Oct 2021 18:22:11 GMT  
		Size: 134.4 MB (134373559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b841d880cc7838bf98f869ae74a64e3816003fe27f95165c2e63f881109d82`  
		Last Modified: Mon, 11 Oct 2021 18:21:52 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
