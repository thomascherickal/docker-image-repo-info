## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:53b427624c6fec86ebf05dd3943fece6299796ae642bed199536bcc6ed33cc7a
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
$ docker pull buildpack-deps@sha256:7025838dba8c0001f349bdc4c8c0f58ead89f414da3baafd48c086ff73ec4f7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66557110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c056ceab0a2360a48b262239c346c6c65c9b6124d6f9bd5c58cc79cd46e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:55 GMT
ADD file:e460e5557be9e7a101d17f1464779b74e918d5484eae72c93315f657014cbcfb in / 
# Thu, 07 Sep 2023 00:49:57 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:22:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:147684ee075684edef9db37a29f6f4f0713d7a9a164e9e80c3c137d65c34a829`  
		Last Modified: Thu, 07 Sep 2023 00:54:59 GMT  
		Size: 47.2 MB (47224066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7afb82f9e4205f57e955251cf5cbe9dcdaca025f970b69ebaab4b9eed8a9e5`  
		Last Modified: Thu, 07 Sep 2023 06:28:11 GMT  
		Size: 19.3 MB (19333044 bytes)  
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
$ docker pull buildpack-deps@sha256:776c581f518304b515f3570bfa3c93a93941052897ad40f7dd12252d8dc14028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69484674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b67d3b796e01d702f1d0d286bda1dd17960e58abc37a721f42c53322da5097b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:23 GMT
ADD file:a310e5bf1552790152899a7201a564545c20b24f32390010fc2f559f8fa49be0 in / 
# Thu, 07 Sep 2023 00:41:23 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:57:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f494cfd3ac94aec1bba59af935e909f26f6084cbdc423c867e5262b912d699f9`  
		Last Modified: Thu, 07 Sep 2023 00:47:04 GMT  
		Size: 49.4 MB (49445333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d75a1727c91eb5f86c6a99848305fb36072ff8bddf6c097df4ebcaa0486e22c`  
		Last Modified: Thu, 07 Sep 2023 07:02:58 GMT  
		Size: 20.0 MB (20039341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:dd818d08a74ee98b61e9c3f6fdd06c2ba1bc686750f49ca5d400e114c1cb03c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71375209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5163a54bf2093ab7a6596e4a6fcb4eca515d361625c6441b73f6711342cfb8e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:44 GMT
ADD file:5d53bf28b6cbc8eac8124a07c0bb8e04ee2d0c8989a8b7219612f6ced4f064bc in / 
# Thu, 07 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e0d37cd24f690f803c53e61b67871ef6d1dd8980331679da74a8059a191a9fa`  
		Last Modified: Thu, 07 Sep 2023 00:49:00 GMT  
		Size: 50.5 MB (50534548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b76d6a16699dd100cc2549b60405a4d0d78dc30f81cc263bee0da056e922a5`  
		Last Modified: Thu, 07 Sep 2023 05:42:45 GMT  
		Size: 20.8 MB (20840661 bytes)  
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
$ docker pull buildpack-deps@sha256:8485a38739a386076fc7157d49d900ed3203f3f1ee662800b1a9981cfd973cca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75060804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b64d076ebbfd53befc56bdf4703e82886e6d6f7ee0c53b5178310fa233e487`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:53 GMT
ADD file:1d1937f8a4890754546a2c77f05e3e1d993bb4a60eeb0ed016941880313061ae in / 
# Thu, 07 Sep 2023 00:20:56 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:37:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97f3d0760a8a2cb56d7bb85c16a268c56539a98f9e55ebfcfe233a88995c86d9`  
		Last Modified: Thu, 07 Sep 2023 00:27:49 GMT  
		Size: 53.5 MB (53456016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02194f17d80e36f8422769cee8ff8b9736cebe272d97a858855044f7884c65b`  
		Last Modified: Thu, 07 Sep 2023 09:48:05 GMT  
		Size: 21.6 MB (21604788 bytes)  
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
