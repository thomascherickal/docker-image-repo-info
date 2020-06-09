## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:938f926ad49f057cac819595d5daf5feb53d98e1fb4c49315f8e52069fa25429
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ce20d2552bb0c5b928bcb0e04cfd6058e9cd765f9a4c4e7a53254d3c2fc30629
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125496597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c54c9580cf7437cbbb84ff4cb13c0ad4098d3361df95144b2b9ae3ed03f035`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:10 GMT
ADD file:5c0c0fbac6fe503c1d3e894e0b3b1081172862074ceed378a7e4b82810536415 in / 
# Tue, 09 Jun 2020 01:20:10 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:44:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:45:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07f1101e3e85b531862163b4177bce7f401eac107a6537ab74195b395aab30b7`  
		Last Modified: Tue, 09 Jun 2020 01:25:12 GMT  
		Size: 51.4 MB (51413507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778b8917e949d9f5a076dfa475de8efd560f3537663e53ea97e720164dd04a8`  
		Last Modified: Tue, 09 Jun 2020 01:58:55 GMT  
		Size: 7.9 MB (7920377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4483e6954e0bd5f111c062eb05965cd7e6719912e726370891437022744c5b6`  
		Last Modified: Tue, 09 Jun 2020 01:58:55 GMT  
		Size: 10.5 MB (10488194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4457fc20950e802370e7f15361944b8f58ae25f895ca6cd42e008e97f37e60fd`  
		Last Modified: Tue, 09 Jun 2020 01:59:10 GMT  
		Size: 55.7 MB (55674519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:80dc6e43ffce422199c091abcb69f79891fd0b189cb75cc0a00e0d67193cb5c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120370404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41ac1e5fc9f58bc63c9843bffa4fe73ca11f6f7cec05d3e7479e39931fc6900`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:50:42 GMT
ADD file:ce6e6e497a66e2260260f97fe2b75c1b96d64554c5be6b85940fc97e2668da58 in / 
# Tue, 09 Jun 2020 00:50:47 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:23:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:23:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:24:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0cdc268ccc707144d53d65848999b81d39614c650312788e7e7f99c56bad6d97`  
		Last Modified: Tue, 09 Jun 2020 00:58:27 GMT  
		Size: 49.4 MB (49386621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86dad966a8a2c2ed7fa83ce42c1fab459f250a20c801eeaf7703e5022cf7bfe`  
		Last Modified: Tue, 09 Jun 2020 01:56:29 GMT  
		Size: 7.5 MB (7500258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5380110dfa23bbdc9c556dbde735e0c5c0b768f93dfc86e54d0c9e2adb417562`  
		Last Modified: Tue, 09 Jun 2020 01:56:30 GMT  
		Size: 10.2 MB (10175863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1be4fce84e1c9c761b63c553df33838f2c301c69f612c6a0c17003702eadf4`  
		Last Modified: Tue, 09 Jun 2020 01:56:54 GMT  
		Size: 53.3 MB (53307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:09045d0c513ff14b62be45236791142c3bc5e5f1e529bdb60729b7ab28aedae3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115351772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e47f785ed6f54fdee147ba9825f66ed91f09b5674678c2d1d2b74d276f2e131`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:59:35 GMT
ADD file:2ade41d5fab2319a3cbf973cc24aec4f6b9e2b14fa04578886fa1cbe30e511ef in / 
# Tue, 09 Jun 2020 00:59:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:38:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c27049a799a3404864ae1732d5aeaafaef7ce0fbbde552819e2c88bf38ae9da`  
		Last Modified: Tue, 09 Jun 2020 01:09:22 GMT  
		Size: 47.2 MB (47197823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b26b1bf1a6c82f64fb3246383f0e2081a0624861a1d56ae6b025e7406652be`  
		Last Modified: Tue, 09 Jun 2020 02:09:55 GMT  
		Size: 7.2 MB (7243223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ad054395bdad7163609959df4dbaf402b1787fb76da08b5c5f89358ac9f2e1`  
		Last Modified: Tue, 09 Jun 2020 02:09:55 GMT  
		Size: 9.8 MB (9823296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf531c73c6f446da9fd9e5bfae5da82ba0d7fc288a2c05cb2981e723a94e0fc`  
		Last Modified: Tue, 09 Jun 2020 02:10:19 GMT  
		Size: 51.1 MB (51087430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e22a87eb96dfc8cb4fe7ea428bb82e659aa05f591bd3953d7119565e02b6b46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124401457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b467252d54f2963448e2e918f3bb7e5519a067f01d6b4a03597248a1f9f5d827`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:41:55 GMT
ADD file:47e352caa545ab1122a3a9df6a86296796c3b1633a1a8151d6fb438f88b47d5d in / 
# Fri, 15 May 2020 12:41:58 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:02:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:02:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 20:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:523842c45f03b461bd15f8ec65b3e2670cde3c595006ef67af2d46f30e971812`  
		Last Modified: Fri, 15 May 2020 12:52:36 GMT  
		Size: 50.3 MB (50328985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e57198818fd11918588ce78d9cd056305b237e52e37463ed090e08379da0ff`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 7.8 MB (7809462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a6e14baacb6f567947c7991213c158c4924519e3e8e989752bb8ff12813c7`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 10.5 MB (10459841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb68fda96e6d2109cadb2b094a5f3b64b213595b13f3f88bf43deb6e56b33d`  
		Last Modified: Fri, 15 May 2020 20:18:16 GMT  
		Size: 55.8 MB (55803169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:64e3c0d96bba9be04ffb9d8750f21201747b11ea081c20e26faa3adc3f6c9293
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129016003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1a9be4d8fc78c7086c774c7c473c726a77b550a92bbb18c0b975d8345cd6c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:02 GMT
ADD file:8b8ef4a5f8149eba4e2e5c50f0e95fcf5b9e729c8fdf74e04ac12871a5e80281 in / 
# Tue, 09 Jun 2020 01:39:02 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:09:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:09:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:09:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2c89c7c8738f073b61540c4d15c26608d6fa4a9756e727acf258769f4f15726`  
		Last Modified: Tue, 09 Jun 2020 01:44:12 GMT  
		Size: 52.5 MB (52522870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68ddf662651a633a2f0e4f65ad7228c24d57d8b14286a1b62fac342f6375f75`  
		Last Modified: Tue, 09 Jun 2020 02:30:14 GMT  
		Size: 8.1 MB (8099334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad6eefe2105d3cfe168434dd0f3ae253e5013636bf2e2cce89b8545995ea84`  
		Last Modified: Tue, 09 Jun 2020 02:30:14 GMT  
		Size: 10.9 MB (10869142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66019f865e61d00591abfb7d0e9c883b48388b55debf3277d36172b8bd3a424a`  
		Last Modified: Tue, 09 Jun 2020 02:30:44 GMT  
		Size: 57.5 MB (57524657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4a4886053ef4cf59ff7b0faacbfbaca597ad92d739141f2287c6497eb7140de7
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122726423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d08fb85567629695b13194105787b344e4dbbc44279a61b59f25e60e06099e3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:08:53 GMT
ADD file:080fe104a5c84718f0c41015a3a4bf48ef0d94088beb50e3b0346ea572302008 in / 
# Tue, 09 Jun 2020 01:08:54 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4295b4a99b75e24118d0a604e63b142af1639be17451d6724215fd11e6fdd041`  
		Last Modified: Tue, 09 Jun 2020 01:16:09 GMT  
		Size: 50.2 MB (50162108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6b19c74224bd3e9030de803cd7b2cf6f938ee3548998819522a786837b1caf`  
		Last Modified: Tue, 09 Jun 2020 02:06:44 GMT  
		Size: 7.4 MB (7447679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e65e61fe718bcf10bce9dbbedd4844ba55e178913be199a5e4cd26a5ca17f1`  
		Last Modified: Tue, 09 Jun 2020 02:06:44 GMT  
		Size: 10.5 MB (10505180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ba7560d369d9be99a66746b1d7e1a04d087826851c960badca01c94c787d53`  
		Last Modified: Tue, 09 Jun 2020 02:07:39 GMT  
		Size: 54.6 MB (54611456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3a7be10ad2e88263a6697ccb41ce2f072ab2af20392db6e434af2459ef7c9dd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135693870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76abf0378f9c85f53029205aac12168521ef58f6ecc2c0c1eec5cbd9e1e1cc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:32:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e43969f6c0ff55aa4240214980deed196b68292106e0144d8d1290495d9b7`  
		Last Modified: Thu, 14 May 2020 00:25:02 GMT  
		Size: 8.4 MB (8356860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eacce9e1d274d8f139e9d384ceb5e66a86ca1857d025523765b1b099330719b`  
		Last Modified: Thu, 14 May 2020 00:24:57 GMT  
		Size: 11.2 MB (11176806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12dd448830e6ab4491686ac42b85cc8f50e9b182a8b19722842140e7e06c1af`  
		Last Modified: Thu, 14 May 2020 00:25:53 GMT  
		Size: 61.0 MB (61049897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:63bd0bfeb45f6b5baa6c9fd8b53658c2e76266b29088d76a855a88ead9f86787
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122886620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5ab76c7c9c50c83d249ad67510566aed450ef144f8daf6e4c7a9e8d5321198`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:41:54 GMT
ADD file:336fb2c808ef96709e7e692ea601159ca29f93c7988099e297914a1da2171aed in / 
# Tue, 09 Jun 2020 01:41:57 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:06:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:07:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce762a1b284e798ef27a5aff0cba859d84a0fba00f59301a1163551445244322`  
		Last Modified: Tue, 09 Jun 2020 01:45:51 GMT  
		Size: 50.0 MB (50017615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ae223e3890552865d89503593412dff73329ac57a5e1550cefeaed9e23915`  
		Last Modified: Tue, 09 Jun 2020 02:17:11 GMT  
		Size: 7.6 MB (7589158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63065300ca352f26ee91c5fb6965d3499bb2bc95f1f600246e2c04629eae948b`  
		Last Modified: Tue, 09 Jun 2020 02:17:11 GMT  
		Size: 10.4 MB (10366737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee31e3673869659188c0be9686bac022662546e4bd6a5f2af2070f533e66567`  
		Last Modified: Tue, 09 Jun 2020 02:17:27 GMT  
		Size: 54.9 MB (54913110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
