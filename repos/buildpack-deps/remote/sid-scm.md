## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:945093168140b621e90488ef0ed46bcb2cc26a2999b50a5a4f6b7a31d823e56f
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
$ docker pull buildpack-deps@sha256:7c5933eed2248b68c715c96b72c91e0ccaa181eb231423fd1b6240d9a73a511a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138082358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1e6a03fcd1de6f186a845d3f6e4e140f416cdb243d7020bed9b8b9f81a4981`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:53:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c93962a936c4e623abcd5c132acd83a550b41b475220f5ba03708dd030b1c0`  
		Last Modified: Tue, 23 May 2023 01:58:03 GMT  
		Size: 24.3 MB (24276999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3f584564987f0be0d812aecff1df91b59183f5667eadff38eabade6484098b`  
		Last Modified: Tue, 23 May 2023 01:58:20 GMT  
		Size: 64.5 MB (64516175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca0129c31bd738d32d309e899c2fb3935540fafc790eefb0cdb5fd67e815f3fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132250396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d394e34a03499c0b680e262586555cfdb14ad7c7dc1d5a5bf546b6d9144363a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:48:49 GMT
ADD file:bbdd13db0e090d7d928a2beba57e3c1340342d05e5c15f7b7377c9791a5cb4ba in / 
# Tue, 23 May 2023 00:48:50 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:18:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:19:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d14a321d144fc48aa438b2364b0f1a5667979322ef9cada9309bca48584a11a1`  
		Last Modified: Tue, 23 May 2023 00:51:36 GMT  
		Size: 47.2 MB (47154613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af911895fe3f6120ef979a3b5dbd9bac4de6b4d900e6ad8ddd6b28ccb19a7746`  
		Last Modified: Tue, 23 May 2023 01:22:48 GMT  
		Size: 23.0 MB (22951581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc480ad84aad81f48b8427943b9e4cb119ca2f0562152d578d98f45ff47a69b`  
		Last Modified: Tue, 23 May 2023 01:23:06 GMT  
		Size: 62.1 MB (62144202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ab0243a521c1c7f1594786e9740b3ea4af0957543c76a2154250e16896e0138d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127981149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a93cb3edb35101b92d8d4bb39ff8037c1209fcdfba20441be54d9a44ded27bb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:42 GMT
ADD file:17739fc730ad8febc64f53eec61cbf10f8d2c5184cfda5466e89ab423a88f9d6 in / 
# Tue, 02 May 2023 23:48:42 GMT
CMD ["bash"]
# Wed, 17 May 2023 00:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 May 2023 00:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0b827c534260a55126ac3b18c14ea9160a3a3a03448b5c2b4462f9f3f4cf0ab`  
		Last Modified: Tue, 02 May 2023 23:53:05 GMT  
		Size: 45.0 MB (44988077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858686fb647755cfaf9d97846212a8b1056f291d77f962bb8bf7be5d16a5ff60`  
		Last Modified: Wed, 17 May 2023 00:24:35 GMT  
		Size: 23.2 MB (23219225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16fdb017446b11706119bca2906a6b8fa79ccf636d08457981e54be450413bf`  
		Last Modified: Wed, 17 May 2023 00:24:55 GMT  
		Size: 59.8 MB (59773847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b4092b6c55943924df5c41d7c192457b2383f9bf1df7a88784b1d139f6498fd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138739471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8543a16b79610649af1d8aa2b6403f15f545d458f63ae31d0af59feb3360caee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:23:28 GMT
ADD file:cb107aa90220a9fc72fe1e3aa26878752691d6e9eb04696738920b5834c6d9e2 in / 
# Wed, 03 May 2023 00:23:29 GMT
CMD ["bash"]
# Tue, 16 May 2023 23:42:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 23:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77a3c1a83d83f65ef8fd579d19879f09a4018e384f42cfa55f82d426f32ff840`  
		Last Modified: Wed, 03 May 2023 00:27:15 GMT  
		Size: 49.3 MB (49345262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52781deab323ab07663419dcbd3af52651bfaf9895ae88fa6160c7a78b5c7c0`  
		Last Modified: Tue, 16 May 2023 23:57:13 GMT  
		Size: 24.9 MB (24896432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c9f3ed5b90a971a7d8c99f95aa99252f2fcd3a7fadddd62e9c1b012f89b3b6`  
		Last Modified: Tue, 16 May 2023 23:57:29 GMT  
		Size: 64.5 MB (64497777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:422d0aa6fff6fcb37cd178f841f4443fbb8e965f81a82e967c9594cac948b3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141766746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5385cadb1e1cdf30b092f4e8fe2ca0e40a08e8704a2869b66a4f8380fba3c9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0773461f28d3828f3df4474bf07fd4bc2d3cdec7f41c65f1253678f4a5f861b9`  
		Last Modified: Tue, 23 May 2023 02:07:38 GMT  
		Size: 25.1 MB (25112113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3b130ddfdd33ce29355bf1322b63f47960cc73b9e64789abc64c7954273d2`  
		Last Modified: Tue, 23 May 2023 02:07:59 GMT  
		Size: 66.3 MB (66343136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1b1edb40ca42a51b07f5bb498c7439c17e692ba56b3fea9752a17ca5bb082f3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136588935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3f823aefc280a80ebb4d6ebd8df0141176ba201aea05a25f28922abd20d2f0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:11:03 GMT
ADD file:4747b72418fe8be7c83a33927d22b74c9169c9f02959e41f61d71d739fd30ff8 in / 
# Tue, 23 May 2023 01:11:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:58:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f1da758a33cea391a9b76cbdcea2cd41c87b5a2c179c4c1f3d65a456c65d8e1`  
		Last Modified: Tue, 23 May 2023 01:20:05 GMT  
		Size: 49.3 MB (49293333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebbc59228088cdeea0edefdf4596c78cc8f25b00177cd12202cf4a879b33945`  
		Last Modified: Tue, 23 May 2023 02:13:15 GMT  
		Size: 23.9 MB (23868941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2051f379a7704fbd90dac1820d91a3165e19ecd15d8720c7e0af0762d9ecd78`  
		Last Modified: Tue, 23 May 2023 02:14:04 GMT  
		Size: 63.4 MB (63426661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4e4e157c685485b0720b1004928b51fcb8cf204acb6f9feb071186aca3e6b53a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149190846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e84aced56271ea273dff3a077a1d6b1b1de944803da6e41e84ae238253cdc46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:17:52 GMT
ADD file:cffada1d28fb1dc246127e193bd218b3c76450667fe4cd380f04a5caf5571be9 in / 
# Tue, 23 May 2023 01:17:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:55:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:55:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d914d1b8acfde6dc74b2fb48f95f7aedafbe4e4ad3b6ea21aa9db007eee47739`  
		Last Modified: Tue, 23 May 2023 01:22:29 GMT  
		Size: 53.3 MB (53302061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd02567bd019328b094640438b56aa8ec096d625eb4dd7646bad29dc33d703`  
		Last Modified: Tue, 23 May 2023 02:02:41 GMT  
		Size: 25.9 MB (25928691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37bffe3818ac84f2da95782d45c9d0ec1ac2686d474eef4dd224cd8a76dca7a`  
		Last Modified: Tue, 23 May 2023 02:03:23 GMT  
		Size: 70.0 MB (69960094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0f3f24588a6e3e641f6ceaf5cac395c4327dce2cd21464e8098d2f6590e17e99
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127953533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23ba7ed8591cde0e9e2378b515b76628f77b9612c90c738b497144207f3e2e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:09:11 GMT
ADD file:20221b6f94aa48c9890226bf3be037d4b2c2cb20a076225236ca9d2c09efcbd4 in / 
# Tue, 23 May 2023 01:09:13 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:04b827a08c39becba5f6c479b23a265f1f501c5d3aef76e037fa30157864daaf`  
		Last Modified: Tue, 23 May 2023 01:12:26 GMT  
		Size: 45.5 MB (45503414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efef68c40b0d23d116a73ed6b2156ae42fb93e63547bebff3d6febc2bbbea30`  
		Last Modified: Tue, 23 May 2023 01:42:27 GMT  
		Size: 22.5 MB (22487151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058e1f937b69e6050ad30d3ef4e1094300d70d5175e07c16d50c7efd62c36c8`  
		Last Modified: Tue, 23 May 2023 01:43:46 GMT  
		Size: 60.0 MB (59962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e046ec9cded061a5b59e552f8a7d71ea7d25430a1dd8d795594c1daa79d017e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136634108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35394c98b44287f15a02362a5d740ef8003f15408dc1def9f0ffe8dd492eeba3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 03:42:08 GMT
ADD file:f714218b704bfe42a591f19c2fc0360b178732edfcd6b12687ea572c74b84171 in / 
# Wed, 03 May 2023 03:42:11 GMT
CMD ["bash"]
# Tue, 16 May 2023 23:43:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 23:43:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cad3c2eaf2133414000bf2d83ce6816eb4031d5b81288493af8102df33f2e4c`  
		Last Modified: Wed, 03 May 2023 03:45:13 GMT  
		Size: 47.7 MB (47675884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bab5e47182cd759c84de89b674a6e02b13aef910e9d07d034d7b802c36c2c9`  
		Last Modified: Tue, 16 May 2023 23:55:48 GMT  
		Size: 25.4 MB (25352347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79c5309e9a86c28868504dbce3cd42aab010a6909a28eee8682f5a41cf684d5`  
		Last Modified: Tue, 16 May 2023 23:56:03 GMT  
		Size: 63.6 MB (63605877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
