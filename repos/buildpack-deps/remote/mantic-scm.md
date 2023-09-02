## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:8bd9b844b36d323148302f979e86c412217a6cdb2678f09e085089c3dc584b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f1758069423c18f1d2a53b15b07d176b308d0f9638ab8a341d5b3664d03f1dad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.1 MB (94121578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c54b8c1116b61354aa3da83ee578fb5023abc99f8611bb09e421976e8abff0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Aug 2023 05:04:54 GMT
ARG RELEASE
# Sat, 19 Aug 2023 05:04:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 19 Aug 2023 05:04:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 19 Aug 2023 05:04:54 GMT
LABEL org.opencontainers.image.version=23.10
# Sat, 19 Aug 2023 05:04:55 GMT
ADD file:87bbd4b1a17b5a9990befc7d85a50c9b813d3cea95c9f28e0001a40d6b7deaf4 in / 
# Sat, 19 Aug 2023 05:04:56 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:07:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:08:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:717fa18fb0fc884d9a94c702c32647885b210c59e1fa77ea32995b51deb76537`  
		Last Modified: Sat, 02 Sep 2023 00:07:33 GMT  
		Size: 27.9 MB (27898869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84652230bf87528d3bcfe5fe4fef2e3d3e197372d5eb30e3cd0952ca6feea84`  
		Last Modified: Sat, 02 Sep 2023 00:13:47 GMT  
		Size: 20.0 MB (20033729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0466e4a84f6b282e06c9695d238afb6a05f5436661d460a6f4cb395921606`  
		Last Modified: Sat, 02 Sep 2023 00:14:02 GMT  
		Size: 46.2 MB (46188980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:de6e17a83b3432ccde1604364752699b4eadb721fbc77b3dd5caf056e92c934c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93301258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa927f0daef47031ac1092ed6424ee9df4131e09a94a53123f76fc9281f5e5f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Aug 2023 05:05:42 GMT
ARG RELEASE
# Sat, 19 Aug 2023 05:05:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 19 Aug 2023 05:05:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 19 Aug 2023 05:05:43 GMT
LABEL org.opencontainers.image.version=23.10
# Sat, 19 Aug 2023 05:05:47 GMT
ADD file:b2556a8208f666e3c07a759d0acbc23841ac60abc72026ca23e8a2d2c96a3c9e in / 
# Sat, 19 Aug 2023 05:05:47 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b202a4ddab8fff273b81c7544dcb792ca7858b4cd7cdcd12e551f3d5382b8f10`  
		Last Modified: Fri, 01 Sep 2023 23:56:33 GMT  
		Size: 25.5 MB (25452732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ec094154d11eaf24d03d379c6aab843118a05535d0377edf88e33135e4cbb`  
		Last Modified: Fri, 01 Sep 2023 23:56:31 GMT  
		Size: 17.6 MB (17596155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75352c292c46da0ffb27109cc56e769c3433ba90f9f5aa092cbdaeddfca30c5f`  
		Last Modified: Fri, 01 Sep 2023 23:56:48 GMT  
		Size: 50.3 MB (50252371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5b632bd358f1b045135d156f53cf7349e7b3311400d67e0f3fcfa8b68d91055
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92440850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031ab4026ed45e324f841017f051a000f86ada7aa43e8cf3a52cc51b0db118c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Aug 2023 05:09:54 GMT
ARG RELEASE
# Sat, 19 Aug 2023 05:09:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 19 Aug 2023 05:09:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 19 Aug 2023 05:09:55 GMT
LABEL org.opencontainers.image.version=23.10
# Sat, 19 Aug 2023 05:10:02 GMT
ADD file:cc6a3e0225d3c4171348881d7482651292156aeaaee88bc0ed81e8a850fe21f7 in / 
# Sat, 19 Aug 2023 05:10:03 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:21:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:22:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7ad6503180330babb207079119820c257dd6aa2275b3a0e8e507fa5535e83de`  
		Last Modified: Fri, 01 Sep 2023 23:27:40 GMT  
		Size: 27.3 MB (27264110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58883c3667ca078a9f47c68653ab34ee1d76f9c3bf1869cfa801b1bbd1f8af16`  
		Last Modified: Fri, 01 Sep 2023 23:27:39 GMT  
		Size: 19.2 MB (19228183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff4bfaffc5bb4a3e10976d79e4dfe9200424f4be3b30fbc6c6beaf5fbbac5b6`  
		Last Modified: Fri, 01 Sep 2023 23:27:53 GMT  
		Size: 45.9 MB (45948557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd0eae220e0953f1e8f6db015f3819e7a0a745b01bb1d8e0c6cc7cc06b878fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97670522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6f57f844a17257f7bc458e8bd3b32b7ee6f2093e6627869cf392d633985d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:39083b5f214b26a57f519ddd9ca7859afa21ca88ccd8920d5bc8e7633d3082be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92860751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7af2798866d99ecca5f843d9237a5aa7e1234de8473978a38d9859aea6544b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 19 Aug 2023 05:07:37 GMT
ARG RELEASE
# Sat, 19 Aug 2023 05:07:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 19 Aug 2023 05:07:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 19 Aug 2023 05:07:37 GMT
LABEL org.opencontainers.image.version=23.10
# Sat, 19 Aug 2023 05:07:39 GMT
ADD file:681bda53818a2c0f492a5b6c8f35eb4ecba1d81c3c51e02310824c03db9146e6 in / 
# Sat, 19 Aug 2023 05:07:39 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:19:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:20:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b09de31f2a7e0477e15ccd77e26be0df5df0f755bea2d6bb52236401d3e3684a`  
		Last Modified: Fri, 01 Sep 2023 23:24:59 GMT  
		Size: 26.9 MB (26936780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d5be6eaee2b4edf324dac730d3dc0afca32176b2dd3c65d0705af55ab42a00`  
		Last Modified: Fri, 01 Sep 2023 23:24:57 GMT  
		Size: 19.5 MB (19502292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17bacc9d32f9c9fbbe2742619bbdc5319125f09d50a550996f882259886d577`  
		Last Modified: Fri, 01 Sep 2023 23:25:15 GMT  
		Size: 46.4 MB (46421679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
