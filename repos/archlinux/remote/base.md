## `archlinux:base`

```console
$ docker pull archlinux@sha256:0dcaf64d23b61a034fcfef1074703dd9c98eb2d6c3222bf1bff59c11c07e8618
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:07d4b2c847ad2f48223969212bf3c4089296dcfc73e2234c9bc3a035a068692e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134106685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a873ad8f908ca1aa9585166a53e5c89e792da2b5df94c816852b7098c4f42e78`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 22 Feb 2021 20:20:22 GMT
COPY dir:949a24967a74b2588b97ebfc31dc42e214d4817b7b6731c7c462285ebeacdd7f in / 
# Mon, 22 Feb 2021 20:20:23 GMT
RUN ldconfig
# Mon, 22 Feb 2021 20:20:23 GMT
ENV LANG=en_US.UTF-8
# Mon, 22 Feb 2021 20:20:23 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:5e95f935bf6022494923c6f51dd68f0c0c9c93e6a425a505ff506426e1dd6daa`  
		Last Modified: Mon, 22 Feb 2021 20:22:19 GMT  
		Size: 134.1 MB (134100046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd059a4eb43131ebc6b0db14754816c35716b926874e900413360454aa6fe479`  
		Last Modified: Mon, 22 Feb 2021 20:21:53 GMT  
		Size: 6.6 KB (6639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
