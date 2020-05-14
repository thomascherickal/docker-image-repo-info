## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:1f533b7d4d0552064264b74bd51b234a14c67aadf3e63baeab37eefe1f977de5
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
$ docker pull buildpack-deps@sha256:0d091a640cc1e374470727012ab470f2518a17039ba3f5e62acc0f157b9e55d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67031426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97fc8fe807bee3997224776a430b4b98cac1b793f1a9277ede2a84914e69988`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:53:19 GMT
ADD file:b96a79161ef28394a61231962b6b094cc6d55101ffa9e159bca48da52498c02f in / 
# Wed, 13 May 2020 21:53:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e01d6f3a75b2bb37376867eda5418ce8818270da85f9e637bc0f8131b3c49c32`  
		Last Modified: Wed, 13 May 2020 22:01:43 GMT  
		Size: 49.4 MB (49359537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4060fe458be3ad9bb5734b9386b2be633e551438da5fa5933a3caf2eef1d3084`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 7.5 MB (7514215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e846164403fa17ac3349dfde468323e0107f2f131933333cec4baa962c230c`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 10.2 MB (10157674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cdff372dea60632cb5d4bd7de46f5a8dd8bb5684eb7d96a0d0f20291eb89bffe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64222884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b61031a71df91f240e9b972a9307b59454781d0708a8766af45cdce628f22066`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:17:11 GMT
ADD file:5c1bf8e876f6ffb8a54374fd8f26d78a98dea1fae6787eb5fc225b65db262397 in / 
# Wed, 13 May 2020 21:17:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:06:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bc0a6102c512ac7a18c58c8bfeb98c10b25edd28979b9a105af510e9c56fd786`  
		Last Modified: Wed, 13 May 2020 21:27:04 GMT  
		Size: 47.2 MB (47161205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f603ac474016e66e34904c06b4aec33100f42c805573cd91e60bfa44fff303c`  
		Last Modified: Thu, 14 May 2020 00:22:44 GMT  
		Size: 7.3 MB (7257035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd00f44c97780ed4c8b26dc3d2908006e596311de54a3c167ea77feaf1dc80a`  
		Last Modified: Thu, 14 May 2020 00:22:44 GMT  
		Size: 9.8 MB (9804644 bytes)  
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
$ docker pull buildpack-deps@sha256:d3d5c5e8ee64e74abea0d9c1a2ff45254bc1c0120f892fc48b6aca71be17f0e9
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68077802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae4eacbbe827a8165b80c07dce4889cd904a8cd18b24dece7ce0082578e0822`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:50:21 GMT
ADD file:414f2e62e00cdfce0e28fe63b849f1edf12ec34ca7cfb09a08a2b45e2a5cbccf in / 
# Wed, 13 May 2020 22:50:22 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:01:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:01:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80f0b2fda6b50bded03a482e7f73f99daa6b715b932d0253f4c3054be1410241`  
		Last Modified: Wed, 13 May 2020 22:59:52 GMT  
		Size: 50.1 MB (50132193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc04cfdc11b752ee43412d0778b055107628b6cd534fb814336f68aab3c695f4`  
		Last Modified: Thu, 14 May 2020 00:19:44 GMT  
		Size: 7.5 MB (7460878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387d9d2e6037ae9b70690a8e4c4191c3d98d50f37419a122cf4cc9084fa2b873`  
		Last Modified: Thu, 14 May 2020 00:19:45 GMT  
		Size: 10.5 MB (10484731 bytes)  
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
$ docker pull buildpack-deps@sha256:95f5b91444303d8b899095d6f186cbde141ec9c0537423d1ac356d609ac2d27a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67950446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded36e8ce611c3ae7faac0b67201c1716cef3b86da33c47007f6390171e14d8c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:22 GMT
ADD file:e7473e4f1acf1308ed319dfcc667696c733d4173125423a8f1b2c67039e5f498 in / 
# Wed, 13 May 2020 21:43:24 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:42:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:42:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:23e07cfb1ab58da76b3f9f0fdc8f5c154643a262a86037b7b6d1c26b5959a166`  
		Last Modified: Wed, 13 May 2020 21:47:43 GMT  
		Size: 50.0 MB (50002084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e62641450b73095b82a741ceaf6d58012156b7f78bf4f67b73575fb15b7a03`  
		Last Modified: Wed, 13 May 2020 22:49:18 GMT  
		Size: 7.6 MB (7600546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f55d4f91dc718f22796b06fd0faf568f26113eb77e940c765216272c8262472`  
		Last Modified: Wed, 13 May 2020 22:49:24 GMT  
		Size: 10.3 MB (10347816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
