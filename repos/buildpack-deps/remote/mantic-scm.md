## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:a01d66477d1b940517b8ca3778a101cfb0db6fed8a05cec3a639d1af8136ee25
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
$ docker pull buildpack-deps@sha256:c7e495a12a1464b2f7a02eda48b5aaaafe94d24645bb7352d2d86eb107bac600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82732162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e3da1fd7d5dc4e9975002d36007814c5c3077c22612c43346ed3266b6f55ad2`
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
# Sat, 02 Dec 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:760243c1a983844f069a293b501cd9301cbd819c4fb9551cc389ff6e1e7cb238`  
		Last Modified: Sat, 02 Dec 2023 04:30:20 GMT  
		Size: 44.8 MB (44753276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afca6c528e9a02dffda09b471ae45eb3c1cd24ff62f025ec89877622c62fca52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84386409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfd5fac42f464b6ae54e8ee27cba67ca6befadd81810a15993572f7fbd736e1`
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
# Wed, 15 Nov 2023 02:05:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0d43664e3e871d40780214b000e38e04e3e840e99201a63699c325b0f02b0e5c`  
		Last Modified: Wed, 15 Nov 2023 02:12:19 GMT  
		Size: 49.2 MB (49223065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf087be5e86a4c17a523c29b076e9f0fe429f185a1485b4288e664384784dfcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab16779c759dc820ef4e5a74d5ce02ee78fa337b3a8e604f11ef1f752d8f4001`
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
# Wed, 15 Nov 2023 06:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1a3cadc26010e0f011e17572f55422b03f3cc9dd1729864eba62145f0aeacf76`  
		Last Modified: Wed, 15 Nov 2023 06:24:12 GMT  
		Size: 45.0 MB (44982339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8e3dc8db0d9983ef98c6265650ef17b378e2e0fb0dc4df96cd6e6e6e23d2fa73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93456849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975a408a5e5596adcff48d38f73cf3ecffd1da203fe40d0444a14a5270af9278`
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
# Sat, 02 Dec 2023 04:41:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c8c14fb2f649d6e1f2a6ecdb5517e059449e766f72791aa8c47aa868b20d52f1`  
		Last Modified: Sat, 02 Dec 2023 04:51:47 GMT  
		Size: 49.5 MB (49544508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a91a88d92cebe1e06032a2e91eca9eed7764f96574bf8209a0e634b723902068
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82887049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f810d9541dc377d4af2da31b65e5188e4419926498729a02895e8664cdb624`
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
# Wed, 15 Nov 2023 05:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:692f488bb8b766464b4e25f6f72ccf92efc432f0c10df1d1003061838b729d85`  
		Last Modified: Wed, 15 Nov 2023 05:30:09 GMT  
		Size: 45.6 MB (45572317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
