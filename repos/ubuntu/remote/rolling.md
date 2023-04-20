## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:a8dfb3445fcaf180259bd36e49037f0b579cfb09950d983d3e45e729de8022df
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:2f18a21d414ad3c0a8eea08fec8f98d730c5c02ddb0d5fef9c60ca72ac53329c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26825187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8c92df8590c370b0dcf10c9273b5c18a74e08fb6089ae37d4ad9590fbdecc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 15 Apr 2023 04:51:04 GMT
ARG RELEASE
# Sat, 15 Apr 2023 04:51:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 15 Apr 2023 04:51:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 15 Apr 2023 04:51:04 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 15 Apr 2023 04:51:05 GMT
ADD file:0974d2aeef46c39070cbf74e10bf8644b9753060809b3c7100126a1bcb448f12 in / 
# Sat, 15 Apr 2023 04:51:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cdca6f9f82cb2f31168afd36307721605cb5f89b51b97fa630583843ddb624a4`  
		Last Modified: Sat, 15 Apr 2023 05:20:43 GMT  
		Size: 26.8 MB (26825187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9afa28d1eb80d78129debbef52b3f2a59b19479b2c15f01d16c2beeccd72dc10
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3781448a65e540dff394a6ae765d032b6c5fee3e0bc008f323330bd44a5aa797`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:51 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:52 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:10:01 GMT
ADD file:7c943de57b75e515f072a13706b12ee97f17d22a120991f8effbc0615c544253 in / 
# Thu, 13 Apr 2023 13:10:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:049083b382db595e625c4760cee04d50fb6110bda597a3dd936406027ce01994`  
		Last Modified: Fri, 14 Apr 2023 11:09:28 GMT  
		Size: 25.1 MB (25067534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:9ff03c2930fce7e915f3b321c6c601380ffb845140bd36715c44ec31d7ae551e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25759013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490b20d4c90f834abcf386620a8906d21821aaa4db91c4665016883f043a10e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:37 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:37 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:20:38 GMT
ADD file:8b5c9a166ff42d52b423d188428558ea2bf225c42aeb3de339514e6ad9fdd504 in / 
# Thu, 13 Apr 2023 13:20:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bb7992c0b6c454d95752fadeb8ec30f02376e386e2dbcde466ab9e74283ed78`  
		Last Modified: Fri, 14 Apr 2023 11:09:21 GMT  
		Size: 25.8 MB (25759013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:56185868328c6dcfff4b9f97915a8868905668fa8ffab0b2b0285dac1dfd84cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31113926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa908635f261aa7b8aa52c329990cdc01c4716fdac960a6f3cfff6706f2b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:21:42 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:21:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:21:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:21:43 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 13 Apr 2023 13:21:45 GMT
ADD file:2f24914c3a2e66342aa7cf589af143b01a1cd7532c92c4263d251fb826b8b810 in / 
# Thu, 13 Apr 2023 13:21:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c6864d2efca45377dbba7535ab73bb2a64f10d73c7d97bfbd768b173970bf455`  
		Last Modified: Fri, 14 Apr 2023 11:09:34 GMT  
		Size: 31.1 MB (31113926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:3af6f4dd8a997017ff74949f2f4e88d672dfa28b5ea06e4093a3e15193bb9391
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25705932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa77ff3a8aeaf751ae3c673bb074b5f67528671ede73189cecded4d61348f7e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 15 Apr 2023 04:52:00 GMT
ARG RELEASE
# Sat, 15 Apr 2023 04:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 15 Apr 2023 04:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 15 Apr 2023 04:52:00 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 15 Apr 2023 04:52:02 GMT
ADD file:fbea81511df0975bdcf894e5be93dc02670d76233449f6221b0a6752e6178646 in / 
# Sat, 15 Apr 2023 04:52:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c6dd1be43160c095f202288009f4efedacf98863e9604b1af368e386488389a6`  
		Last Modified: Sat, 15 Apr 2023 05:21:07 GMT  
		Size: 25.7 MB (25705932 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
