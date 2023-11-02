## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:e62c7af6b879e506e13d108beea0191c5716d696df3f3b20d0054bb070a29a59
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
$ docker pull buildpack-deps@sha256:69b4c504c9caa677158b04a5dffa59425c7649f735a7b8728d6537f55e5bbf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139405504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea95fd684a079be0c5deeb96861c07b4992a71e7818a9c7960f6a1baee07c8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:57:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bf371b8152e5df155015cbda7e76bcf445a8be262f7017a9c2cd27a64c3bd875`  
		Last Modified: Wed, 01 Nov 2023 00:28:24 GMT  
		Size: 49.5 MB (49534303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdee5573ddff91e45c81d11193d3d33f964fe89aa56549950a84c64303f6c2f`  
		Last Modified: Wed, 01 Nov 2023 01:05:03 GMT  
		Size: 24.4 MB (24354415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee245293502f2c719e3e2302ae5289fe69631d1c3bc58055166bf026f0a28a`  
		Last Modified: Wed, 01 Nov 2023 01:05:21 GMT  
		Size: 65.5 MB (65516786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9417cb6ff8564c4d3bf1b82efb889976197dc0cb69f9ef179d844ff4c5a47a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133219295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791053f347823ad45507927ca12fc46992f6485bb6ded865460b387df1861d71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:00:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff5e12103a446acf43b661291fc30a67ca5851b7c1f67906ac39a5a609ef1c`  
		Last Modified: Wed, 01 Nov 2023 03:07:30 GMT  
		Size: 63.0 MB (63010355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd781c833a3b0edcfcd2d86a091e60c74feac13e09a04d42ecf30ed1992d57c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127826362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82080f96e7a0b68c7bc49369001f13514e2d0bb7da42e22f391c832020ee4beb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa95d6d6902734ac1af894edaf67096b114b4935d12a40bf35b44bca0f33e21`  
		Last Modified: Wed, 01 Nov 2023 02:45:16 GMT  
		Size: 60.6 MB (60610186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24a9674f7ee955af54b2ff9dff74e3a3a5ab908c092ef87046b36185bba90552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139074611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49432ff4faca7e8f8e7e1c0674996ca4a6b2a93bdec8b6cf4059353c81e1a6eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:09:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8977dd4a34d5416619317940446894bcaf8bc0c5f832e562683f4aa703db7f`  
		Last Modified: Wed, 01 Nov 2023 02:16:44 GMT  
		Size: 65.6 MB (65605231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf9e365b381337f4d6b2f5562e4a5c66f62d51e107a697e2abc16c6cf3807722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142969483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890f7be8650dfbec3174b0c555ee6f84c9085c83f218e591ccd4bcd9822ca9fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a1138df818473932216f10a656452bbeead89efc81870811003208908e138`  
		Last Modified: Wed, 01 Nov 2023 14:00:17 GMT  
		Size: 67.3 MB (67267247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:be68bbc454236b68329461f9d169e194956bde9a85d831f12f67ffc86823332b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137560466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8009d8ed04a6125b5b9fefa3fad72e3a2ffe0dc6f0abd9e503ca667526d713c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7d59b79a44cf2fd6509592cd5ffa2ac26dd4a37fb70dbe72408010c4a2926`  
		Last Modified: Wed, 01 Nov 2023 22:01:27 GMT  
		Size: 64.3 MB (64323488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:353b2a9b54d029503ae0b036b97d823535850f152a54820f9faeb5adba83eb89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150372100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8e3c9ad7f10aec351582b84c48d9a4a2a4b8b4496b3fc285248982f5238995`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0c3580029357b03dab5202367b9675aa78ae0db89b391735b34327fa0aad12e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140042075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4c6469d28f8ab0416e1b296a12c5545babdafd6352d9d73e5fab9096a5c5d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa15755375f48461c5f3dcfc8b172b68b06d99c8b37bacff592046619c269ff5`  
		Last Modified: Wed, 01 Nov 2023 02:07:15 GMT  
		Size: 66.5 MB (66478150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
