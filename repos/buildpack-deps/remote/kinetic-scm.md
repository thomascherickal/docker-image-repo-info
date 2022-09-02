## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:7ab6640cdf7d6dcd8eab9645ffa82212dd1c802cde64a7848ef79acafde2914f
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
$ docker pull buildpack-deps@sha256:828ba173c64d2b06cfab5015d103cacabaf810768a3edebde3bc29cbdc44e5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77570973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf0e5aaa1e96e04823419e7cc270da44b5ef7482b69063331a8f8dc4851ba7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:32:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71363ea1301988ddf4ef6039b34a05a19b44a70e1ba2764e95fa0f47b3585c12`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 6.8 MB (6779788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d261ea038a7743d40031459e01e57001571ca5986a617d9e2d3174c66d98187a`  
		Last Modified: Fri, 02 Sep 2022 02:39:23 GMT  
		Size: 3.6 MB (3633660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee5c450c1549fab83f54e9138820f82132ebf0b50a52e7ffb97b6074e98c1b`  
		Last Modified: Fri, 02 Sep 2022 02:39:39 GMT  
		Size: 39.7 MB (39729510 bytes)  
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
$ docker pull buildpack-deps@sha256:0ecd3a16684ad715fdc64797dcb67e50a578b932508e659b89877e29aeb60c31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78259290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eebb88c0344c66b13bb1996a4cd968b97228457505a37dac024aed53fc270e0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f129e4299698e3c5c9ab8769330e17dd80fdc69e682f5705ef355e75dfc32ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75653148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:505a854970b8539945a41a684cd6895a2b377733c46184f17c584767122c2b75`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:10:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:10:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a9727cdfe9e4d0ad02573de5f42a04ee40c70d014fcdffb4b684522e06d667`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 6.5 MB (6470487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626668509bf2d37bfd328fa211e8e7ad57c719072d9c7f1fc379bc2c187745`  
		Last Modified: Fri, 02 Sep 2022 02:17:04 GMT  
		Size: 3.6 MB (3625387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947234f2c6685065fd711d09a80a70640e7a9c3b7521b8bbdd0c52afb85d8b5`  
		Last Modified: Fri, 02 Sep 2022 02:17:16 GMT  
		Size: 39.6 MB (39561768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
