## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:a313748aee07ee21dae0bffd41480c1d2e1838e226b33a5f16c2482a971a3402
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
$ docker pull buildpack-deps@sha256:89525570cc62a18f90b561f94ec9111ecff87157767181293ecb06c475c671b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129826986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10abb968ca71a1bf00261959ee253d8e4c332736ac2ea81a3df52e6f72d5bd22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:37 GMT
ADD file:859abf2d579747b132742454ad96e32dc879955afff8af84fab63dc41312a0e0 in / 
# Wed, 20 Apr 2022 04:44:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 07:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:212be0dc3a8ffdc400158a5e3a9812f7413dbb5a86269ff50e41b84b37fdb9f7`  
		Last Modified: Wed, 20 Apr 2022 04:50:51 GMT  
		Size: 56.1 MB (56112566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0603dc0dbc00177fa56a8c1af60fd29d0bf2e8e1e8df8772164b08d8ba1ac`  
		Last Modified: Wed, 20 Apr 2022 07:07:58 GMT  
		Size: 5.2 MB (5209066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da99ea31fc35c2341d30c71a1992c692753c04c61b2e1c25053bc3f9d269992`  
		Last Modified: Wed, 20 Apr 2022 07:07:59 GMT  
		Size: 10.9 MB (10924522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a400dfe0377271d31b8196be8ab40ac2db5aa00dd677d631d372b1df286ddb`  
		Last Modified: Wed, 20 Apr 2022 07:08:18 GMT  
		Size: 57.6 MB (57580832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8439fb8b385f8cc11abcd6183924c2b48f3a94cd6399032750ba3d6967d186db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124495170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dede622cdd74a63b8d99b43833aef742deb88cb75e710c1e5c8476dea3ca5be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:20:15 GMT
ADD file:5cf288f7326d2adfff5d4d3ad0b8951ab86c23ab83cbd1d7799d5c3f7e16a857 in / 
# Wed, 20 Apr 2022 07:20:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:47:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:47:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 12:48:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8db2a46143e157b04953cf05194b0c408afa491a70876185538ed8dca91f9f55`  
		Last Modified: Wed, 20 Apr 2022 07:37:08 GMT  
		Size: 53.5 MB (53518487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341b88f54fc68d22e9e84a8661e65a14684ef134f7f3e5501db09108de37dcea`  
		Last Modified: Wed, 20 Apr 2022 13:07:30 GMT  
		Size: 5.1 MB (5105948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36b40c86c120d43041e78ed7cce077bfa51b33140635f860a17b56fd9349f04`  
		Last Modified: Wed, 20 Apr 2022 13:07:32 GMT  
		Size: 10.6 MB (10597935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445e44e0b7b81da5c386d988323b74e27b2d376a346d93dee764c34c229b7cb8`  
		Last Modified: Wed, 20 Apr 2022 13:08:23 GMT  
		Size: 55.3 MB (55272800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8da87533204b1f590f5251e618b455723ee3a2a4072dadf74fcd26e87984ac79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119539684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a64994b34216f64da7d61c6219d12ebbafbdba5d7d65237127d357187287139`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:31:17 GMT
ADD file:0bbaf7ead1d59ceb682d490a4942a357b01272b17a3eb062c89673ee4e166052 in / 
# Wed, 20 Apr 2022 13:31:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:14:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 20:15:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bdfb6c7c7f66a4f6d01a8add17283f952a25f6c31c2267fd53d1ff9148edc16`  
		Last Modified: Wed, 20 Apr 2022 13:48:09 GMT  
		Size: 51.1 MB (51125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4823bde2923c5442c606b104de74dcb0814457fed2088fa724dd6831b9767bbf`  
		Last Modified: Wed, 20 Apr 2022 20:36:47 GMT  
		Size: 5.0 MB (4962895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767785c6f4268da31b8fbd1e7bd3fae5bfea9198e83ef63566d05d7bdce6428`  
		Last Modified: Wed, 20 Apr 2022 20:36:49 GMT  
		Size: 10.2 MB (10244681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ed9c3ce00c659ad57fb1966e00c23737a28269aca3c7f45e75e5465b127332`  
		Last Modified: Wed, 20 Apr 2022 20:37:36 GMT  
		Size: 53.2 MB (53206444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fa0a1d0743202d712e076273d5d6e54530a515a9b629b527ee639640aced1d17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128525138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d47665dc88b10e3ec024d39c07c4474e932954e98af456ac2c542b181138f9d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:37 GMT
ADD file:21175f4b5f80ba5d755041ff362152a8991b53f89e3c6699275e0c99f6ff6acd in / 
# Wed, 20 Apr 2022 04:30:38 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:47:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:47:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:414d522b7454847f294a8c61536f57f36cb195df33ab1fce8c838de3d5ae109e`  
		Last Modified: Wed, 20 Apr 2022 04:38:18 GMT  
		Size: 55.1 MB (55063805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc9a9c4b1c386c65ac98874ab622afc88e90b73f7a0e1c692ab412bdd01c571`  
		Last Modified: Wed, 20 Apr 2022 06:56:31 GMT  
		Size: 5.2 MB (5195986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d918141859173a7d14691da560e5afcbb7c353d5694d9541d73f88867578c95`  
		Last Modified: Wed, 20 Apr 2022 06:56:32 GMT  
		Size: 10.7 MB (10691633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541426f7af00f836dff3b2b6976f4053e14eb4fe2fe3a8f804c6b8781c7c3fa0`  
		Last Modified: Wed, 20 Apr 2022 06:56:51 GMT  
		Size: 57.6 MB (57573714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:943ce3ae3c525b37d4092d548129a5c4069582e648d85b6f1cd73fce7aeefcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132646725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1922d4df210d4d5cce69ba302f70f95fa3ce71030382cb8708c79dc2b427a41a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:08 GMT
ADD file:92a4df746589380f0ee875ec89574f67fa2f56164bbf20da79eaa902a778eff6 in / 
# Wed, 20 Apr 2022 07:39:09 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:20:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b42fb3c96c9db2aa67a5b3b033791b735ef01e8c8f15321f44a085532b703190`  
		Last Modified: Wed, 20 Apr 2022 07:47:30 GMT  
		Size: 57.2 MB (57154017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00924a45119800495fe2fa0b6d6aaf354e649da6676746c97c18df9c77e13002`  
		Last Modified: Wed, 20 Apr 2022 10:29:51 GMT  
		Size: 5.3 MB (5340392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa8d253e5b8d891d6ce9b90e438656a4b5f68ca7b4dfb8f73c36b3da2e9043`  
		Last Modified: Wed, 20 Apr 2022 10:29:53 GMT  
		Size: 11.1 MB (11104264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f2bff506a180a1affdf12a35e0f3c11ba1731569fd21a8a49b19251f503f8a`  
		Last Modified: Wed, 20 Apr 2022 10:30:13 GMT  
		Size: 59.0 MB (59048052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6b12d00824474333e2a83b3030dd2638bf9717953d50005bddf4061a9762dbba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126848704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f910101301810453cc429c78a440678b17803e89b44762ce47e9256f5f6f459d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 14:31:30 GMT
ADD file:3ad0c34fcd14c5fe7c8ebdd604aaf6408b7bd1797df3867dc95c1e62649776f0 in / 
# Wed, 20 Apr 2022 14:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 23:31:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 23:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 23:33:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f4c77aff8255984992f37180c0f928131e7372860c0f93b1c0b9320726de80d`  
		Last Modified: Wed, 20 Apr 2022 14:42:37 GMT  
		Size: 54.8 MB (54772282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c264f04825b386c359d75b8413b57333d2dc19406b712e4d068e217c52bf8`  
		Last Modified: Wed, 20 Apr 2022 23:48:36 GMT  
		Size: 5.2 MB (5160621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3717b462f275ec8cc92879f116a0d1eb9a8d0edc5909c1aae7979d31243449fe`  
		Last Modified: Wed, 20 Apr 2022 23:48:38 GMT  
		Size: 10.7 MB (10673322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb29766e9c3cd0abcf658b8bfd96d7d63ea6a56b6844d0c07b603a763139d9a`  
		Last Modified: Wed, 20 Apr 2022 23:49:27 GMT  
		Size: 56.2 MB (56242479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7499727d4a5225525bc7b754a2587201e45bc7b9f940b64414dec247585d560d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140007983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee85556520eb1f67b39ffb0c489b90d2bf79e54040baf5f7d8f76d95a0cdca9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:49:13 GMT
ADD file:fe481980541905937ff6238feab8ead20ee273dfc616bf9e647446ec0f98b510 in / 
# Wed, 20 Apr 2022 09:49:19 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:07:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:08:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 17:09:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a4e99688ea8909140343db9b1a83e87f7ddcee1e1ba6d630b79487e5e720199`  
		Last Modified: Wed, 20 Apr 2022 09:59:29 GMT  
		Size: 60.6 MB (60558000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d38d0e81f1d25142863d436c077521a366a4b21640a92ac901895221e55ea`  
		Last Modified: Wed, 20 Apr 2022 17:34:37 GMT  
		Size: 5.5 MB (5483458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48f909cc9d2e0af9952aff147f17b193c00be915fe067146c11dec81ebc29a`  
		Last Modified: Wed, 20 Apr 2022 17:34:36 GMT  
		Size: 11.7 MB (11703518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d315112327d37e1ce52ce2a20207b2e675c4977a693bb657bb705301a4348b`  
		Last Modified: Wed, 20 Apr 2022 17:35:57 GMT  
		Size: 62.3 MB (62263007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:9ecab38a01e3293e383f1c1e05f39d55b70ce5f46485e0a6a115ed4e73b2db88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121417253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2800581f75c7840f0f04607fa7a0cc1492b9e75655a7bd5606148d295da500f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 00:15:39 GMT
ADD file:250fc868a440657403e5cf8fde95da30be6fa0968ce4385656b837e923d678b0 in / 
# Wed, 20 Apr 2022 00:15:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 01:02:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 01:03:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 01:25:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d7000bee08e5edd84dede58b856acde7ae5b24268b5109b3fe7e2260ac19618`  
		Last Modified: Wed, 20 Apr 2022 00:34:42 GMT  
		Size: 51.8 MB (51757327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa082dac6e71b36c14761bb8e8e6da43417464e08b11b0729bf95f3bd2741231`  
		Last Modified: Wed, 20 Apr 2022 01:35:22 GMT  
		Size: 5.0 MB (5016640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe9981ca4f10e51876d1697f6c0393395afae2737f4194422601ede16a3dfcc`  
		Last Modified: Wed, 20 Apr 2022 01:35:25 GMT  
		Size: 10.3 MB (10324162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee1c60c98e49b0ca61bd33feb06c463e03d6494741dfb8b5b9a5b949a2efa5b`  
		Last Modified: Sat, 30 Apr 2022 02:26:16 GMT  
		Size: 54.3 MB (54319124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f0f7d03377aeb13b3702c16a615167883d858199a9ffe7018ce819100b7e8aff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127234276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008f0528cf59906fe56d1772a3c4fdacbb27d1abc0c68c5318bac1e5678334d3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:42:10 GMT
ADD file:39be572f6c0b3f6f84497807d4bcb370f80b4ac4167f1857002b5571a4dba6b2 in / 
# Wed, 20 Apr 2022 08:42:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:21:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d9529e5f0bb592a3bb453a841aee9e6a765fede232bccdc538ec2c8b96421d2`  
		Last Modified: Wed, 20 Apr 2022 08:51:05 GMT  
		Size: 54.3 MB (54330969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8df2c317b7e7ca98f001f2d15c613527928de02e7eb3e9f728cd782b7338cf`  
		Last Modified: Wed, 20 Apr 2022 11:29:56 GMT  
		Size: 5.2 MB (5186233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e828f9d86f39827cc0435a54750db181b2f8df2785eca1dddfe35a5536c021f1`  
		Last Modified: Wed, 20 Apr 2022 11:29:56 GMT  
		Size: 10.8 MB (10818188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7992815e0e3b1d2397114927abda25dc906ea8fce59d9acb7a8cbb8c4c2e98`  
		Last Modified: Wed, 20 Apr 2022 11:30:11 GMT  
		Size: 56.9 MB (56898886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
