## `debian:experimental-20230202`

```console
$ docker pull debian@sha256:e8aa5a5d4ef0c5912bdca1e9c7790a3fda99417e2435f8fe6b7b9382ba1dc4e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v5
	-	linux; s390x

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

### `debian:experimental-20230202` - linux; s390x

```console
$ docker pull debian@sha256:673f31991acef53cb58cec67247598b2392949c76a5b4d74f0899a112b59b634
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47408318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7802975822b68f2f940c7a2cbdb77efbfc6932683a63da0f03933069298cdf76`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:07:49 GMT
ADD file:3c9acfbe477ef9b7cf73ae31792916ba05d27b89c732e71d0daaff74ddeb122f in / 
# Sat, 04 Feb 2023 04:07:52 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:08:10 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:62f7571fa4c40757b40308fc2a271dea2516970f00b23711f52075edd81b8b5e`  
		Last Modified: Sat, 04 Feb 2023 04:11:55 GMT  
		Size: 47.4 MB (47408096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fe70fdcbd94cc004489e579a756862719cd7f0250c9f655ee35d6322365c68`  
		Last Modified: Sat, 04 Feb 2023 04:12:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
