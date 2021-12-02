## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:ec07fe521db0b2538041a99dfe7d04c04076f7b55f346ffbb6b18da990c2df71
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f28d2d6e1776233ab20d37c9192876ae2b354e6eb27b5e358eea942fdb4a3487
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128650506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5180d8eb28afc4cb0431784c7876ee583d6a4b54ddd7803124e57b3c3b914f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:37 GMT
ADD file:aa0a8871e20fb4e68758bdebe7ee1e99e982c5e9d2e97b73575b8dcc2ab4adf8 in / 
# Thu, 02 Dec 2021 02:49:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:43:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:43:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:43:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af46a953975205f2d7320842b5338767ad3d4aa084267279fc21cdc807374c52`  
		Last Modified: Thu, 02 Dec 2021 02:56:05 GMT  
		Size: 55.7 MB (55746868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923af8c82d6eb6585aa625d753ea67606bccd40758565b49eb6e0636c4281a9a`  
		Last Modified: Thu, 02 Dec 2021 03:51:55 GMT  
		Size: 5.3 MB (5276824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c97b84d4ef8d40d6b16c75023fa3aa650861e59f1151d2ab44e9643bfa121be`  
		Last Modified: Thu, 02 Dec 2021 03:51:55 GMT  
		Size: 10.9 MB (10904313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80321460c0114c02492753431792e6c46ac3fe9b80600356543e3068ed7a067`  
		Last Modified: Thu, 02 Dec 2021 03:52:14 GMT  
		Size: 56.7 MB (56722501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1783730181df97e59f6d8c14c4276b564fa279a7cb98e0e5021369e5b757d2c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123402292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7829c469a1887981bb88d9005cdec6b84bccabaf5e6dc2e698490175ca7aa080`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:54:44 GMT
ADD file:358278336204ee1e51bf00f8c88d281c73e7e5d5b537fca1ddea89c9e69da90e in / 
# Thu, 02 Dec 2021 02:54:45 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:47:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:47:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:48:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92d580f40fe8bf02becf360f6a4dc76454bfd66964c4acc0ddcd113fa0e9c2d1`  
		Last Modified: Thu, 02 Dec 2021 03:13:27 GMT  
		Size: 53.2 MB (53226256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638194516b96610900042221009a8c126b7644c26fe612397f2b2622bdfd03ac`  
		Last Modified: Thu, 02 Dec 2021 04:04:39 GMT  
		Size: 5.2 MB (5180320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b2f3d24644f1e0eec33ec3662f820a19dc6b8cfa47e1f1551776f80f739780`  
		Last Modified: Thu, 02 Dec 2021 04:04:41 GMT  
		Size: 10.6 MB (10611050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced16911b039c1097a2b138cf1e729c67a19c941b575a03dee7c08a1c42d3e6f`  
		Last Modified: Thu, 02 Dec 2021 04:05:17 GMT  
		Size: 54.4 MB (54384666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e25517d9e4d5c71b0fd71f8672be17b1407629cf364b7b4c875a48dd1572d1d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118543731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22e7df05fd0bffeca4c0755b5570159b2a6f9ae77bca4317c40c4257b7e6e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3057f63e28cc1fe4f0dd11039577f14ac057f713e42e2b2e13000b37b8b86967
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127533393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4bbe255f47709b63ebef085398bae156c616dc66fa9f1980c105e345911141a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cab4dc0eb95cf2e9a2e2a5f77eca7d76108730f09e1e205c09465b4fa35934`  
		Last Modified: Wed, 17 Nov 2021 13:39:12 GMT  
		Size: 56.0 MB (55987448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1d02882df3820d09283a729b38d8ae0d4682ec62fdd19537ec3f6cced97b426a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131641845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374268d5a1c98546987f58c5ff168fe7be3e3eea1e2be170cbcccc6f2273ab29`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:41:35 GMT
ADD file:166234c060754022c10737b949088caccb46aa6315aa91f9ff63dd1f60704729 in / 
# Thu, 02 Dec 2021 02:41:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:14:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:15:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:158718d3425b2eb9ceb4c5321a7633c30d7b948b7dfe2a98608b354788b1c2ab`  
		Last Modified: Thu, 02 Dec 2021 02:51:07 GMT  
		Size: 56.8 MB (56808054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fe1b108338e18a41ef0392f3153179fc4c7809ae0d46bd4c0ad04d928fa2ca`  
		Last Modified: Thu, 02 Dec 2021 03:23:43 GMT  
		Size: 5.4 MB (5408797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360266616da2d6b21d216fa2104faaa2528b4c353538e2fc67ab8b0942e7f3fc`  
		Last Modified: Thu, 02 Dec 2021 03:23:44 GMT  
		Size: 11.3 MB (11285984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99c83bcfec09f5a8285a2c904ff5ebadbe779a1888d98acbc22ff42f814c916`  
		Last Modified: Thu, 02 Dec 2021 03:24:10 GMT  
		Size: 58.1 MB (58139010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:277451baec3ac7c41ff286c5d4bf89c602eb089f8ec4b24e96281dac4cea121f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b49a0d880ec3185395fff15df7416540f343c3c377be897de3965fb23c1cfd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476b323dda6fd93fbb86e98139e76c07bff3f2d7a4b07b087d8e2c114b346f2`  
		Last Modified: Wed, 17 Nov 2021 08:52:57 GMT  
		Size: 54.7 MB (54724326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8262acfa4cec540a727499b029781e6d9a768c80567ef0a550cc50eb38db0b5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138527990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70616a1063b2854769c53da57f912b1b4adb02a65b34be74ac6b6749e1606f88`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 08:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16114ff6b100453ae456bca4961ed144a5cd72589c05128a5b44f063feab7bb`  
		Last Modified: Wed, 17 Nov 2021 08:32:21 GMT  
		Size: 60.4 MB (60400057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8486f624b42b956b1401a5bd240b03ad282ea1e54edb5242ea846893478a20ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119790274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b441fc86b4e2662aeadd8e308872b18de076f1c73c976e045a69988dcff041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8e5535d8b76c576ccc669d4f642fe2ed78be80df9778331222b1c87425845db7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126169798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6223c90d2c69ea15d0c2c6ca6033b860ee5f424c5d543919e86bc305d827047e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
