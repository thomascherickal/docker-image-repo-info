## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:529ff9bffd4ef3c00c72a669a88acb71ef9b1d795b91801400022a5d8ef53b74
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
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:832381cafc44879857f084dd780d246e2afc077bb9f97cc76d02665b50a7b51b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25244973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e05e891c9b4d59dea3e056be161095328b7b723250ac89b69e4178a45e894ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:956aaffe9fe2861fc716bca41f30a50ff2eb645844bc74edb8b90428a5ef3637`  
		Last Modified: Tue, 26 Sep 2023 05:34:08 GMT  
		Size: 25.2 MB (25244973 bytes)  
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
$ docker pull ubuntu@sha256:7507a6b5347931e91ccbf64eccb1d47d9b1a3c8c731b370efd21fbc28c08bfb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de3a97de9876c2336ea46851c0df7a2d9ad45c60022dfbff95d5d6e75ccefca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 10:59:52 GMT
ARG RELEASE
# Mon, 27 Nov 2023 10:59:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 10:59:53 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 10:59:55 GMT
ADD file:63fd35cafc829797c017809779c1ff420497005f85c88df5d033722104683537 in / 
# Mon, 27 Nov 2023 10:59:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5bb3f3c327d75c33efbc824eb228df818cdf339da3fdd25997cbb0e8e84093ba`  
		Last Modified: Mon, 27 Nov 2023 11:16:00 GMT  
		Size: 31.3 MB (31316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:a353c527eb5233fdfc2ad112c7897cce7da6ac28b24d3aaa8f441f27ddf613c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27072390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12eca28f81d0bd51084742dc133e32c215a83739fc5603306f1ad774311dc6ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:56312385d597227d0c1232049609586ed3412b04e6ec96c5f6626f5f50f438fe`  
		Last Modified: Tue, 26 Sep 2023 05:34:22 GMT  
		Size: 27.1 MB (27072390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
