## `debian:rc-buggy`

```console
$ docker pull debian@sha256:d67c45d2ba5ea4f7b3ad18ba6deb67ca084dbe97ad0ff1796d901de8808ea2c5
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:e148c01faafff70d9d506961f3bafbedef38990aaf2efdaa9f62d05bff79ddad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53162126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e935be398080311b76d779304d5bae7b479263d6e3a23867f57c77540b3d96f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:32 GMT
ADD file:dffa51e87e58558bb4b777e117ecb18500d90a9646513d0d8d9724bb5c949dc5 in / 
# Sat, 28 May 2022 01:21:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:23:03 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7fa02d3fa6e2ab30d6142a096f5321227237c89c02dd890ff9fa745dbf0790d1`  
		Last Modified: Sat, 28 May 2022 01:27:35 GMT  
		Size: 53.2 MB (53161898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2b3e8e844db205834a3141e72bdd7c9dc1e646e91958969516c6247e8dbfb5`  
		Last Modified: Sat, 28 May 2022 01:30:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:917820f1fe302b56467bbcbd693539ebf3d438f538d38afc63c3583fd13f7f7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50940059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01e83b6fac36db5aeb7498b43d76132e51fd36ffee63ccac59de218b4696780`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:53:50 GMT
ADD file:4f142f5aefa97fb474a705d0b74abadc5a3efdc7faa28a865e8f774b46affcfa in / 
# Wed, 11 May 2022 00:53:51 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:58:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d1faa3808d790c86a331ed5dce0a7a8af6a26aa395d982f287f5d3fe6362186a`  
		Last Modified: Wed, 11 May 2022 01:10:36 GMT  
		Size: 50.9 MB (50939831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9690c9d6869f0e146db789a53a2ab5d60825ca265a823e7fd6354b05a0ec2`  
		Last Modified: Wed, 11 May 2022 01:16:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:19b565988d310ce5011fa5a63aa24d3e23b3430ff3eb8a58e966b0a0893a6d99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48693715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb254726069382002a742d82e0a65ae5f89af978402bd600286bad55ae679d90`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:03:25 GMT
ADD file:8021dbeb20862f976e9f6edfab38dfb8756a92dd1ede73d49af4c657334e675d in / 
# Sat, 28 May 2022 01:03:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:08:13 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0e42766a606a457d26f0182502f6f1920959f31aa96f3bea8438d9c1662a0e5`  
		Last Modified: Sat, 28 May 2022 01:19:59 GMT  
		Size: 48.7 MB (48693491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2809724bb3f25b79819bdcf175e9e34dc735e5ce2e736d5f3fea89580214ab`  
		Last Modified: Sat, 28 May 2022 01:24:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:99429a692c76b00d96a37ea1ad6c2dcaa6d47047e2b34888a60b6fdd0cb9dd3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52261530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6e19aaeac0e389346a25a0907a44711cb3fa99b0f29a527dddb89f98d618a8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:02 GMT
ADD file:759f672e6b6df1008eaa41bb27f3166127eb98b40bb49919dd41fa53f7e9d598 in / 
# Sat, 28 May 2022 00:42:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:43:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:eab2172da7bda865d054e2983e44baa941cea4422c5c64ceeb52f19efc8e9a16`  
		Last Modified: Sat, 28 May 2022 00:50:07 GMT  
		Size: 52.3 MB (52261302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14192d76a4a08a40688357598b1fcf246eb8922673176765bcfea0e585c9edf6`  
		Last Modified: Sat, 28 May 2022 00:53:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:94ccb245b576b501331506350eaa0feb0da151a2667e7f649ec7acdd0c466230
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54158944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91615f672daa741c0aee0f743df7985b287e3740bb4308bdaad3dccd3e81321`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:03 GMT
ADD file:dd10bdbf07bc13b42a7021b48621548cda7b383bf0edb8dff1e35d908f50c392 in / 
# Sat, 28 May 2022 00:41:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:43:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e233042357300fc1ac460e8583f90e2b88388d7c2a9016f91be99da315c46fcc`  
		Last Modified: Sat, 28 May 2022 00:49:18 GMT  
		Size: 54.2 MB (54158716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5ad64f8c5ed67f59112c69f772bc1553a1e013a3611c6c558f44e98052a79`  
		Last Modified: Sat, 28 May 2022 00:52:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:36e02890760424c3db7b259518abaa7365b3bcd6944a09d2e8220a23b6288bf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52283428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a3087e337df0902d887e3eb7043be6f5f73a8fbc35ab1cc1e018be23f76ce3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:14:06 GMT
ADD file:1687a4039bc00edb9de7ba18be7ce08c7df3d2cf6a4b7a30cb5bb60f41d3c082 in / 
# Sat, 28 May 2022 01:14:11 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:18:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a7336e150b70b2115ef0d770279f4e6f79de8d6e16c87dd256445530c1c68d1e`  
		Last Modified: Sat, 28 May 2022 01:24:53 GMT  
		Size: 52.3 MB (52283200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4727c9bcc061540ce01dc87863718ae603db9365c4396d233e99d03f040fcac8`  
		Last Modified: Sat, 28 May 2022 01:29:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:895ec750c45a5745066b8a2da37c2dc052b106557b44732d2e481a27f878414d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57378699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8674ac4b13f4433ade5c4fbce5ce869bf27d5881865ffca2a9dd3009efa0fe6a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:25:12 GMT
ADD file:ae9857e5f5e911c083920a02f175061f1626b33e8244c6b286b16a61fb6326ab in / 
# Sat, 28 May 2022 01:25:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:28:17 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:37e804d95f71e07756995895c16c589fb7c512c0b5fda75c9e57d4ba10ea4c27`  
		Last Modified: Sat, 28 May 2022 01:34:49 GMT  
		Size: 57.4 MB (57378472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ada2efedeb7146bd82c565fca120c7c8dadddba3b8e7ee461218f0f582f873`  
		Last Modified: Sat, 28 May 2022 01:37:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:62f79cd3374aa69a0e21069e6f082c057551f1770676a845f7f287cefc3d6ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51703442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ce9ebfb788ae8cd919db4460d2c9120f0db7770f4f5553dfdaa6a542bb0a60`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:44:37 GMT
ADD file:03a528116badd98d1660ab1a83ce0462a11168a2dae972be4891032c54483f22 in / 
# Sat, 28 May 2022 00:44:41 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:46:58 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0cf941fb152b37e3fda284ae5eceb3dab36c26511fe06a7105ee43081ca68554`  
		Last Modified: Sat, 28 May 2022 00:51:02 GMT  
		Size: 51.7 MB (51703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fe12babf16ad61003af3e401f503375debf9090b06ef2bb8b467eabc19081b`  
		Last Modified: Sat, 28 May 2022 00:52:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
