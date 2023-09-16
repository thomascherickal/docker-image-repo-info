## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:ee3af8d7c81aeabaf31589a31efddb2b45e17b92bd0493b019b29f391ac93bfa
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
$ docker pull buildpack-deps@sha256:1bb630df22e33291642f68a48e92df5c11f6fcc8addc857c65c5af3d56781944
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86739196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6570c5059e2f4f42a0e476bc6d23ed3ba68c4aea4460b81cd43807e5e9f904b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:44:28 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:44:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:44:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:44:28 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:44:30 GMT
ADD file:3eab7cbcee278ce63f29f9808cb781d2eb15c0ab34d32a3a96af0299bd7f8f57 in / 
# Tue, 12 Sep 2023 04:44:30 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:19:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:19:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de5bd8f63131b365a8b75ce84fcce99e78eb1a16bace032fb6b3436580aa3be5`  
		Last Modified: Sat, 16 Sep 2023 02:23:58 GMT  
		Size: 28.1 MB (28086986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d50b023cfbb59919320bc1707382e1cc5a96e00f043ae469ddbfe2aaab4c8b5`  
		Last Modified: Sat, 16 Sep 2023 02:23:58 GMT  
		Size: 13.9 MB (13886113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9dcf24a5c0ec80290ed7d9375e305d49cb984a6209470d032dd7876091e93a`  
		Last Modified: Sat, 16 Sep 2023 02:24:14 GMT  
		Size: 44.8 MB (44766097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dfd672a620a588d03e3ef7e561eadbff81d8dbdbde7ab92714fb5d4a069e16f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87729696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456109293a891e13861b3e830e4e55a1cb417dddf91fe4daf3ebc772b29a325e`
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
# Sat, 16 Sep 2023 02:43:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:44:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:901b7210b5b59d80ecd06f3107fe68dbe84f1a47ffd468aa90dd8894057f62b7`  
		Last Modified: Sat, 16 Sep 2023 02:49:15 GMT  
		Size: 26.1 MB (26068467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3b650c0e7bb6739dbe1082f6637079b42eebc467b66032c563599bf955dffe`  
		Last Modified: Sat, 16 Sep 2023 02:49:14 GMT  
		Size: 12.7 MB (12712685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908b46c2007ad413fc72abfff7e075713078a4875b6d49c60bc3f10db0f1111d`  
		Last Modified: Sat, 16 Sep 2023 02:49:32 GMT  
		Size: 48.9 MB (48948544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ba870c6142c667492230556ac92598b4d76a2a87fba834d4db2916a517ba8bd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85359835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d779c8f23b725d69c505388f02b61a6cb54653b6c3e4e2345ddeda9eb6978a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:46:07 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:46:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:46:15 GMT
ADD file:e7975e06b9483ac7786a825720e46167975054bca8b0679a3c001d143c325fbc in / 
# Tue, 12 Sep 2023 04:46:16 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:08:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:09:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8e30ad94028d16a73ba211f5c6c54cc5246b12575575b6c44c6c55b6f331994`  
		Last Modified: Sat, 16 Sep 2023 02:13:44 GMT  
		Size: 27.3 MB (27318189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb011cee5097836afefa9b1443d4ca56b7a28b4181bbba91dbe5f98c84c81a49`  
		Last Modified: Sat, 16 Sep 2023 02:13:43 GMT  
		Size: 13.4 MB (13393412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ce9808c41502adb5c86180f08ac4e060e6cbc9e4c1c827ee7806a31f97b48f`  
		Last Modified: Sat, 16 Sep 2023 02:14:00 GMT  
		Size: 44.6 MB (44648234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:977c79d6b8f01f194b957f7275c4f50d1d671a66c30b44e19a8143013fbf1f94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97862194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff61b5ba517d57e7d5be3582786fc0eab77fff67a3c96b95be77cdead8c4da41`
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
# Sat, 16 Sep 2023 02:42:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd229c9aa7cae185d030f835d891646d81b863cdb9cb773e41f12ee940228d28`  
		Last Modified: Sat, 16 Sep 2023 02:50:16 GMT  
		Size: 32.4 MB (32367087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec9bbd29feb8adb47adfbfa6309c9d863f2e8ec5f80cf30563f27da97167973`  
		Last Modified: Sat, 16 Sep 2023 02:50:12 GMT  
		Size: 15.9 MB (15938863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f18bc37fc98bef3457686b1b305b6bc6178654b8998f68ee0fa0dcafcf065`  
		Last Modified: Sat, 16 Sep 2023 02:50:39 GMT  
		Size: 49.6 MB (49556244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0455529e5225c85cd91293b3e29caf5def9ac392c642de5efd807518abdda497
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86723954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d4c8d1fd98e9d1a0e24c2af3a3dc2a7cd9cd32a8535ade59e4011c131a0232`
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
# Sat, 16 Sep 2023 01:50:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 01:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac93ca815ee057f1083e81c9edcf7787c1047a557a07ded971abbb05fa515ca0`  
		Last Modified: Sat, 16 Sep 2023 01:55:18 GMT  
		Size: 27.5 MB (27458487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939194dd385d3eacfbb7f1bf5b9dcc18c16873f21f0cd06b02cceb11343c00ed`  
		Last Modified: Sat, 16 Sep 2023 01:55:16 GMT  
		Size: 14.3 MB (14252767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8e1239553e1d4214fc014d8343ebf58fdaec6f3d8c02336f867a7364d774ff`  
		Last Modified: Sat, 16 Sep 2023 01:55:31 GMT  
		Size: 45.0 MB (45012700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
