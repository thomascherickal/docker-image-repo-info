## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:11f41e6686d08ad9578447f4b15f5a5a666ba5c456c52a2604fa15bf799d1cee
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
$ docker pull buildpack-deps@sha256:8f65a6ef88aa3e7772ffb6a4385f8cbd5d410c47d0d5b63af8a42f5bf228f98f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69788376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06bba400b0ce9a3e4a0d0f55ee9e42334b1e39c13575c1e26d82ab753a96e981`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:22:30 GMT
ADD file:1b99a100214a4a86a413bf6a826c70d07fee06a8c4e6d1f3ed1550fb08f9818e in / 
# Wed, 13 May 2020 21:22:30 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:268c82fb25093fc20c25872a9f96ca2bef121a19a81a91079b62afb96b725135`  
		Last Modified: Wed, 13 May 2020 21:28:35 GMT  
		Size: 51.4 MB (51390987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a426d8c659d27b64d66f82bd62c2bb3dccd6560447f354396111cb0c27bc0e8f`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 7.9 MB (7934296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac7ef969a4b66cfe2e8dae9867620b1821ab5b3d64e9e37b0a3ca56f574a44`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 10.5 MB (10463093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:48010584ff634e5dd031f11b9811df3edb0cdde6eb98eb8774d1dfef8b32ff47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67044807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2095f210a201cb48655cef01f70bcc2c419b92e1781176c6cf8e1dc15af4c1e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:40:47 GMT
ADD file:c2ef493946404baae91412a79e2336f831835f471608b615f053cc8cc1c1cb62 in / 
# Thu, 14 May 2020 22:40:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:53:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d6200ebef6b4ed212e54012a0718d6122f96033e0dbe7fd95e64d7739c61b3f`  
		Last Modified: Thu, 14 May 2020 22:49:25 GMT  
		Size: 49.4 MB (49372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e62f5ec2c655eec6bc82424f1d1705ab9a002004800db4b3d6d52fd101c1f6`  
		Last Modified: Fri, 15 May 2020 04:04:43 GMT  
		Size: 7.5 MB (7514186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282c779adbdc0e96ca8947af087a331e91a4c580e8c0092a57044a79a102cebd`  
		Last Modified: Fri, 15 May 2020 04:04:43 GMT  
		Size: 10.2 MB (10157673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fb52536da9993b9f83335f4b3af3c3847db5217d2696300f6826e97fc8b1c4c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64240900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd472cabe9b837610ff2d854dcd2825da533779955051e29e426e27c96fdca8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:04:08 GMT
ADD file:7bc7b5e94debaef8aabee3128de6e535c9867794ed42649aadb9ba63a66a547b in / 
# Fri, 15 May 2020 01:04:11 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:44:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:921baaddbf45818850d057b247e93c5fa875838ac2dbf11e2913f526f5ac4d94`  
		Last Modified: Fri, 15 May 2020 01:13:34 GMT  
		Size: 47.2 MB (47179178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b833ddc7c9debd21799cd19fb7e5459feeaae463d767cea9ca2c02209d4e68`  
		Last Modified: Fri, 15 May 2020 10:59:56 GMT  
		Size: 7.3 MB (7257028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dd78efb72e462bafeddbe0df6aa29d83c9f987bcd797c2d1cb8c813c1bc59`  
		Last Modified: Fri, 15 May 2020 10:59:57 GMT  
		Size: 9.8 MB (9804694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e443b8076af21f2947052a1ac4a8a3fbdfe55f69838f26dcfde385af60b9d02a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68597978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f3d08d69787a0d416333a76c2fdddc0c7e4fe6267e4a9b2905628720340554`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:45:26 GMT
ADD file:22517e10f0b5d2760fafa2367b5a187d7ecef96291f15a746c24bfa50f756219 in / 
# Wed, 13 May 2020 21:45:29 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:27:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:28:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ad0025dc69d6f0241b2f5b614e96cef6e1fd54c9ef07b726338235b4766714ea`  
		Last Modified: Wed, 13 May 2020 21:54:40 GMT  
		Size: 50.3 MB (50328664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de8e099b34fe681d2134dc5800a33dcf2d66893cc852ada1704e600b8e46fac`  
		Last Modified: Wed, 13 May 2020 22:41:03 GMT  
		Size: 7.8 MB (7809465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2735cc8b188a094edcf282e931946b14d50022e973d985f72d13b23f3a1a810`  
		Last Modified: Wed, 13 May 2020 22:41:04 GMT  
		Size: 10.5 MB (10459849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:92c974fa29739fa627912d437fe3a68f9fda55e604603e620afa7b92e28a4f1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71434957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d4581e0bcd1da9a4e4b23669a0d96ab8686e7e3a51e8dd791f5f2c70ab5f724`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:18 GMT
ADD file:bbf57f6406dcdfbee8d207ada2ed9150a3e775fa2cb6e0784c3e35e1c3216d25 in / 
# Wed, 13 May 2020 21:41:18 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:54:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:430f489239f0254d72f3974fb8f614ac80ef76f642ab0bddcc4f20a8d4a3c68e`  
		Last Modified: Wed, 13 May 2020 21:48:41 GMT  
		Size: 52.5 MB (52481574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65cdd6becdc738c09b87ead3f88dbd9e0a0028929d1d7f9698c406b2edfafa`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 8.1 MB (8112129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2540c9f9f0836e2023dc2dff06e7a2a5186841f2f2f6bc12a2a1a2e05d7fa7a`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 10.8 MB (10841254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5e384e37689f7449a3c3816596a713eb1361da3875b79a0490bd25f4592798cb
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68094559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4924c843b78f7d6104f05f18fe2e06bd72e4e1fa4e56d4c24ad42640670604`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:49:44 GMT
ADD file:2c7c92015da849bc75eb25960609c90178c9ac455dab05aa4ef031806d26ad64 in / 
# Fri, 15 May 2020 04:49:45 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:41:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:41:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:567e61b8ab78e586542d5b9fab62c3880de99927de482a73e9e8b5b304f5284c`  
		Last Modified: Fri, 15 May 2020 04:59:15 GMT  
		Size: 50.1 MB (50149003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171157d3bf1886098a7c08bef7ab08c3c7a0d9b292111e8a5b8f39eecf07c2eb`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 7.5 MB (7460868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093eefc9c96bf46513b1575ab2e19b673a8a64043aca4e9ae4db05a4c7f3e803`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 10.5 MB (10484688 bytes)  
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
$ docker pull buildpack-deps@sha256:2ae33da38147da3e4ad67990929f8bcc0dfaa77409a8a2a5b8c2baf4893f2955
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67957365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1e9c0383ce7b2a7da60bc270c6035661a53f084ee61793995258d7db00146b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:07:25 GMT
ADD file:e200f47e248587a66670fcf47316228d04373cff77498412eb3cc5d6a1ec50a5 in / 
# Thu, 14 May 2020 23:07:27 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:02:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11b5223327afa0d65cbb885c5383c894bdfd11269c346392cfb8a39f81aabaeb`  
		Last Modified: Thu, 14 May 2020 23:12:06 GMT  
		Size: 50.0 MB (50008939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcaa68d7c0d7853692ccebd673ff13ab4103a32fa894d7f1519715d3fb63578`  
		Last Modified: Fri, 15 May 2020 05:09:57 GMT  
		Size: 7.6 MB (7600688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112c6cf752bfa2d00b26e941e53dbde668d81bd2884edd4dd74954197be2a175`  
		Last Modified: Fri, 15 May 2020 05:10:04 GMT  
		Size: 10.3 MB (10347738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
