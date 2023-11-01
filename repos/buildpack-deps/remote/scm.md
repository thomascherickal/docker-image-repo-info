## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:3ff215415c41c73cf8b9382d1b0d23e92f2efb27fbf5b37bc724bf2a389a7587
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:93590f9f25a12437d9d01f7ac4309b83af5532680e36bbc01181f61e19ae7135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137761586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941f9c887621d4fee5936ccc92b35b887f74ed81aac7b90fcedc1fcb5d65741b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3f6585039e542b0e19a291d5b489ba1d3647b261627e2c2467209933bd6424e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131646709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3619e24c9c6a8902a9cef46ec89de341f0bb65f1bb2c8e5f914176c890aa0259`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5c80e22ca4ce0fc1769cad578ca3c0ec2d6020358bee0e0708ad8a7a4e1890eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126400592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19fe7e4dbcb60f0b62f9d2258c1b8367310a78105eeac8cf15a871a70b0f97b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ece8d9aa98c4e2ac79b982df68ee2ac9b4ae41a08fb3d92800f7124578ffffc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137194983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0674043e7c55a6a4fc06506c806c8d8dab00a6ab67719922aa473372777950aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0225376ebdabef6ebca5adfd31d8e251c589b21de778ff4d6eb5f4435c87b92e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141471994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4557670d1bf5012131b762bb020c0f608408deca580a2b2638a6a0794046695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:978fa0881d84f169ef3b182a55614b8c003440bfc7daff138acec86929b33f45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135971603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399ffe5bc61d49dc80a6a20678665009b14d5784ffd8ec66bd758ded95515def`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e720e0531751cf77d1933f62e84bc5d4d2d63c0da3d890797548ca4e0192e571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb46a21911fb664a3630a45e7195ee955092521b2066322ec031cd4dd405ff3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:198224f3809fdab1ffa595ddb0d788d97dec1c41556a1a5e913b711ec6ccdaab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135122600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8fda4e35a32e1c513adb4a70b998c8a77f96ac52d6a7c94f6f085b1d1995b8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
