## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:2c7212348d43e19ae7628be0866adfcf9099b6f98ff7134b5c4efcd9bbe802e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:543dc97b8e4e7901f3e696c1c9f030a0d5b5210fd2b09f190e2f2f17a5934c7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81754441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b5f07579ffa9423839e89638dbbd9f7313652c2afd51ea2b39c9661471ecb9a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:18:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba419f165af9059de838373e4a92f32ac4204c46ab0a25eaf0458a054a903130`  
		Last Modified: Tue, 02 May 2023 23:41:48 GMT  
		Size: 9.3 MB (9341953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec1066fb8995b9d44c4b3619ba985360d37dc4e3790190a5d31f1e16e0fb8a5`  
		Last Modified: Tue, 02 May 2023 23:42:02 GMT  
		Size: 45.7 MB (45701742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a0c6116f0b68c17b056b86c0dd94218202059e39f75a61faefeb12c35f01450e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71294805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5346d93c8e011840332f5470a553027ec93554ebbbf8cf84e4374ac76f078db4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:08:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969f7b91ca161e7f81edfde2caef7769678607f2eda9a368b88473a11873611d`  
		Last Modified: Tue, 02 May 2023 23:39:30 GMT  
		Size: 8.0 MB (7974207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae45f9298f3fa741a5e56033223704de8cb5888e8619414c5f85abdb60ca295d`  
		Last Modified: Tue, 02 May 2023 23:39:48 GMT  
		Size: 41.0 MB (41015224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:73a5d25262672e1381ad7e9bdf000137e42890fedf61a45876fe6bcacbd53a1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75771606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b946904afc73df09dad52fefa6c323e60c518b5eb4dead2efd847ed9ba50dc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:46:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:47:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b6ac8aa0ef17a4ecc09729de5294c6904aee755dcceaee749aca7b0911111`  
		Last Modified: Wed, 03 May 2023 00:13:55 GMT  
		Size: 8.5 MB (8544155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb20e651edd78cfdb6e4f13581c87e6171457e101f71d1b52ac4013202fb4ad8`  
		Last Modified: Wed, 03 May 2023 00:14:08 GMT  
		Size: 43.5 MB (43492745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a2fec2d10fdfbac0140a3630df399c38b947dccb95c259f6499972195a8d27b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84286242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e846e68fa824a02a8239d98b51fad28b0edb5ff0044649f408e0fdc73e92a74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:49:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:50:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ecd335a38ed53ee57177d2474a0e898531d4f60dc6978a8df04beae83f717d`  
		Last Modified: Tue, 02 May 2023 23:58:47 GMT  
		Size: 9.9 MB (9866067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b212c4aa811dee28092711fbd302ab141e4c34f923af8a513b32235a11b85`  
		Last Modified: Tue, 02 May 2023 23:59:06 GMT  
		Size: 47.3 MB (47255565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b7141721c1c36aeb08c52212453e0b366df30dca1d192fd1a6b820fc40567392
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94845665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9534ee764dbf3fb8374598c73c71754d969f8b59304886e3a1b922f695d1f00`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:21 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:21 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:23 GMT
ADD file:362fa5164fb227e6f3d45a41742ca485fc50dde3cfdc3fdc1f9233011d3d1b84 in / 
# Fri, 12 May 2023 09:26:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 00:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 00:57:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab08883ad6ed65686edc81fb213d333beda55de0937170bd1f83540ca1d8f68f`  
		Last Modified: Tue, 16 May 2023 00:54:52 GMT  
		Size: 30.4 MB (30443542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8612663af4b782213cbb53b76c256a5a24aee62f19a60124bec464be1c91d4`  
		Last Modified: Tue, 16 May 2023 01:03:01 GMT  
		Size: 10.5 MB (10474415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c2c2f8054a6c2a3e88e6346c543ad5671c2424fd30cfc62c5a20f5807a3aca`  
		Last Modified: Tue, 16 May 2023 01:03:25 GMT  
		Size: 53.9 MB (53927708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e0f143746ec08a3de83bfd4cc45127f60cde71c3a0c351dc9073853776906afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.6 MB (79611765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f48d35492d41f963807ea390ed16c15e2d0a999b60e12b13c3fbde16b58c6e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:12 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:13 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:14 GMT
ADD file:8abaf7bef475e944e369ee2369d14001ea58594579438de5aa0e2fa72e805c72 in / 
# Fri, 12 May 2023 09:26:14 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:11:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5490589b1a9dd4773f02a935037b1960843ae0c35ff2284a0209a8d6d948a95`  
		Last Modified: Tue, 16 May 2023 01:16:19 GMT  
		Size: 25.4 MB (25372959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bac593a1156dc49dae6ac86a45fc34982b24751af006b77e6876a5c04fdd713`  
		Last Modified: Tue, 16 May 2023 01:16:17 GMT  
		Size: 9.0 MB (8982576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e6787d7045a27db04a439e0e0dc9497702567502669dfe4452c953601bd6f8`  
		Last Modified: Tue, 16 May 2023 01:16:33 GMT  
		Size: 45.3 MB (45256230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
