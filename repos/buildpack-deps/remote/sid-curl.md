## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:6463790dfba81cd3e402aaf57f68e2fd6ffa49a1d69d098f4b77102c4809758b
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9b20c5a55ac15095f95ed1da0773811ea9a0dbb041a5b8d1a839ef2c5ed25d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70027528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91ef20525f2e3a5ae857d73e288591b2275f389c3f6f7dd5463b3c74e6de48d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:28 GMT
ADD file:49aaad883f9932e76df5604c9353bdbc51cd2c74b986b57b2dbb4f3aeaa46404 in / 
# Tue, 09 Jun 2020 01:22:28 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:54:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:54:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:516091449b2853b301713d61c7a73bfbe7ae63ace598e76e1d5e9da246f88b37`  
		Last Modified: Tue, 09 Jun 2020 01:27:16 GMT  
		Size: 51.5 MB (51526780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3385de445fd2842a13718698d3fa721fdd723aaede5f9cc079f9bc763e815830`  
		Last Modified: Tue, 09 Jun 2020 02:01:38 GMT  
		Size: 7.9 MB (7920994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd8a6c64c26854ad6d393a2096bb413e86391dc5861cc5a961eb2c55eaa1f63`  
		Last Modified: Tue, 09 Jun 2020 02:01:40 GMT  
		Size: 10.6 MB (10579754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:30a749f4c7f66da5e6f31da95d9ee9f68956d4581a5cf2950d6f3cce00ceb241
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67271752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59c6340d3ea8789957913f23e11bccf5b0bfb6c1522ec5858883bd7e3789d67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:54:09 GMT
ADD file:333f6925c41655ef86c1c55aa4628d69f324c5f263e27174c329a670a7408728 in / 
# Tue, 09 Jun 2020 00:54:11 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:40:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e514d65a1f93d9b21040cfb52628de87401493f0b2eb92f1a22c9d381f15df3b`  
		Last Modified: Tue, 09 Jun 2020 01:01:40 GMT  
		Size: 49.5 MB (49505780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95254689f8f0bf61ba2fb5802bcfd31293fb3a56d7c3ee6b7653d100b6e62f`  
		Last Modified: Tue, 09 Jun 2020 02:00:49 GMT  
		Size: 7.5 MB (7500859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e156bd6d1d602264fe07ee2e4da6116f3627a0cdcb05d3f8452ab7e6a15fc5`  
		Last Modified: Tue, 09 Jun 2020 02:00:50 GMT  
		Size: 10.3 MB (10265113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f7067e3e95b49d917f577be3658080b7a86d40a09a0c6b3f474f9b39739e229b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64486247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7dd9f276027b2fe04cb5552ec0d96dca729665892678f6779b4614fd121476`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:04:25 GMT
ADD file:f137ab200a6655933430876a9a0f3c675ed39dbf4a73be4750579b0c66812888 in / 
# Tue, 09 Jun 2020 01:04:32 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:58:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:369ddd165e2326d11cacb52bac2afd8d2277bc9506399fb693a5a5eb336716ee`  
		Last Modified: Tue, 09 Jun 2020 01:12:30 GMT  
		Size: 47.3 MB (47326325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ada3ce7a1b468f31af8a1aa9f083d4521fbeedd0d46757dc5d1f97c49ebf17`  
		Last Modified: Tue, 09 Jun 2020 02:13:48 GMT  
		Size: 7.2 MB (7243269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab399397acddc3f7ce3a847871519a272a15f91ee26bd786a485bf8a41dc870`  
		Last Modified: Tue, 09 Jun 2020 02:13:50 GMT  
		Size: 9.9 MB (9916653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ef3f5f56f817c5d25d77487c7c1d9d4c162c669859352c850647ae78ee66f225
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68875617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccbd804121e69fe6792eacae4ef4729afcd92c9f3e2658386599769e0320eee0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:53:03 GMT
ADD file:56e3fbb5c1d0a4c301b36e4f85f596b26f32562da8ed0a704496f1e3ca5c676a in / 
# Tue, 09 Jun 2020 01:53:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:35:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f925f2558464755f2d5e30c33f6f9072851b0da5fb44204c52fcecdfb3bfbb44`  
		Last Modified: Tue, 09 Jun 2020 01:59:06 GMT  
		Size: 50.5 MB (50491571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b751eeb6110560d41a2af99cdea392104b87433a0ba6fd41a17872f77369f134`  
		Last Modified: Tue, 09 Jun 2020 02:48:52 GMT  
		Size: 7.8 MB (7795590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f1451ccb4e8af4e45ad26e876fb36dc52c07dd21d5c4b226f8ac6a9407fba`  
		Last Modified: Tue, 09 Jun 2020 02:48:51 GMT  
		Size: 10.6 MB (10588456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b48f5a94b0a7c8a3ba287d786a4222d29c1e1f6de749a39fd037efaa3fa406f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71704413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc17b2d4da31a481be444dd42f5fb8b471d92b25885d3a3701e1e3b820d79ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:41:24 GMT
ADD file:e46d18aaa3cf0eb6320c1b26b025ee8fbec78b2c4e4b3f5d4343393f1cbc769b in / 
# Tue, 09 Jun 2020 01:41:24 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:23:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:24:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c73d5896f1a36fe56b17fa2ffd2771c0b97b78e1b086e696cfa14b05618bbeee`  
		Last Modified: Tue, 09 Jun 2020 01:47:08 GMT  
		Size: 52.6 MB (52644936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf148f44d6df7cce1b2964667971df2c24df9d24505794d9324b303eff4da0b`  
		Last Modified: Tue, 09 Jun 2020 02:35:07 GMT  
		Size: 8.1 MB (8099472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8c598f01778284c7219a5d6e3853bc2247c68a8e1ce0851af567867177c31`  
		Last Modified: Tue, 09 Jun 2020 02:35:07 GMT  
		Size: 11.0 MB (10960005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1b964419cf8dba4f97a895e3ea6a592442853ae0304ef3d6d8e89051ef550d6e
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68311260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39beed23589f41c91a82b8b807081bef8913fcd8fb5bbc9fd25f3d2e34bdc67a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:11:18 GMT
ADD file:2c0e5d72dc26223a4df660e91acd4c8c70d1b0ee1139c92fb9cb3f041d81bdc2 in / 
# Tue, 09 Jun 2020 01:11:19 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:78e0a34f3ecd34b89d20cdb0b915427acd1691184f4f7649f816759737ddb842`  
		Last Modified: Tue, 09 Jun 2020 01:20:19 GMT  
		Size: 50.3 MB (50264875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff174bb9582ec89056fe600d1820b6c6e7445d74e52537dfea39a4dd2b4324e`  
		Last Modified: Tue, 09 Jun 2020 02:14:03 GMT  
		Size: 7.4 MB (7447530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a44807d6533dba987e8712d4b69466283e5bbe760298ac86ccbe1ed4ea542e2`  
		Last Modified: Tue, 09 Jun 2020 02:14:05 GMT  
		Size: 10.6 MB (10598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d6c6d200180963ddc10c1e148b62498d55d704cd945044d16849b8d1aca5f7ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74645356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f9edb49829b37593278b5b0c36ceb8880094cf358b2109d89ce7fce0c81396`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:28:26 GMT
ADD file:7e16c349b13e97e4784ee396bb36ab2d3a069714388b0803f18ceb8d526be36a in / 
# Wed, 13 May 2020 22:28:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:55:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2aad5ee0ac7c9bdb0530f0a2f94bcadce58437453bcbdc7a2f20b5366c22799`  
		Last Modified: Wed, 13 May 2020 22:59:47 GMT  
		Size: 55.1 MB (55111830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb4a67eb9efabb0bee7a8a6ff0c8c5d8b09a6992b8574669e941eb06ffe22d`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 8.4 MB (8356775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba850bd6d1e4314d0d2953223c98e2452ff03935b42d421bbd2d54ca027da5f4`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 11.2 MB (11176751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3ccb66729103c49d34b86d7529a88391567ef68064d72f11d6197c45e179463a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68201650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9804b2b0d19ed6d712fa840a7b4c5371d431ef6757b7107a1a6875a0c0628802`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:43:14 GMT
ADD file:f1ebbcfe99a36749cfce4bf2c38aff7e5a06ff0eee49c1c44970cb518d59c6c1 in / 
# Tue, 09 Jun 2020 01:43:17 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:68d68a3a62e23bc275e3488ccf04bd3d9cf392e7f00f7ac29a6f1d74be8ec63f`  
		Last Modified: Tue, 09 Jun 2020 01:47:06 GMT  
		Size: 50.2 MB (50155657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69552bf02d312240efc0fa7fe7d03054f5a709076df8a08878cd0782b3cac8b`  
		Last Modified: Tue, 09 Jun 2020 02:18:53 GMT  
		Size: 7.6 MB (7589963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77d73b4136a153380a7e5348a698053b0ee98f961fe50d20e65ca30de8da8d`  
		Last Modified: Tue, 09 Jun 2020 02:18:53 GMT  
		Size: 10.5 MB (10456030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
