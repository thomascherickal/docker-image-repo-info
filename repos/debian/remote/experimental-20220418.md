## `debian:experimental-20220418`

```console
$ docker pull debian@sha256:80c775c1b7c5af36787782f0362d16420ef48ee3a35ac6f29e5b93a634b3967e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; riscv64

### `debian:experimental-20220418` - linux; riscv64

```console
$ docker pull debian@sha256:a1cead4d44ed77c5662eac9f2429556006120420caba2d19a63ec196fc62a185
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51757584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3dda1884db97d35d90d8cc9d6e29762b5d5a1efaa65abe6947b0ed8470c295`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 00:19:42 GMT
ADD file:eb73ccec6d534b35c3f0725251b8917d96bcd87d77d960d0a879ca91d2530a47 in / 
# Wed, 20 Apr 2022 00:19:44 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 00:23:27 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:62d036327287ffa181f78db1cedfa9a2d2ddc4c54f3c3838d75dae32e11ff1b1`  
		Last Modified: Wed, 20 Apr 2022 00:38:38 GMT  
		Size: 51.8 MB (51757356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6440a805ff86b05ccf55572b7ebe62afdf80683fe40032330d06f9f2896e63`  
		Last Modified: Wed, 20 Apr 2022 00:41:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
