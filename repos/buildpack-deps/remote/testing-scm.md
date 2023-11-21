## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:8379a6d16f139d251f0ae3b4a28e81077eb45e62a893a4832250166eb3466c58
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:462e243f20451b99d0d4631d40e08f3aba91c7940a658745d7943320c2f05060
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141250980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d619a60defd797722d81ef2e28e8daee71fad5dc46f5b42a61ed8e4addadf451`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1d4213b5ecd42e4e5d502fa5018177bd7bb7a3f432a8efda32f3fcf3e25470a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135006311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf22d4e85d7661a17d70059b767ea7b7860e81f80d7c21d4e3894acfc178b9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1eeb03a8240f153b8290020f4477589eab862383b6104a427817ada174625af9`  
		Last Modified: Tue, 21 Nov 2023 06:28:15 GMT  
		Size: 63.0 MB (63026793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:75dea238cd526afe7ce7b9513ca46dbf1cc6dadc22fe16aa542aabad67481013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361deb5742958e94144bd2fcf2dca7450743abbd022702c2dcbb5df03bf5b48f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:996ba0fb550a4858251501430c769432e96b323ab0b37fece0320e74ca51d64e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140932507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd12d0b0c131a48bd2384a168b67b7974f1533250aa34782f5a4e6a43c24a523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:945297878d74e2e2c19a6a94a85622c203ecece7a80062df11aa21c95b4cbace`  
		Last Modified: Wed, 15 Nov 2023 06:23:06 GMT  
		Size: 65.6 MB (65609297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6a71927e5c8018db89d04ec95f5d9c4a5ddaeadec1a6b19a620de50b9e3381de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145041655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769c21d85929a1dbb4f206fbca8a9aefcf988596b5655c3a1486b1997768bbc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ea21f7b2672fa2cfcfbb88d236a9d3c18479bd05f2cfc6504481d3006ee65214`  
		Last Modified: Wed, 15 Nov 2023 07:54:36 GMT  
		Size: 67.3 MB (67270819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:018e682c1fa14ae9daeebeb7f90363910e3dbeb3a6c031b7d8c7079e35211784
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139677461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dc06258e7ec131a3593eb9cdd566566727a64176af57e747bbbca3bee96d6d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d10b4a6b3ef635a2b679169bacda8ac4b674df60ae3371a03c8a1f5cc86e7a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153174776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897ba107c9d649eae78c14111b541fbffa91311376657fbeebbcb7275085fe88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:09699f0245492a67f8cf23ca1a57b1830e534c2904c0101f5032102ad5f2c4c1`  
		Last Modified: Tue, 21 Nov 2023 07:10:57 GMT  
		Size: 70.9 MB (70922067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c1151634c7e3a017b784f1eb9a20d31ca5b19e61af07410c71d068ffca257b06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142290545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585f78d00d4e7d5176cfb4e20e019ad8271fa52f40eae6313924bd54827c4bde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d09114f0213626e79784208aa286e09335b4ba1f291eb0eca1b085809f09d3a4`  
		Last Modified: Tue, 21 Nov 2023 06:19:11 GMT  
		Size: 66.5 MB (66490948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
