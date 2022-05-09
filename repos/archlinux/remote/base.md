## `archlinux:base`

```console
$ docker pull archlinux@sha256:1a41747e580242f84d43743662a7c8af73e8c379b0cd44ed636efbd3f19b19db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:e36c2dad19a7cdd51c8ad8f8922b784d11245c22418c49fead56b27af7bc5a9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132744292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433f486b31ada5bd714c45d7a876bf4f5f2b8fe7dd4ffe156e46fe597effd7a`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 09 May 2022 18:19:51 GMT
COPY dir:8102286307ac8b6749f05db3f72a8bb9b21cc51b2501eac683940c7be9ea02f4 in / 
# Mon, 09 May 2022 18:19:52 GMT
RUN ldconfig
# Mon, 09 May 2022 18:19:53 GMT
ENV LANG=en_US.UTF-8
# Mon, 09 May 2022 18:19:53 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:546907580fbd98b6ccb0a9fd384a92bc9fcbc8416e2f9c735aa02be6892029f0`  
		Last Modified: Mon, 09 May 2022 18:21:39 GMT  
		Size: 132.7 MB (132737116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8df19ece1a435e0c13cc7813b02d6be73603185beecca7b2554c6fb4d93ba0`  
		Last Modified: Mon, 09 May 2022 18:21:19 GMT  
		Size: 7.2 KB (7176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
