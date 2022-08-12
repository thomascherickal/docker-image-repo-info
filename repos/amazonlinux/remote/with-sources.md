## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:fd9b4eb6bf0f5ce0b9074867ebef131505ce4f4735e493f121aeebe8e1051067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:112e2657cefe343bb8d09ff30a6f4feec6eaf5c0813cb38c895fa3c43e402c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.3 MB (486338250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:255bdecc3d95276f497d739d3a60969d8f7802a30152ab824f3aef4116382d94`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 00:20:41 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-c49e40d8cbba1157c747e1483c3371ef9e59567ec7d1e3cc5f21cde9df7b4f9d.tar.gz"     && echo "66afed6d6747b523bcb2d9acb55c562107bdc4c5a06b822bd5c2c7775772824b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39a5207cea55497b8a954978bb7ea93401d4a5ad0f19d2629d2d0773b38c376`  
		Last Modified: Fri, 12 Aug 2022 00:21:51 GMT  
		Size: 424.0 MB (424022034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:89254f2eecdad7f0fa019a718f913a194297fd0b455df4b2783bb512bef3ac32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487949918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aa933c5f77a29a0d263eb46994456ea32cff3c47ec93f82be70ed043212f888`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:39:26 GMT
ADD file:3ec97c6bec2a8682b0b4088021da97853effeb7dfafb69329cfcb5686c3dee30 in / 
# Fri, 12 Aug 2022 00:39:28 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 00:39:51 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-c49e40d8cbba1157c747e1483c3371ef9e59567ec7d1e3cc5f21cde9df7b4f9d.tar.gz"     && echo "66afed6d6747b523bcb2d9acb55c562107bdc4c5a06b822bd5c2c7775772824b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9f9c648afd7976bdc42d03595d6a1c1c502c47f18abb3f42a9a20b38e7d6e161`  
		Last Modified: Mon, 01 Aug 2022 22:09:01 GMT  
		Size: 63.9 MB (63927916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d1f88192a4287bbbeeb2fd730a6ae32120d881986dfc6898b18084e3c4bb94`  
		Last Modified: Fri, 12 Aug 2022 00:41:18 GMT  
		Size: 424.0 MB (424022002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
