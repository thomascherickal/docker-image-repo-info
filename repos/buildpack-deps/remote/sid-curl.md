## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:d73594bc7e05039d42fa3ad9c5b2daabadc46b38fafe9e9e545616f582643259
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
$ docker pull buildpack-deps@sha256:cc22c156446c9313c4680623e26c6e48bba2f98ec6ce87c8ed3a0d52e716c0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73367169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8c38f75980c2def43a2d61e770ccc0b3c9955ae57c722bb79d7f977a21e31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:59:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda17d2d1d2961ba6c7083d3013dde5fb5af68bd80ee1e40adbf7886b64df3c`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 9.3 MB (9300772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d617f2e2db52d55fec066a28a409d69e1dc40dd9f91f7f03c19ec8d16c587`  
		Last Modified: Wed, 05 Oct 2022 01:21:27 GMT  
		Size: 11.4 MB (11382118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:003e17008ddaf3d07c54f0e22bf1740953332445e88af588740603583bd313ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68957196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735e2d1a8b82054ce8ae48afcdbd6e7bd00b34f6107e66adc81d2023c1a0c787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:50 GMT
ADD file:829f8e96e527611e85aa710b19c01c75a4760a27c651fb439f8cdb5609db64aa in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:513ea4862e78a8cc07ed6d320f10e746ca770eb039dec1548c31a9de19d1f7ce`  
		Last Modified: Tue, 25 Oct 2022 03:12:19 GMT  
		Size: 49.6 MB (49578888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ace4b71d48c3105e8f55674a41898f6b1df73d7ee8b05d5c3d3b3fea66077`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 8.5 MB (8548544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ee02803cd3666baa3051b15b273e86d1d20710ddd79191fb1367a0dda5edc`  
		Last Modified: Tue, 25 Oct 2022 06:20:29 GMT  
		Size: 10.8 MB (10829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67e81d32e4a379ebc001840f12d827e5f67833629cc8d825dc7e62681fdec972
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead5cdfb9f5e5c275759c55be9d11eb1dc155f3aa55dad5b5be0cb66efd70376`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:38:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00270159c4caaec159e25e1eaca6209b11c838dd60b5e0f5194e2279c51cd70`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 8.4 MB (8399366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8524fd9b0e923155334b98a655b41aa941eb210e3248b7cc375ee49257b2b929`  
		Last Modified: Wed, 05 Oct 2022 00:56:26 GMT  
		Size: 10.7 MB (10663790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0fa7918450dd9fe388abd5681d138ceac42806881b9f01ab9773a5a6cfce977
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70715689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d50f6af0113bc54f7f717b62c4be946ce8984d31d0e202389ef84720e47a647`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:29 GMT
ADD file:6a2d69a5a731490271c915d99634a89755f7236ef56712924ea061730d8552c4 in / 
# Tue, 25 Oct 2022 05:46:30 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:01:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63a396bb133ce57141398b6c6d776ce17e3e973085b5a1b746d76407240a376a`  
		Last Modified: Tue, 25 Oct 2022 05:50:38 GMT  
		Size: 50.6 MB (50643735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89cf1bf3c8da06b08672e8551d2511df312e843fb3acab24e31d9ba0afa866`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 8.9 MB (8932959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e653e6dd7e514d68792b5ac0d2812dbc50a0e1d5c4842fd356c767031c54aec`  
		Last Modified: Tue, 25 Oct 2022 08:32:19 GMT  
		Size: 11.1 MB (11138995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7a92edc5d0d1d9b005fc402881b8f8eddac8e13c8f5adf57fb62e1a26d00983d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72287451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1893a81cbf84a850be47ff4f28e1dd4035b9c2256bdedf86584fb4079c771d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:38 GMT
ADD file:80dabb60a37b1d88f3750adb85c9e159d00b55293f70ad93512f94bd3cfd99bc in / 
# Tue, 25 Oct 2022 02:23:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:18:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:367799113badd94b9683087d6086436649a1fb7127698c42b0d730f5bbedcf86`  
		Last Modified: Tue, 25 Oct 2022 02:30:22 GMT  
		Size: 51.6 MB (51625321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2fccc59969c0b37e3bb8384bc6545a4cce125daa11c7e8b599ec0acac788`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 9.3 MB (9282393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9213196e288bdcccf553107591d6fe4f04fccea4da55faea35dd79cfff15`  
		Last Modified: Tue, 25 Oct 2022 05:30:00 GMT  
		Size: 11.4 MB (11379737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:177c731ad458bb98287f9b7f0ff300408fc1a53c32e1d406bb638c4c00719d21
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d48d0070c45b656746927bfe7b8ec4a82c7b00acdd9cce150d2c20e17feb87`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6422d53934b53541883e4d8479c0384974a4f8c2ca335b2e86b900b4cf761d7d`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 8.7 MB (8665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd86c88bcf963ae10ae57261059a1b2bdbad2590061f63513acf0308dacf1`  
		Last Modified: Wed, 05 Oct 2022 01:35:18 GMT  
		Size: 11.1 MB (11130537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:124e076bd786711b687044fd136c24af7bc4500c1e67e6e1f0f4086eedfced08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76327268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce644126cccec0395c556b7c4763b65ccbe0344029fc1fc5a5a1c93e9d1c4787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:07 GMT
ADD file:6e9efd6bb77c835520332c88cb412f38f0d8573ec3347b090b77965e17131780 in / 
# Tue, 25 Oct 2022 03:14:10 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a3962f6ac5b86fa159789ea1e9241ecbb956b3223e8312f7d92d7fbb8bf5485`  
		Last Modified: Tue, 25 Oct 2022 03:20:03 GMT  
		Size: 54.7 MB (54704717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c5225e6c97e35e08afc065bed0fb4156a1727da9a3e12b4a611189682c919a`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 9.7 MB (9684744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fe7c3b495d9320ca99478bfddf7a3fa0412a37c56ca95a4cc891ceb738e62`  
		Last Modified: Tue, 25 Oct 2022 06:50:49 GMT  
		Size: 11.9 MB (11937807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:91c41397454a62656ddc234f54c6ce9bc6eebb7463198b379aec9760ef9f5ce3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67996548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c82f669a88d6376397cb790855001ce2a2328184d9fc8f1fbf316b588cd40e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:459e259ac9d973e273d44f4977a901a7c57dce7f749c5caf0ade7837350bf940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68792946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8919e63d46a3758bb8046627e26a7d852ed8e26e8b044f56948b519863d33fd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:32:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67452e329e71787509a1583923b8e1e83b22a2fb76e48111393a03205d4c20`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 8.7 MB (8738304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7be163526b121ed701b3595b33b6d8755aba04a12b0fd801f9c899cbd3ebd0`  
		Last Modified: Tue, 25 Oct 2022 02:50:30 GMT  
		Size: 11.0 MB (11041665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
