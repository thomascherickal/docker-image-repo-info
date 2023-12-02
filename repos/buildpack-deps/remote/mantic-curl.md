## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:f4b5aa0f522b4e72b713513e415e0fbe24227308244666233415f8887d7bf3a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c6f602b7643df9f295b45b95bfb4be8dfa85b98b94dd4e280809748a07d3dc36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37978886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c449b2867d49805ee4b096b0a3444aafcb711d7e3543e906c551acfb15076`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:21:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cb8122a41e708f03d563c8ba7400f85d27af325fae5fbf4e00380a11f4ca1fa9`  
		Last Modified: Sat, 02 Dec 2023 02:22:28 GMT  
		Size: 28.1 MB (28070890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3950b4737b0d86b7d5a2758a2148e06120a5a73d9f1593fe22ad1a7c8e83a83`  
		Last Modified: Sat, 02 Dec 2023 04:30:04 GMT  
		Size: 9.9 MB (9907996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2913f2f84d97ff1be7ca139b43ce4e8d05cfaf7ed3248b39aa9e6a70b154ea91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35163344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cd33ac4877ec60e73bfb24bb572ad8088801b2acdcc70314770203d15b6c91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d649d5fa7ae482f135330be776368c49ff5d30b7336734c39ad94af9a6064874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36985512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ce70cb7143b41128b73de1bc7c1520314ceae722ab6e435381a4fd31188a78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:04a3cc193a0eceb4125d729128dd4d0f0bb1b8a47085e1e23edf8f7d56da9b0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43912341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8991fd5c6982603f7891b53566d2c7e1439126fa3cdf93b211adbff3f17bc315`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:40:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e6a2519a5ea0f832b2e35477f84cb47f263c19385218548bfd1ef20a7b0ef71`  
		Last Modified: Sat, 02 Dec 2023 04:51:30 GMT  
		Size: 32.3 MB (32337524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78920d0cdc2c45a2f364052f0f3ae1ca5ad03f12e0ca0ede2059df652d0396b`  
		Last Modified: Sat, 02 Dec 2023 04:51:26 GMT  
		Size: 11.6 MB (11574817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e3fb9abd82bd63f435954245545251574327c9881255d2db0ca53940bda40d64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37314732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64946e8ba5952759944b3513696715ee3fc336e4cb5f02dced4113a84b7fb861`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
