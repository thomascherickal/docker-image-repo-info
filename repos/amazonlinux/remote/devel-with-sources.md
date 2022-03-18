## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:182ddd498eb7659524a3a6b2d1f4a90d49270c8bdf877d5e9466163072ac70e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9d70c6acb55094f295cb8b5a825f196fdf6e21ccb871820c521f7b451cc85279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **475.0 MB (475044841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c50a5ed22d2d8eacb5b113a93756909e390d9b515b4c812f7654bdec1aac97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 08 Feb 2022 19:19:55 GMT
ADD file:a17c7e0c1674512d1358af2a8ecd7d3ab42c3f853ca0d502a0a5ccf61e7cc1ae in / 
# Tue, 08 Feb 2022 19:19:56 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:59 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-cc7e5469c58d5d340a4834dfcb1b4f5cd38df8115a8622b945b52156d73005e2.tar.gz"  && echo "356327ddb540b40c52a2a4a6392991c4fb8a6b15c8f6a0bca616a7751d776175  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7bc2af7bb0f9d7bc2dd4e52e139b26d5ec36138f2349163c565b89eb4c5dcc6f`  
		Last Modified: Tue, 08 Feb 2022 19:20:49 GMT  
		Size: 67.4 MB (67393012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec3e1a9e03dfb694ffaf58eda23ce244264e78f40f7876a54a3c178823663a`  
		Last Modified: Fri, 04 Mar 2022 04:20:27 GMT  
		Size: 407.7 MB (407651829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:efa82a440427284fb42c3bb04f8b6883d1d25256b94825dedc674a5dbd4bf666
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **473.7 MB (473701235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:766f7a9f1488c64f9e231d75c17a96d6c7861535370a772aa719bf6f9d439a06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:34 GMT
ADD file:0a3f467739b6b34c1677c74456d43d60dd73758c7cea9f5299bf964ac83a6f07 in / 
# Fri, 18 Mar 2022 00:37:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:58 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-fa0d04ab17f6ae9cb1de39ab5dad52c2e6d9fb369f43679b2f6a0c9e5d12c284.tar.gz"  && echo "35ebd0b74ac0b0422bf72c99f18fd2a38f226202adf6ee9271c52cf2ea7d3df0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8879502b9714388f162c398379c27a6290a8532d379327519640e91d05ac5b15`  
		Last Modified: Fri, 18 Mar 2022 00:39:40 GMT  
		Size: 66.2 MB (66181332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72833236772f911f636d1b918822c9a8ebd9cd41307464819b9beb9a35f16870`  
		Last Modified: Fri, 18 Mar 2022 00:40:21 GMT  
		Size: 407.5 MB (407519903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
