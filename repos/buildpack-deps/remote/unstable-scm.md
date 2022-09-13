## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:bd27d999826176f8fe47495e92bde630b0e9511a933b1e0c259521d389aef3c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b2d5286cbad5f8ed5edfbc654eed430078d3793b1fe504ffa25550d70cfb6eda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75beaab1ccbeacadd2c0ba743923d35c0d9efbd9ac65e25d791a7ad7d8e7d9c4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abee259a1d9101a0890f49e244222094315b4c017c58d8cb8a6cc0cd43e833`  
		Last Modified: Tue, 13 Sep 2022 03:52:28 GMT  
		Size: 9.3 MB (9298049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8698192cb686ddacc8322753abf5c95c28d7cca2e06243ec755c2044f89760`  
		Last Modified: Tue, 13 Sep 2022 03:52:27 GMT  
		Size: 11.4 MB (11380792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a113e2744da1b277bfdaa7b2eb0ce67a02441dae47ae08b93fc8cade18fed1`  
		Last Modified: Tue, 13 Sep 2022 03:52:47 GMT  
		Size: 58.1 MB (58067914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3790e08befbd29836b37ef45b9e4effef84810f67d841ca40ff6658ef4f1a6f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127315429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6892c8a75ebf24db9b3aac5cb667ec8003f81280ed22f345c89797eb47c1264f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:56 GMT
ADD file:deaaf7142ee9e9a9e95756080e3fc42695c32c1325ff22432d1a8335978dc0c7 in / 
# Tue, 13 Sep 2022 00:53:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:27:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:27:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e65672912f1f23209ba2457b7da75b0ac0f01a46e88659ca267298886972343`  
		Last Modified: Tue, 13 Sep 2022 01:01:43 GMT  
		Size: 51.8 MB (51785975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450eec1a6153448c36952598d71f319ac819217fedd3e398f945533effbdd0ae`  
		Last Modified: Tue, 13 Sep 2022 01:33:08 GMT  
		Size: 8.7 MB (8742366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088da11e23af30c629ee1464862f0f4a3fa55ca8c0ebcb8c54f7acd20d8111e3`  
		Last Modified: Tue, 13 Sep 2022 01:33:09 GMT  
		Size: 11.0 MB (11029211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a09ddfaca20e6dc9446c7d725e5492c92f2a4a2036df61574e3b7511ece7b3`  
		Last Modified: Tue, 13 Sep 2022 01:33:34 GMT  
		Size: 55.8 MB (55757877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a1f8c1940ff94f1fe7160cabc22279c4da1f87d722bd3622ed58c681a7bc26c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122305412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907fe6c8af6435809315022e3274f80faeda7edbc031e6a4c1447d0326bb532e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:44:03 GMT
ADD file:6c202b99cd5c91b3c2b2bc39ddaf5738d4def8520e18a716d249d62881657e5e in / 
# Tue, 13 Sep 2022 03:44:03 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 07:37:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:261cac8f52f598a2e1428463187e026d01259f7076e6ca3adf9b13c1414ba47c`  
		Last Modified: Tue, 13 Sep 2022 03:52:11 GMT  
		Size: 49.5 MB (49523940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e346b65163965ce437753259a3a5635ac1fdc3d48b6735d5be0f1dc103653`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 8.4 MB (8397051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c75620166463dd3a4557387e6591fccb3f2196f7d3af1c7d033dd15cc6cc0cd`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 10.7 MB (10659656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd2c4f9d78247385adc3f52a5344d1ca72d43e2ab8f373b72acb1de956dcce4`  
		Last Modified: Tue, 13 Sep 2022 07:47:29 GMT  
		Size: 53.7 MB (53724765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:27af6bc48046dbb0124adfee76256363155522f89bf9cec2bea204b160a20b2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131297285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:862e5e494c9e7fa2e2817e2ec89948779dfa12154a09f1f0d18bd9d7688734bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:54 GMT
ADD file:13af7384e2c4f0c81e2c22e39e5d930dc4524d300c5f3d92ab3288096c308777 in / 
# Tue, 13 Sep 2022 02:11:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:04:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:04:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:113c8010a5d8650dba62a6df118557cb9b270a562e4a0537563cf79291f65ab0`  
		Last Modified: Tue, 13 Sep 2022 02:18:11 GMT  
		Size: 53.1 MB (53103634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f00ceb8508161cf15d9580001f11e56a6e5eb7d0293d831a4d3bb4932e1050`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 9.1 MB (9127731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac595041e810cadc49116d5630a0f49b2e0bb6084756143d92c87a24e9c24f`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 11.1 MB (11133512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d53dea7bf1a209edbd8cd322893334f5833b0fe4fc7f12f48fe6b6efe11e6f`  
		Last Modified: Tue, 13 Sep 2022 05:12:43 GMT  
		Size: 57.9 MB (57932408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c64510c2ce14b7f3c0ede9aa2989f04231429d382d21c66aaae35a6a1d6d459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc54499ee1c5ba769bac4c6d77cf7dca1a4689210e47d3ffdd73fbb2c057a67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:48 GMT
ADD file:6c1d0f31b3527c2c240577c73b2476b1c6bcb8fa8d10fea614680e40f1c15858 in / 
# Tue, 13 Sep 2022 01:40:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:52:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 04:53:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d4ab670272048731963c87509c528d8f874ef24e7e5eb410c2b800aea0d16cb`  
		Last Modified: Tue, 13 Sep 2022 01:47:14 GMT  
		Size: 54.0 MB (54012005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c04187b376672562963fd175ddeca1b7d946a1a8549cfced79b8ad15f14bfe`  
		Last Modified: Tue, 13 Sep 2022 04:59:31 GMT  
		Size: 9.5 MB (9473423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab613e1d69d3fd1948062b98b955ccac19ca917e8a3dcc8e71abdc22b83e9897`  
		Last Modified: Tue, 13 Sep 2022 04:59:31 GMT  
		Size: 11.6 MB (11576535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e07ced1faf9475820e62de73f3541fea07b3862a0dbccfeac8685967d00dd`  
		Last Modified: Tue, 13 Sep 2022 04:59:51 GMT  
		Size: 59.7 MB (59675489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:be3cfb47ad33e8486992ba11215e24e84cacd7c9266e925fb9d4a48b3442f068
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129749351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629cfa93c4aa74ef348f01bfbb1146c1e9a0a90fba80d5a9f289a386d33936d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:30 GMT
ADD file:dc60ee74dfccba12269b444dd45f20e0133d724b1942c6b0f9c5194eb68bc303 in / 
# Tue, 13 Sep 2022 01:11:36 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 02:00:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b00b55b6e19db9300c81bc3c7da4bdd60a1432296143ff24c14dc6d0eee819a2`  
		Last Modified: Tue, 13 Sep 2022 01:19:36 GMT  
		Size: 53.1 MB (53078760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86798e592e4c27c8b93559a482630aeb78e21c77d475b6073a710cedc010c221`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 8.7 MB (8662682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e754dd24f2e4a96086e83f849cac69c8b471a4e9c281073faa059f3ffbe46df0`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 11.1 MB (11126979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351873532902ed248b22ff16c56ca4bc1b19a4eb00d077f99216736216e8e2df`  
		Last Modified: Tue, 13 Sep 2022 02:09:53 GMT  
		Size: 56.9 MB (56880930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bf65ab0139b830d02fd51d2d4b4d00c51526c95a99b06fa8c7ba1fead4bd008e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142067694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b1ab9ed49e05cee0724793e10efea28eaa604b6961982b4f63d3c939310f20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:08:14 GMT
ADD file:7d9f6a3f8ad433abf431bcad8e6116e9904ba35fc9bce2c28a606c6e697eb4ad in / 
# Tue, 13 Sep 2022 02:08:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:17:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:17:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:18:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a14f00c47c74a23076b6e04f2c1edb527d3e4b88249c3395ff38af7d4a745799`  
		Last Modified: Tue, 13 Sep 2022 02:14:11 GMT  
		Size: 57.2 MB (57189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735886547a07f8548c5997c489b42bc8ee28201c1944154a2d51099b3431a97e`  
		Last Modified: Tue, 13 Sep 2022 05:26:48 GMT  
		Size: 9.9 MB (9884481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4869677af77dc3f19d87e03cfd23841b6b7b0c65fed4be462f2bc786a3b67`  
		Last Modified: Tue, 13 Sep 2022 05:26:48 GMT  
		Size: 12.1 MB (12142712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ce98afb4b4ec55ce30ea48aa7da9329b7619f43b0bcd31f96e1e3766b19ee`  
		Last Modified: Tue, 13 Sep 2022 05:27:16 GMT  
		Size: 62.9 MB (62850919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:71e5cc1320cef8c950fa66f43b308ca184df3524c0599ad884b59f83e9653eef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123135872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706df53c2ba215a83a7d5da01705bd278182db468c40406869882891dacd0c7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 02:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f5ac0089cbc5e6a2fd5b2e4f0a87d121dfc9b18f21dfa4cbfa5fc80eea4dfb`  
		Last Modified: Tue, 13 Sep 2022 02:44:33 GMT  
		Size: 54.0 MB (54030810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b54c9d831a7d644f29903c35f1ebfd7b3e6267ffb2ccb9ba92d16d2fd0ad1cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128914854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ebdda1c64e12107af61b1b1b329399859a4b575ee107ab286acd63fbce81c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:19 GMT
ADD file:c95e2b098d871c8f60e72d16096a4bcce80e256166b62df3ac0abf8c1cc5384d in / 
# Tue, 13 Sep 2022 00:48:22 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:27:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a47738c5650c377467230bf819bb4be695718c6effbf5489b6e0fc8e11229d95`  
		Last Modified: Tue, 13 Sep 2022 00:52:55 GMT  
		Size: 51.5 MB (51537006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa5a30de3637ebbcd271e1f1795c92f2432d80f355e866dbb37a7875ba82d9`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 8.9 MB (8935914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2c639682b677cbe7eebdb0376ad10594f99f1d23baa05fe3c38f108872567c`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 11.2 MB (11238889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0c71abe4e7d488f67e164d6e756534c33e5365e594afc695cfbc8dc27b493`  
		Last Modified: Tue, 13 Sep 2022 01:33:55 GMT  
		Size: 57.2 MB (57203045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
