## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:9c5d9dc31c46e42857fe71925e7bb7777399aaeb18ed91ad1f76e1deda549703
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
$ docker pull buildpack-deps@sha256:183b0d8da52453026ea622f8c7c995c1081c5ae8a3f6862372f63e7b7919e8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71899437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2b5a8f8d6c6dac8255764c07b7f9820742d18652d355b4c770aa79586d64d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
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
$ docker pull buildpack-deps@sha256:5c597fc3f240d9ec58bc7a8bb6eac544d7f91bc95c583c0dea4a8c5343d2cd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69636607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799b9d80cfbf3d254cc2d8e1ba2618aeab9932ba566919d1c5b40598e8817518`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fda33c228a37bc721c34159128f4b6f92a8612f6ff05cb52658d80550ce009c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71375549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b7cb6002b21caeea5999881a72aa5b1ca27460c4602a3328892064928b5dc6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
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
$ docker pull buildpack-deps@sha256:a025ed6b3c26a7fbaeb80a232f467b2b87e5075ffbf6a43ed4dfc3f122c22f88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82205298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04223e52eef897909d667acd82f3d25674d39d08063ec943bee425cb270c6ab7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69f5a6be863cb69c5e8fbf9fb8eaf91c2994ca992b4db4df61c766a3dc512c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68959952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c167457a1683a82fde1556d548ac9344db2d2d3e22530763b33801be31261264`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
