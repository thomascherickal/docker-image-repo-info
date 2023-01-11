## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:792e833ecdf805ccea3ae20e4ba805c7e78ada7ec243435a904fcd5c66945c79
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:67ccfadba9024a28b93563f14db9944a2c649f233db3cfb90f155333678cf215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69428500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42de8cdc96b8d839a3f771af32b8372411736863b8062700709298617a3b2ea6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:41 GMT
ADD file:3bae49887734af64f153e9e3668684efface6dd04ba31139b3d6b3aeb7589128 in / 
# Wed, 11 Jan 2023 02:35:41 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:07:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:07:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a0e522725e09a558b80e5d58e7b360150ad3fe901915db5358002bba7e461b9c`  
		Last Modified: Wed, 11 Jan 2023 02:40:40 GMT  
		Size: 49.0 MB (49040747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9982d6c78fdd2a5e480eda90cc33945a46c3a49f844c51993bdb61ea401c22`  
		Last Modified: Wed, 11 Jan 2023 03:14:08 GMT  
		Size: 9.0 MB (9034446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f912e649ff1b5f13cde3e28b1254be9cef3ad6b8f7e119be8bade6ad4a2c301`  
		Last Modified: Wed, 11 Jan 2023 03:14:08 GMT  
		Size: 11.4 MB (11353307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dbf167c21240c1242196d8c90baff84fe0655902508a531fad9591f9d56fb1af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68339179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d887ab2a1969db624022a02ccf6517953432d7e4b390d23ad1d6ad45d3a90d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 01:55:48 GMT
ADD file:c258ec7f780b3ff9c8cd584e0032e838b39a09afc46940f4ac745695130b67ed in / 
# Wed, 11 Jan 2023 01:55:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:28:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a63c02841fd8a16e36e06a2fa4539584c2578f39a3f7bd88934a6c67fc294d9e`  
		Last Modified: Wed, 11 Jan 2023 02:01:08 GMT  
		Size: 48.0 MB (48017943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e0852ac4954f884346a0ba77b1c72d65daf0148903acb9a35db7dfad06d432`  
		Last Modified: Wed, 11 Jan 2023 02:34:15 GMT  
		Size: 9.3 MB (9319858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff229adae1feab6cbc20cbc1815df4cda72e4b5f1550cc783d1ac1878ee67d`  
		Last Modified: Wed, 11 Jan 2023 02:34:15 GMT  
		Size: 11.0 MB (11001378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:723454462b46c3071a1b1083b87d93223575eaab12cf652689732b945739d0cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.8 MB (65840117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f836d491b8a43622e2ff201557e259d0f7890b28b053493563132a85418994de`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:59:31 GMT
ADD file:9f6e7ad60906ff390d6369133d129df5057cc1505edafd2cccc2eefa5265ddaf in / 
# Wed, 21 Dec 2022 01:59:32 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:31:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:31:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4d12d04403dcef32bd0b6201954d02c0de421dabf04dd54d568898f376cb96c5`  
		Last Modified: Wed, 21 Dec 2022 02:07:07 GMT  
		Size: 47.1 MB (47080683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36680a9d2eba076180efb89a2b7a21233fc4e0a38e383b2c389f543e56a48be`  
		Last Modified: Wed, 21 Dec 2022 02:40:30 GMT  
		Size: 8.1 MB (8110360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edac00689713d5d2b7fdcc4f1c017ec260832d0c2a65021c7f013a4a71c9bdf0`  
		Last Modified: Wed, 21 Dec 2022 02:40:30 GMT  
		Size: 10.6 MB (10649074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5b19150ca15f1eb7c7266fadcd800e667b3b9ff81e83013d843b4c45b6591249
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70508385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60199b467e5dd3ea8330df0ea5fec2a5472ed13a1ea6eb114fa2143a2402da54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:40:22 GMT
ADD file:afdb0d23dc73b5f1a887a2dfc3fb8fc2ebf210e9ac6b5d6748cd89c77d9e436c in / 
# Wed, 21 Dec 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:09:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:09:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:951a6c4c03238810abf592f0f3beb641ea6b4153bfa55acf62944018b9ed669b`  
		Last Modified: Wed, 21 Dec 2022 01:44:40 GMT  
		Size: 50.3 MB (50335976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdda1c5e6e87491ced136c13ab5b4f5638649dbeff005a13d621df9a094822a1`  
		Last Modified: Wed, 21 Dec 2022 02:14:29 GMT  
		Size: 8.8 MB (8843497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae130f92dbc53edf856d24c52cbf32f0410d34ccacd94bac928422ef4f4fc7`  
		Last Modified: Wed, 21 Dec 2022 02:14:29 GMT  
		Size: 11.3 MB (11328912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:39688e5acae617a66aacac8b2c337df17081834d9766015d93e90d43ef79ead8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72091705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9cda77143d276c8089ad774d900671ffe8b5effc6bb0b67e9a95784bc53fe84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:40:20 GMT
ADD file:d73a77dc412cd093f533d8c6403c7a4a629d7a7d31b1ffc8555e0f7876d98ec3 in / 
# Wed, 21 Dec 2022 01:40:21 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:56:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:56:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e5477ffb90e4da3fe8a2c9a63f402783b74fb55b190b59240e4d1d7e5b55a2da`  
		Last Modified: Wed, 21 Dec 2022 01:46:35 GMT  
		Size: 51.3 MB (51340127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17da88d33e2a230fdf9667832a8cc65fca073921763a6ecc2a858766d4f937d`  
		Last Modified: Wed, 21 Dec 2022 10:02:31 GMT  
		Size: 9.2 MB (9186105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e431ea7ae865d881e1efe5608caa34a7813792150546854d8a8462ced5ba`  
		Last Modified: Wed, 21 Dec 2022 10:02:32 GMT  
		Size: 11.6 MB (11565473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:73d41217368bce50e169d9865daadd3d5485d5a756dc572306449a883b73ed4c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69788034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ebb67403d4f8ef4a6649282a3df5aa669795e3ea2cbbf6e66b43ed1f670f677`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:11:07 GMT
ADD file:bc4f0f717f54bc1982dd6d104f684f180c7b8da660351e5be4853a56b38e374f in / 
# Wed, 21 Dec 2022 01:11:13 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 00:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 00:03:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:22a773956e0933f1a01038ae977c7c99f46cd5ce02f672c66be9a1c837de4eac`  
		Last Modified: Wed, 21 Dec 2022 01:19:25 GMT  
		Size: 50.3 MB (50292945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189eef164aa69dcb61fb78c17df64c6779df804d82ba70a52d4e89d3b19eb0ad`  
		Last Modified: Thu, 22 Dec 2022 00:18:32 GMT  
		Size: 8.4 MB (8376404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1e283b7e05e1f80446c30786dca684e73248af2172c069b9d51b1bab48ee9c`  
		Last Modified: Thu, 22 Dec 2022 00:18:33 GMT  
		Size: 11.1 MB (11118685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ef9bdd4e7805981e28f314b3f1d6ab2368ca0b597854b299c641c02ca4e980b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76053714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3938d40149accd7e13667d3ae5d8ab4273dfd296e8ad33ae93a974fe776a560d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:58 GMT
ADD file:4af1feaa33ee2a3c1112b5ed0efbcccec637c4dc23a5af7d55343f6ab7005920 in / 
# Wed, 21 Dec 2022 01:18:01 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:58:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:47dc200f753ddc67a9fec80382c7c2b6f164cb907748c309862373fa8d94c504`  
		Last Modified: Wed, 21 Dec 2022 01:23:50 GMT  
		Size: 54.3 MB (54332986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e0edfe8dd05f3e4610a7a82df7e8bb9b034431efe825b28230c1de8996756`  
		Last Modified: Wed, 21 Dec 2022 05:08:00 GMT  
		Size: 9.6 MB (9590429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8048f68261b2fdcd0cc93bbe51dd77df8e43b57c3da698cc1c679e192bf4360`  
		Last Modified: Wed, 21 Dec 2022 05:08:00 GMT  
		Size: 12.1 MB (12130299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:497cc8982890eab597c6d34bdad7c65b903ffb329fc1dd479748adab4dcd7558
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65240087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb5da4fd1d86a7ef3a37f0981a23b5ed7a1ac32ca8221d418dafceb3054feee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:21 GMT
ADD file:ce5483e7a7d6e8eae2ec1f1c22390523d24dd0e613a20f8d424c81a1e12240ab in / 
# Wed, 21 Dec 2022 01:10:24 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:05:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec8e0a8db89be83ab5fa46e2a3ecb60ab7e5df3621c585c4ae748c563af17385`  
		Last Modified: Wed, 21 Dec 2022 01:26:34 GMT  
		Size: 46.5 MB (46453589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f8c6e126b4271f9c21a1890d7345d3a741f26baa2d58b1c871c87435c0d4b8`  
		Last Modified: Wed, 21 Dec 2022 02:33:08 GMT  
		Size: 8.1 MB (8052896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45d51aafdd462331d0b5b67c93150c348af9265261f8e51be63ebd57302f9d4`  
		Last Modified: Wed, 21 Dec 2022 02:33:09 GMT  
		Size: 10.7 MB (10733602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:501736616e0043817cc4266704e1b2ea46d71785a8fcc91c5cc9cad0daf2f524
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67315403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5deaf1b7f5262a80b1874b26dbc773337e201a6f1f0d4db98eecb9977d8a5f62`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:22:39 GMT
ADD file:603b8f38f314737d8b96d7fa7c31b4c6ede8fec5c46d30621085354a718b7cf6 in / 
# Wed, 11 Jan 2023 02:22:43 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:50:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:50:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63d179f68a4d4f8c050f7c24ec5c73831d75b928d359ddbbf2e658360463fd13`  
		Last Modified: Wed, 11 Jan 2023 02:27:08 GMT  
		Size: 47.4 MB (47434084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8ad9595a7cc2a79974880bde3167e302536eaeca227adc959cfa976ef5c29a`  
		Last Modified: Wed, 11 Jan 2023 02:57:32 GMT  
		Size: 8.7 MB (8665726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53049c87c88bc24602f77d08379e056c3032ef773e4e1b619f0f1b543464ab90`  
		Last Modified: Wed, 11 Jan 2023 02:57:32 GMT  
		Size: 11.2 MB (11215593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
