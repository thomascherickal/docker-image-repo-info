## `debian:experimental-20230202`

```console
$ docker pull debian@sha256:aa4da2de818f78a4683c3c042d2dcca11a0dd411e1fee3c3affd3aaedaf2584c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v5

### `debian:experimental-20230202` - linux; arm variant v5

```console
$ docker pull debian@sha256:2c7e662f54edaa34010a489063493b4f6e3e9cfadda6bf794c02cb819f1e0ba7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47996666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcdb27cdd25fa0ba2b9af2fde68f944899becd379c9cd69f2f56f61187881356`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:48:05 GMT
ADD file:534c27eb76f803f42e515e864256cd12d48c66bf4ca93d3518e9613bbc45868a in / 
# Sat, 04 Feb 2023 02:48:06 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:48:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:efe88ad76b423ab908ebbbc5d07cd3011845d565716e73634fcbd0028219ae6e`  
		Last Modified: Sat, 04 Feb 2023 02:54:13 GMT  
		Size: 48.0 MB (47996445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824990dafb7317e617f7cc2aef25fe33a06cdda045d2af1b10c0ae124cd0fa9b`  
		Last Modified: Sat, 04 Feb 2023 02:54:40 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
