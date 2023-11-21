## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:d45682fe48133a66ef3b5d2a535b87687296abd7a0f00917ad9264053e63091d
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:16d76495ee528187f25d63a08b40e77e5331d2d813b678c1bd4b2874cb4958f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75742315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08129f3119f282d801ddd2495b0ce1a0ff7da19d113e7643294c273eefee0517`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a7da9b745838c041278c9aeba2fbb2ca1837a9530b6f96239c8f5c58d6b963ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71979518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd2c0fa32747f25861583e129cca4b26127abcc0f95d20b84cbe0118c62cefc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e31302afdcfe501a4c29c36c0a87773fff9d16438b1671c9029e28df9d629a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68886120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c65f518912c504507ebe9ed5400c06cba43acf501dfe7b266a37735559d3f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:57ab995ed8f689c7931c0a83b6f2b948ace8c98a21555e6f297fde5918bf4996
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75323210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905f2ed7423347e36afbd048bfece66a4d84b57c278a57d081648102e9399b77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c6c188fd23ca22f501be40067c2957e2a3a5d1f7f4c18b0bfd7e2bdf9455fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77770836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f98cf6f937c6e49091148e07808fcb8d6c74b67e7a76d289068b9d3fdb2e89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4912dd6e6037dde41e039e3f907c9a89a70a4cb4b47eb68958c1d742b35e0a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75352468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ffb34227c79ce599b62d0355af9d7910bd374bc71278835a773cbc85704dea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:965f912e338611b668babc493a452d7633aada0b922596c5ef12cc6e50e27a3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82252709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bdba459863fec3e91bd7c853b0ea34383073b319aa7a132424943ec736438d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cec0b4b3003b6e8ca7b66e3ea1180aacfef23d35fe6903a4accc9f2e403d199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75799597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31893a587eeb03b3917a1a1c908f5d45b32756818b46d56b8e081ce5579ba7f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
