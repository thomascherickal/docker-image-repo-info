## `debian:buster-backports`

```console
$ docker pull debian@sha256:e52504eca8fe7ca760544ebd0b7abc0530f555334293d8e0b6a2ec22a8826bb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:5cee24386e991d71612ab6603b2aff208c27307120244f056144a829e75e1c95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772a8bf029bb6c561bca9f7fb1b0946ea1bcd183340c2045e1dd1c91c02a5643`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:20:39 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73104bcafd56465a15bf1dc7a6ee33d7f91692b9f20f0dd8a535d1d85d480d37`  
		Last Modified: Tue, 04 Jul 2023 01:26:13 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:5b5a775a224016909354d484cdfd5367605b51e79bf2a136efd22916ab868ee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fb2b4ea95237b03a7b71ba22054a5d39756dc5eb23ce1ac5b5a9f75763047c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:58:34 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d7a9a6f5f8af9bc7b70d526883758c669829e4729676cb679627d37198c4a8`  
		Last Modified: Tue, 04 Jul 2023 01:04:09 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a5a9c4833de0112ae2ce5c6414e7fb35cd6621a15c658a97e1b20de0efaa98ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49238628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9e7ab0562b5a1b39a35db005720d8c17775f80d5c6217e6cd55c96bce29294`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:41 GMT
ADD file:bb3cb9e6abc423742d7c1b6bc006a7cef70038c5621c71a90a2ae7c1ea29ec63 in / 
# Mon, 12 Jun 2023 23:40:42 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:40:45 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e8371d57f7426517aead21bff5af0cf321625cac166c86214c439fb67db84243`  
		Last Modified: Mon, 12 Jun 2023 23:45:01 GMT  
		Size: 49.2 MB (49238409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5cec9dcb24a633e7e56aa1b73177a1ca694b011e0aefed457fd5b0061df0ea`  
		Last Modified: Mon, 12 Jun 2023 23:45:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:4705dd99f61ad3bb0d155376d6eaae60d58e62e5f9d33d983d3a171c008338eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b900c0e5e1a3c1d73dc0aba90988b428f23ec8700ef489e4bcfafdce24c043`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:16 GMT
ADD file:c4d7ce8374a492278fd0b54ca10fd35f995676380e4ef134e484fd85ed50c58b in / 
# Mon, 12 Jun 2023 23:40:17 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:40:22 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:121d519ab26049cf059ad8c480f995a2bb103d39a5b57857d7ac27ab2b0d35f0`  
		Last Modified: Mon, 12 Jun 2023 23:47:27 GMT  
		Size: 51.2 MB (51205988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e700f289ea17a660e80ccf6be3d01dbd39d4e569aec2a742a5f60a04e62133`  
		Last Modified: Mon, 12 Jun 2023 23:47:39 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
