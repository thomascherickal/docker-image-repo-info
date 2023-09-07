## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:0d483dfb1c0e94fb40d737281bf300aea460e0fe8c7693af1ae60c6792799309
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

### `buildpack-deps:trixie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:53ca813178bc4fa62af963c4528dc066b3c4bb62125333bf9c8d04a789b45f96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69769550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc8643019ad3a77b64fcfb7b8151d2536d3f9a70cda00b7b6f8c5ff4a742608`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:27 GMT
ADD file:34ee641d9bad402a9422c8f96269ac2c74e06369bc362a916c8cdb087156bf70 in / 
# Thu, 07 Sep 2023 00:23:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:02:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e32a7bcba7c1847ff42b03e176da563d6447b045a6f2d5a9ece6acdce60297cc`  
		Last Modified: Thu, 07 Sep 2023 00:30:28 GMT  
		Size: 49.5 MB (49514761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df261e695bd837ce65c269e99eb1a12049f82c345fa073f411be6c5b6d7d3b75`  
		Last Modified: Thu, 07 Sep 2023 03:09:01 GMT  
		Size: 20.3 MB (20254789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c0849926a45b2c03c11a9782b7bddc34172517e4e92a0c683616566fc8b8e8a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67645396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2618e8d298d5ab31281cdeb2f17c60c23978b45a81b1b043b045f2500200a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:56 GMT
ADD file:d0da838ea8ff64a44e445dfb0001a4f6a2442085f0c0f942d0129b6f8054c7fa in / 
# Tue, 15 Aug 2023 23:49:56 GMT
CMD ["bash"]
# Sat, 26 Aug 2023 01:57:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6d8f24fa9802404161e1d0ef0d1db6d5f4c20cb1f0e5884dd191e1d77f2373c`  
		Last Modified: Tue, 15 Aug 2023 23:54:43 GMT  
		Size: 47.4 MB (47395127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f867d323ed66972b6c492120ce3fa78d7e1d63e0279362a9a55229db8e7127`  
		Last Modified: Sat, 26 Aug 2023 02:00:38 GMT  
		Size: 20.3 MB (20250269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40e5a63fdcdff1779a4e79a41d07552b87d4338d098a499fcd5efda863fc055b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63611435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d08b2937efada250c8ac1f721e401fc1621ac8e264bff2f523fefe7cc7fadb9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe3001385a2b717c083b0eb81363b8210958afe6ccf0dfe6a62a78df022ec5`  
		Last Modified: Thu, 07 Sep 2023 01:49:25 GMT  
		Size: 18.6 MB (18600941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:07a6298feb693f4d212aead137b90806a90e5224731919ae7fd085593fdd52f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69560118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83daf480e727a68a12ae06eac0e0ce21b12c83090213b1f8505f30b8ada3554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:42 GMT
ADD file:16621389c05de9ece6b8d40e6c62ca81465940296cc58f7f1c56571fac05b33e in / 
# Tue, 15 Aug 2023 23:41:43 GMT
CMD ["bash"]
# Sat, 26 Aug 2023 02:57:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5fc9f67522f8eb1fc65844ccc91e1d93595f85d410842d334c85f7e0a15d841`  
		Last Modified: Tue, 15 Aug 2023 23:47:22 GMT  
		Size: 49.5 MB (49521978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c849b78c27f87cf11f7bfc3a6c274880955ddcf718ceae8fe425a331d69fb`  
		Last Modified: Sat, 26 Aug 2023 02:59:50 GMT  
		Size: 20.0 MB (20038140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae903244a0a7c407c348c787c1d71a807c2c4967fd0fea7cb34ed756fbb45ea9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71458433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75af6cb3cd46b8071500f06c320433c0fabeeb760fc4d382feac7d689b378466`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:32 GMT
ADD file:4d14eb57255656e664c93bdd44713aab3556f53199d3002e8b099b8a4f99ee66 in / 
# Tue, 15 Aug 2023 23:41:33 GMT
CMD ["bash"]
# Sat, 26 Aug 2023 05:50:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92cb61533d6d73bc90b946ae69c5db6942d13512056cb4f565d14697cd7aa909`  
		Last Modified: Tue, 15 Aug 2023 23:48:22 GMT  
		Size: 50.6 MB (50618535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb29c4acf204aca1bac764fe7dc16e996b09849724a7e8aa9f0ad59c78a11e75`  
		Last Modified: Sat, 26 Aug 2023 05:53:36 GMT  
		Size: 20.8 MB (20839898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:04ebc787bfae1cb8856d0445bb8aaab8b9c5f96ab37fd3fd42869ccdf4794eac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68917194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b023f6c7ac715ebab4e8e1e3d69a7ebe946f31082eb17c19ae23c8c907fcca3e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9d654b3c49c164cc43a4683b85bf2e1374ecf02ddb2c3f7187cfd204ec3309`  
		Last Modified: Thu, 07 Sep 2023 04:30:10 GMT  
		Size: 19.6 MB (19559687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6a44051400f6cc3488db159e1b84cfff370321f5b901f7fc0655017367fc24b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75147750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7220e378c2e0b1b53e7928e586eb22f1dff712ae790f7f709c52898ac06e700`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:12:56 GMT
ADD file:121000b06bc7b1fdd1e3c87b4b93debc6d4ff153c7e305f8fb9fe076a52c4ccc in / 
# Wed, 16 Aug 2023 01:12:58 GMT
CMD ["bash"]
# Sat, 26 Aug 2023 06:49:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aa279ce1030b6b03f549d223eeb76ece36944bfb3a79e0a2758b54fcadc346bc`  
		Last Modified: Wed, 16 Aug 2023 01:20:59 GMT  
		Size: 53.5 MB (53544042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330f840446ff0bbf07de565959e01855c0e142613b5f006ab2f5cdc4e09b455a`  
		Last Modified: Sat, 26 Aug 2023 06:58:44 GMT  
		Size: 21.6 MB (21603708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c78966048922f6e91c8b97f6a868939a94e2e7d6ab9bfa4c3dc6063560ae2cb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68499325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f94b25d47893079227ca09fea6058c467eaaad1934da225e6e5a6efdb16c921`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:47:24 GMT
ADD file:85c1414a9b16cd9b51c31b6e346dff8675b8a78ca36b9b6e41fe6711444ec72a in / 
# Thu, 07 Sep 2023 00:47:27 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:020f83d738584194c53a58d8f6c431413868b7fb51d9873c9bc0e26b4292e8cd`  
		Last Modified: Thu, 07 Sep 2023 00:52:16 GMT  
		Size: 48.6 MB (48573746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6a12ceebdf73872641b973e28cbc96d9146f8098bfd6cd4d37ad06255121c`  
		Last Modified: Thu, 07 Sep 2023 01:24:56 GMT  
		Size: 19.9 MB (19925579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
