## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:ac001358efc018a0beff4d6cd87798564fb867a283eb1218991494c6d883afd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d5054f5178784f94338b5f22bc7cc57de844585f0d3ba14ff75ce547ac3a052a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77439658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c8bc8abde86925db2e401715cc24df22910342c642169836b5f31a591c6a6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:02 GMT
ADD file:e5fa8bc7f766f2ed38c381684cb1db20880e853d3767fb3c11d7c2c82f166df6 in / 
# Tue, 02 Aug 2022 01:31:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:11:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:12:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90b96841878b7af8ea3a64515404538ce0332b459991609eb863be5db84a3470`  
		Last Modified: Tue, 02 Aug 2022 01:32:34 GMT  
		Size: 27.4 MB (27444732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d0dd055e4367f30e890d117b6f1ffd6db44dd0aed3d102fe5eff81ef9efcb3`  
		Last Modified: Tue, 02 Aug 2022 02:25:19 GMT  
		Size: 6.8 MB (6788538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7b9cc450b3fe5f68921cb876bdc2ae34b4e682ac83c2ef0a9afc63500440f1`  
		Last Modified: Tue, 02 Aug 2022 02:25:18 GMT  
		Size: 3.6 MB (3567036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7703e4480955109a8ea62f400efc32febfe290fbb8f49fbc67f6a13a7a5997c`  
		Last Modified: Tue, 02 Aug 2022 02:25:36 GMT  
		Size: 39.6 MB (39639352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:17ea7c014dd54e74001c3bab896535c87693a7b5d58631791976e68aac09700f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76826806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f02ca7f634f87e5e06535223f07ac0c2c6910afe91f8a62dd87f0479dfb515dd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:08 GMT
ADD file:66e6471f52fc58fc2800d34f1d39716910c1cda3611b70b14120742c855b63ad in / 
# Tue, 02 Aug 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:01:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:01:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f8bc5dc03fab2ee54b70f6218aaaa0c6cd0f00b7df0e688df71d48899d1633c`  
		Last Modified: Tue, 02 Aug 2022 01:43:57 GMT  
		Size: 24.8 MB (24813035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0730d1b5a4dded6f7fae7ef8804e621785ca732706a3a9cfcd18833cf802fad`  
		Last Modified: Tue, 02 Aug 2022 02:17:55 GMT  
		Size: 6.0 MB (5975718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783bb70087bc78639e7d81451739990ad377e2a52f9f4dbd7ff7beca3a622906`  
		Last Modified: Tue, 02 Aug 2022 02:17:54 GMT  
		Size: 3.7 MB (3723518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e95b071738cb28d6e405084a8d7254a484c5232753c807cdea74a44d7f29b5`  
		Last Modified: Tue, 02 Aug 2022 02:18:19 GMT  
		Size: 42.3 MB (42314535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:79e271176c69a7660b26625a1c7bd384530ac8f31d3d77a6d19a699070296c93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75151022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4b7a3c5a62b68fe2a98e6e089fe565441eaead208f4f4f348ddcb234ca48c46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:08 GMT
ADD file:9a13d2dd4ecc4e3136c25a7b16372d77ee8ccfb9b3fcafd78af5797485ffb038 in / 
# Tue, 02 Aug 2022 01:19:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:38:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:39:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229a80be8f0f33867b5a29c230954f11922f0e641aff2a6c16048c533bf5290`  
		Last Modified: Tue, 02 Aug 2022 01:21:12 GMT  
		Size: 25.6 MB (25575171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa5256bba7c1c373d0a1ef1a0465e7994cf5726371518dc47bc17dde7bc45b`  
		Last Modified: Tue, 02 Aug 2022 01:51:54 GMT  
		Size: 6.6 MB (6622247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a514ca1576757eb70513da350b92d860ca64561744d13659787f0224196f53`  
		Last Modified: Tue, 02 Aug 2022 01:51:54 GMT  
		Size: 3.3 MB (3338957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0973ec85a49f90f8cd56e042492c9b81693d2b9c27b1fcb4ad9660d506a262`  
		Last Modified: Tue, 02 Aug 2022 01:52:12 GMT  
		Size: 39.6 MB (39614647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a2f55f66e82d72869c3f073d51fdc5e180ac0511de7a1a0c686b75f49399f03f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.5 MB (88461394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bfa73f289e4e2c662f27ef4465735f26a7aa9b142fe86e7762d538494a189b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:25 GMT
ADD file:e4538e524fdeb5b21a533de6fc3133a1a6831075e4ea42e90ee91a41cb6b4df1 in / 
# Tue, 02 Aug 2022 01:31:27 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:59:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 03:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f94baeb4ad5a685eb35db9740eb61d6eaa8854d3510d8306bb9c21b3064b3a06`  
		Last Modified: Tue, 02 Aug 2022 01:34:33 GMT  
		Size: 32.3 MB (32251435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670badf94496bc55795c1a7c42248ced4988d2b9c6964dc3e626b10befa2e3ce`  
		Last Modified: Tue, 02 Aug 2022 03:24:35 GMT  
		Size: 7.8 MB (7796376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7205d78fcc8ccca412b95e3dc72d73c8372c1f5e59687d4ad6b07d5c7b042815`  
		Last Modified: Tue, 02 Aug 2022 03:24:34 GMT  
		Size: 4.2 MB (4247095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf6317d734eeeae7807889928e91c4046f47b3847455dcd617a302287cdb046`  
		Last Modified: Tue, 02 Aug 2022 03:25:00 GMT  
		Size: 44.2 MB (44166488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c2643ad3484686e2858b69a05bde4fe769ef12f2dd6a79d335138ac394550627
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77714650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a41ee3379488e7bf93c4783e23dcb88e01742cbc94659a4ee81afb8819470ac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:15:07 GMT
ADD file:e538ea349fef49afb4859ff2b8b6fa242b257efe00eed553377d27cc7d1d48cc in / 
# Tue, 02 Aug 2022 01:15:09 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:44:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fd09c311966d9a0a80977ea856824551305831230cbc3c5e3b28d4516c420d2`  
		Last Modified: Tue, 02 Aug 2022 01:33:35 GMT  
		Size: 25.5 MB (25543933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f893a4e0f3e57a74ec7cdbf9a3dcfc88ddabf037e9a8f22cc1aacb8a6ede403`  
		Last Modified: Tue, 02 Aug 2022 03:38:09 GMT  
		Size: 6.0 MB (5956178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd30571558bd98b68a34e44f206af9f8ba2d7868fb5990d6d8715e5fee95cb0`  
		Last Modified: Tue, 02 Aug 2022 03:38:04 GMT  
		Size: 3.8 MB (3783013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1772c66103c431e7f2cbbe09b993f88ca219893a6116ad76f113ac25ba12e6`  
		Last Modified: Tue, 02 Aug 2022 03:40:29 GMT  
		Size: 42.4 MB (42431526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b20a67371a372b668cb40595905f38abc2dc807723de3e9853a1a52e8efe34a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75466502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be381061213e2fc9be0539a24ab5fb7261d5032b933b7a0b8e51fc67a7c59961`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:28 GMT
ADD file:6110741104bb6cdab4d1f236e0e14d83788d0d9be2c117cc21b818cbe53bb7c1 in / 
# Tue, 02 Aug 2022 01:02:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91b26e5129898f349569cdb5e70f8a6e3046baf255fc1b62684edbcb5f7f47bf`  
		Last Modified: Tue, 02 Aug 2022 01:04:08 GMT  
		Size: 25.9 MB (25944242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afb051b7b1df235b2c41c69ce633d0f3026bc2d13a7ecb55d0cb483443d931`  
		Last Modified: Tue, 02 Aug 2022 01:40:23 GMT  
		Size: 6.5 MB (6476893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5e4c7745db385f92256fe54757ac7d96ef0485584e1ba21d24b2b7d6ad7e1`  
		Last Modified: Tue, 02 Aug 2022 01:40:22 GMT  
		Size: 3.5 MB (3480396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5876af59b8eb33cdd8bf87b6b512f61e104fade6fdddd8532c9ab1530c05ebe1`  
		Last Modified: Tue, 02 Aug 2022 01:40:35 GMT  
		Size: 39.6 MB (39564971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
