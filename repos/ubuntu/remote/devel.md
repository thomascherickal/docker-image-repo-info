## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:3c38c7f067cc8103c300b3ed089a0b916ad5c9852f402a95c6fb8a8cf4b69b23
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:7e44d7ed904145328785378ddac5de49ac931d3b28b72f6c9f5fb350f9b4a849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27277147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8801a7ecb54952ea17852be887c1d858fd7bd78dcee093afc11fee7ed53f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97e98d3adb77a3f73850e0a81cdde417afce9cd9dce78c444f99b9258caee9fa`  
		Last Modified: Tue, 26 Sep 2023 05:33:55 GMT  
		Size: 27.3 MB (27277147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d7e166e923d882bda98249bf852065c7cf27069ff5c5aeb5b8535f0e529c614f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25248894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7b28a5258684f51bbf3c6bc2fb3215a3965391e08182a8ce25c4ad40d87b50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b88dfd009c781b3ca94bb2f78164c028587fdbf1d6c56f41f12b7d8eb03bd975`  
		Last Modified: Tue, 12 Sep 2023 05:02:36 GMT  
		Size: 25.2 MB (25248894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:bb9a61edbd6cd4f0b8458daa9a78bc09ff7ffe638e7da0a85dc28a5b6c26adb2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26356283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461b48f7d9e026c91692982d4ad80e66be3245f28c14eebf5e1c2fd88c95bbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:afcf80ae17bcd3e5b46853b0fd5d9358fc62ae2b878d7ccb081bd357330cd0aa`  
		Last Modified: Tue, 26 Sep 2023 05:34:02 GMT  
		Size: 26.4 MB (26356283 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b8cd2a5eae36321f5747cc2df64abbaa05e1c14c770fc744d6774067fa89a998
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31370401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de077450c3dc8887a07aff9caf353b1d070608a3f884085cddd389662992462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b3c414ea1cf4bfd1e808fd228f0b9096a8def2e1f9df113dcfa135d2422b27b`  
		Last Modified: Tue, 12 Sep 2023 05:02:43 GMT  
		Size: 31.4 MB (31370401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:f6ba7caa089441d7433604f4371a79fec8d58950cda10bd6d29be8ed899fa3ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26908064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7ded0e47b6d77072838e6f9f2b41db1bdf20834e54d02cb325c1880a43cf89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2fc3f13b6a87a63eead8aeff863bc67a0870656493725efa7e3cb1cd945c9134`  
		Last Modified: Tue, 12 Sep 2023 05:02:49 GMT  
		Size: 26.9 MB (26908064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
