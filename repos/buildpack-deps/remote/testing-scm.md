## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:52796add874d5c9e549588bc1def4a882fb89f58a8171dfb9a22208fb9d657c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8735fb99988269c8a2b89299ebaf55d7d69e8308468201cad8294119bc01725b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131269061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7ef268718c160b48b1775f18503f088a97025240ac20125e240281ff504445`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:19:54 GMT
ADD file:7e968e6ae38ede120a52f1d2e734b4fee4fd4ffd6e5f747edc8190d2a8bc6a52 in / 
# Thu, 23 Jun 2022 00:19:56 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:48:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8849e73adf621df4a443e9ac4eec9b698476e4f14f8ed894806f302d5b33156b`  
		Last Modified: Thu, 23 Jun 2022 00:24:12 GMT  
		Size: 53.0 MB (52993983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a3004561e732519f3aa704178d4bc2d97eae3c1cc556af0ea0d3e66e28ba24`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 9.3 MB (9291497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0f93f12fe636ab6b9beed73979390ba6a1aa6fdcf7bbc5cb403f683142a0e3`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 11.3 MB (11264030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85c343cd3e553d90219aa415a28525986ebdcf4ed151ad763eea350150fd70`  
		Last Modified: Thu, 23 Jun 2022 00:57:52 GMT  
		Size: 57.7 MB (57719551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:be983a23293cada11119049bd73f41a925b1d2e81d0e85afbd5ff6f1c28e5c67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125809657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7176eaac8a5f1d7d4bb21260631ceefb6bf6078160168a387e460b206520ce60`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:49:07 GMT
ADD file:d8a58d5f4d1c34aefbf2ca6b2eeab0bbf20b8cb6400548926c6a16cce570dc9d in / 
# Thu, 23 Jun 2022 00:49:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:32:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:32:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:34:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5248fb4f18035bd1257a3136675241430095c1cdf250910c001999b7f421381c`  
		Last Modified: Thu, 23 Jun 2022 01:03:30 GMT  
		Size: 50.8 MB (50767843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b7a64f309184d3ebc17e9dbe6bed869037215ff9f9748c7dffa9ffd3e631ee`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 8.7 MB (8726860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a0203b6e2645c48e6d7e1a1ec99807f7da08cea315ce1d19d9ca8ae62d6246`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 10.9 MB (10927730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f066702837fa4198900a9738fb6fce0276868d06d1e1cd19d0dda62c8bc1161`  
		Last Modified: Thu, 23 Jun 2022 01:59:03 GMT  
		Size: 55.4 MB (55387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1056ff9a8d523c4332a76628eb3927a8b979a913827a1d6cbc2b12a2280ebc11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120789743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:020ea930650a0891c8f0fd59e488f16dfbbfc231c6e437f0b11b6216a80a1cb2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:58:08 GMT
ADD file:485670bbc3d21c74d06e079229d1c74d05970c4bdf8c5d25692ab1464f0acfce in / 
# Thu, 23 Jun 2022 00:58:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:42:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:42:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:43:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da5c76d2fa54760a1e859c83968ea6d7dfee1c43064fb6f34c27f8d639859b07`  
		Last Modified: Thu, 23 Jun 2022 01:13:19 GMT  
		Size: 48.5 MB (48506514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231adce49f6a983a4cfa3f3683a6c276af5ef432ea37e705272135b3a56084b1`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 8.4 MB (8397133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487327d153dbcbea96feb013bca9efcd1fa6319396003a967515da5f4ab1d6a`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 10.6 MB (10572720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2c56a82b9fbf3bde9d03894c5080a67cf22d4eb43fb32978cc465e44267d81`  
		Last Modified: Thu, 23 Jun 2022 02:11:11 GMT  
		Size: 53.3 MB (53313376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:666aa6474b9943bb263bdfb7c54d8023773f4c6d43c0edc6b737c25b9a47bf3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129956051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5bca0c8a473e290af9440ae7773f3ba7f75e0a5143311c1165a7246258ebd3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:05 GMT
ADD file:149d923f098f33a347aa57ca673aae5cc103628b202337e4ff2ea5ac278e5c18 in / 
# Thu, 23 Jun 2022 00:40:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:09:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e34000263ac838bb9254930c5e34d9fa4b486f544707ae0aa508bb7ded624d59`  
		Last Modified: Thu, 23 Jun 2022 00:46:09 GMT  
		Size: 52.1 MB (52074605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d844fe46570aeb3a40b42c67a4714c432ac2d6ccc31125f7eeb076c05e919ff`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 9.1 MB (9126954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39d92840e0fe1b4aa70af7e37d1e6c48b3c61da85b2b3d9e13efb83c990d2d`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 11.0 MB (11041433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbe8b6171db521e3284e73fee8669036467cffe10b2030372d262cb498caaf1`  
		Last Modified: Thu, 23 Jun 2022 01:21:01 GMT  
		Size: 57.7 MB (57713059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:613adfc7b5f518a1f50612561ec8d14c3ed878fe6754ec6c2521e485c6899d2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134085106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0b196d8a676e45eb4be69cd16d32bd26ccc114852567b19d99e87f76113932`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:38:52 GMT
ADD file:d8108af9af2f3fb7f3dd905a9b4dd8391d568ba8dd590a9ca2bbeecd44354e03 in / 
# Thu, 23 Jun 2022 00:38:54 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:08:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:09:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0120d80f9ec3d96114e34087bd467cf9989c9c723cf7622bb16fb3675443565c`  
		Last Modified: Thu, 23 Jun 2022 00:45:18 GMT  
		Size: 54.0 MB (53963635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a0c1f242a443b42292f09b23bf00a038a40230b125f2d832ff706e0b0fd009`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 9.5 MB (9464738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2c7e9a858ffdd4f52faf3fc1e4e080485c9024f299858237d4b3961f4e27d`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 11.5 MB (11464163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000d7279af4a42e39fe0892505db82f28dc4127c5b4ff59701217c5f3921c339`  
		Last Modified: Thu, 23 Jun 2022 01:21:26 GMT  
		Size: 59.2 MB (59192570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4d3e1abd06c8e516a9fabbb3b39b030e8326fb328305bd30763da0da5d9fc625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128127521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2884b1270a2685260a263a49c7465734ec353f89583b74b94d9d79846ebc2d31`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:08:42 GMT
ADD file:8bc6b496d7debb22306bce782f6b34ee75efae7151dc19314b45a9751b8fbdb4 in / 
# Thu, 23 Jun 2022 01:08:47 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:44:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25ef8061366d5e6abd7ca324b8c1f08ba96be6bd0e55fd310e046a1e4becfdb6`  
		Last Modified: Thu, 23 Jun 2022 01:18:17 GMT  
		Size: 52.1 MB (52089294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8d0efe31fb7f6ccd1d5334126a57a6651ed1009e9a6eb93f4fb51019078cf1`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 8.7 MB (8657797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d342e8e78e8778dab632125fd70a05b026d9c29cfed07832f8527747409a8a67`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 11.0 MB (11019371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93153ce1ff5d2f9dd76da70875ccf9835543f0261f518018d8d826434056dd06`  
		Last Modified: Thu, 23 Jun 2022 02:17:34 GMT  
		Size: 56.4 MB (56361059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:01abbd67144a305250418e65b858e75358993e8e18e35803d943aff98b305a52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141575807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eec84a70ab72ec4f2b588aa5cff10b2b416f8c1e2b3dcd1362293a2632e4db1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:00:58 GMT
ADD file:d857864fffea40faaeec8c9492ef1805e6c891ebf06f1427f02398a3824debce in / 
# Thu, 23 Jun 2022 02:01:01 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:43:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:43:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 03:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8afb6214160c68cb540431e94c7bfe898f1a094dc45a834aa07634d34b1505a3`  
		Last Modified: Thu, 23 Jun 2022 02:12:13 GMT  
		Size: 57.2 MB (57198049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a70dd21016ae34b7615f4f27bc039c2c609a2ac123e43b625424da683ee24b3`  
		Last Modified: Thu, 23 Jun 2022 04:54:13 GMT  
		Size: 9.9 MB (9883483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb14a4d02ea4ebe3ab1ddfc7a7bfdc8945f0478c8c9592495931e4a0a21b69d`  
		Last Modified: Thu, 23 Jun 2022 04:54:12 GMT  
		Size: 12.1 MB (12065040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1582dcac09eb1694cd819ab79fa690166d66caa532597c54cb2899dc67c2f55`  
		Last Modified: Thu, 23 Jun 2022 04:55:06 GMT  
		Size: 62.4 MB (62429235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a373641202e7c882b0da9b89ef5e62a248c8e40d7b24353f807586f4dd9f77ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128655003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70a0ffdd52edd3fabb65952a0a8bdc149069739b2d4994a94ba626160ffa22b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:51 GMT
ADD file:b7c920f3965a4e47e7a0f42e020e195f493babee2f175c563676dd0d45c0b27b in / 
# Thu, 23 Jun 2022 00:41:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:12:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bb926b744d748e9437f2a0a451eea25192350981dae9cf0d8effd239dd22e761`  
		Last Modified: Thu, 23 Jun 2022 00:51:01 GMT  
		Size: 51.5 MB (51530571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ecccdf5c546fed3b800725dd538dd6145ccb9ae337d876c51b657ce9b04f1`  
		Last Modified: Thu, 23 Jun 2022 01:34:04 GMT  
		Size: 8.9 MB (8938768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98bfe7c167f54ada5e3d22060e56ad9ef2d8269fb0c0bbd4e5683afaf21b548`  
		Last Modified: Thu, 23 Jun 2022 01:34:03 GMT  
		Size: 11.2 MB (11157453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2649e5b4208cd3e4644788449131d6ce6bcdfd648d98111724b67c0429e1f0bc`  
		Last Modified: Thu, 23 Jun 2022 01:34:20 GMT  
		Size: 57.0 MB (57028211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
