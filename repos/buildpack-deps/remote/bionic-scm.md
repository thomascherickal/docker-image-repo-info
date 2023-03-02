## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:bdbeb92cdb417dfefa084dc354ebb292bc3d80354b576d57918b117d81af1984
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
$ docker pull buildpack-deps@sha256:bc9e9bbd14e8a837e30009807718c317555b3585704c270ca0544ef30f322d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81867757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd2ec34b02293026aee8b871a2ae86c29c797aa05892297f3a307185c275e28c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:22:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f631ab33a755e153343352043423161c6232b94c3be5472cd780d6fb66fea8c`  
		Last Modified: Thu, 02 Mar 2023 03:42:24 GMT  
		Size: 45.5 MB (45513091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c945aafe1fad15d38e1188cc1844f06e144bab7335c3db05f2caa56f3ca460ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71282811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca2769a55b83b9eb31be2f63bed94363f1630e19ee1d39e592aad1851a18bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672070d854b2efbf7e9d5720a994ded06c4e58c97060013aed2981fd327517c`  
		Last Modified: Thu, 02 Mar 2023 11:54:45 GMT  
		Size: 40.7 MB (40712962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc66d659df3c4d980bfd741e281c52d81cfab1027cdb9d0449f4d054806fdf77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75891803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4349a1a66435e325994ec9e6ec99ad5776cd7ea349f06b3e79c091f197bda134`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491410c5ebb78636109cdab447342140dc9a4facbc978baa236f142ea8e9d64c`  
		Last Modified: Thu, 02 Mar 2023 02:35:57 GMT  
		Size: 43.3 MB (43312084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f8c35b10a7e33961c8ce0a4bb0387e1bb73fa5a4677e5d36f56be2dfd6ea1b7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84425697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc4a367ff17e24b264b6562eee2668fcff45fcd418f80cd1e43989d1f259f5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 14:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd34df470431bd99fe8348a0b7488317fd90179a50fc094b1bc09cfdfff0f651`  
		Last Modified: Thu, 02 Mar 2023 14:33:08 GMT  
		Size: 47.1 MB (47097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:61f125647b51960eaaa1628df14c40ad5596f9a0c8ca31b75db9663c5ff8007f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94957007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae7f36d16db90652afad8c37a9ea6b419e7b1ad7a94291093ec62e326ab0e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68956dba4cc03b50dc85a017a1231e5796aa790462edfefff2e29d810938fac5`  
		Last Modified: Thu, 02 Mar 2023 03:54:58 GMT  
		Size: 53.7 MB (53737565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:54ddd0cd0622a5cd6cf1b28c3cb01a126d011f4d8e4c29ce1903761bfc7da58d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79698067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:206911be72a3fb03d2417b774c512074beef855e16b0cd2235cf6e178d1a1736`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95174d0c3f8fa7400f2fe1baa0a15756c66695199991cb0126f6cd6586899`  
		Last Modified: Thu, 02 Mar 2023 02:21:45 GMT  
		Size: 45.0 MB (45039451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
