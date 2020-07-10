<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fedora`

-	[`fedora:31`](#fedora31)
-	[`fedora:32`](#fedora32)
-	[`fedora:33`](#fedora33)
-	[`fedora:latest`](#fedoralatest)
-	[`fedora:rawhide`](#fedorarawhide)

## `fedora:31`

```console
$ docker pull fedora@sha256:ee55117b3058f2f12961184fae4b9c392586e400487626c6bd0d15b4eae94ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:31` - linux; amd64

```console
$ docker pull fedora@sha256:829948d9a54ca9926c7fa01a976bbeccf38d66e85b558ca61f4b589246ab2d26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66966026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adfbfa4a115a799771d3060d0aa213584c91e549187da4fb0036240294ca4a8f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:06 GMT
ENV DISTTAG=f31container FGC=f31 FBR=f31
# Thu, 14 May 2020 21:37:14 GMT
ADD file:aae4719060028e855fba1a29a337a9eddb011d34368d5754451bba6953287a5c in / 
# Thu, 14 May 2020 21:37:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4c69497db0358623df08ede06fbe682f0858119dd6b60a97d34552e5eba05c54`  
		Last Modified: Thu, 14 May 2020 21:38:26 GMT  
		Size: 67.0 MB (66966026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:31` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:2bd5c2ae5e0de798d6cb0114837c1fe8b1f7913f8d445a9b2fb55c7631c342e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66686395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd14e3f5fc19cc3b63ee29e7aac0ba9ca4c4ee1396200e97c4362b8f8f4cf053`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:00:08 GMT
ENV DISTTAG=f31container FGC=f31 FBR=f31
# Thu, 14 May 2020 20:25:13 GMT
ADD file:c2a1561f6cd9931d32b69cdd20033a4c8aa0faf3e81ff44e6e68c2f6a9226b26 in / 
# Thu, 14 May 2020 20:25:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:21d2db314d55c5a8ee37e826502ddb24522a652180dc8cc1e82f9dbce0b784e4`  
		Last Modified: Thu, 14 May 2020 20:27:25 GMT  
		Size: 66.7 MB (66686395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:31` - linux; ppc64le

```console
$ docker pull fedora@sha256:f6908fb03161c9d8ca68420adca93c9ad9d5bb051a3054c59d29f6ba1b3609fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72720784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da46d0845c7b9c5725caa9607fc22cfd5c0bd4236b895d466bfb3464b5d78ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:38:07 GMT
ENV DISTTAG=f31container FGC=f31 FBR=f31
# Thu, 14 May 2020 19:00:15 GMT
ADD file:8e61ac6cc804dd3da088020d326bd41761d4e550f1f9c64ec14032f106b9c8ad in / 
# Thu, 14 May 2020 19:00:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:870983bbfde565dcedd30fcfb28ae539f2b153c6a433435cab222a380da61453`  
		Last Modified: Thu, 14 May 2020 19:26:45 GMT  
		Size: 72.7 MB (72720784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:31` - linux; s390x

```console
$ docker pull fedora@sha256:e17b07279a9d99212e9d99219a8cee635dea191022f6a72f0a919f191b728d73
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64222679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd7e87ea01adcc5dc193ed50fa6f63a4f73e3962f255564ff88102e3513f58b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 22:42:41 GMT
ENV DISTTAG=f31container FGC=f31 FBR=f31
# Thu, 14 May 2020 19:47:57 GMT
ADD file:290d309bacb43d375d7c858f2cf9b5cfca2b1dd336f4ec5537c6c94dea776081 in / 
# Thu, 14 May 2020 19:48:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:21d955128c3bb343995999edb7a1660f48ade018d808489ebbc0cb767fe5a2e8`  
		Last Modified: Thu, 14 May 2020 19:49:00 GMT  
		Size: 64.2 MB (64222679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:32`

```console
$ docker pull fedora@sha256:e69b5a62ce23c673885bddc94e6679c9b2af683059637ceddb9cff458537a326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:32` - linux; amd64

```console
$ docker pull fedora@sha256:df6e2e0f4435151ea77a444965b485ae23380a3d239dfa9f5e83d422d2d524b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70725419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a8d315e6208e83b094dc86933051bf53944fea3c372a63f8cc7d5ad8c582895`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:25 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 21:37:40 GMT
ADD file:27dd871d276a768f643c130f569d5dc14a6f4cb63b24ba645f0498ce76e72ea5 in / 
# Thu, 14 May 2020 21:37:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0169c1449c1683326a646321d0823c58e8fbbfdce158268222f416211963facc`  
		Last Modified: Thu, 14 May 2020 21:38:43 GMT  
		Size: 70.7 MB (70725419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:32` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:3635f8a7897fa899385a1567808059b65b301607c8b3bd75cb6d5d4efb1e60bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70934825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533f07d9c4c129a737fd3fc5feef28f52b7e8e869cc8e0e904d274049e15660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:00:50 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 20:25:59 GMT
ADD file:ba47c1c95d41525b403821b60e838677be5971e000b116d1fc12fb7bef8f2bf1 in / 
# Thu, 14 May 2020 20:26:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e3c512ad26c648010d2cd374aab5cbdcd2367f89fbb5930fe480e919d803f7ac`  
		Last Modified: Thu, 14 May 2020 20:27:50 GMT  
		Size: 70.9 MB (70934825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:32` - linux; ppc64le

```console
$ docker pull fedora@sha256:58d4a665ff9790fe974253be98c0fd6ae095b786b02793451a0153afaa449d97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77814155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814461ec3c5c4e664200a9a6b9edd0f2ae01a8f7553e2bef639c72838a979d78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:39:03 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 19:18:18 GMT
ADD file:312e76f1ff504b57f4f8ea0ab465c6bf4f26c898f9ea987e02d179a9438b9dca in / 
# Thu, 14 May 2020 19:18:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc7b791f437427423c6e2dbe6244fbb26970c9e69ee5dfa492b0a921f047f9bc`  
		Last Modified: Thu, 14 May 2020 19:28:22 GMT  
		Size: 77.8 MB (77814155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:32` - linux; s390x

```console
$ docker pull fedora@sha256:fc88cbd231d2756d094c14b99bc386366818aeb829a6b1268464917740f1aca0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72968816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427ad744d0b765a0562c3ebfa4e801e330e57ce613acdc4b3a4149f7feae1e2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 22:42:59 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 19:48:18 GMT
ADD file:3d8605dea411a4d92995ac5caa4187b4e09cb1b7d9f49b8d17189ceb8e445fe2 in / 
# Thu, 14 May 2020 19:48:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6742256fd3528d6e61f867c0b40f24e2b98c0b6ce874729132a81d34b9ab60d8`  
		Last Modified: Thu, 14 May 2020 19:49:16 GMT  
		Size: 73.0 MB (72968816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:33`

```console
$ docker pull fedora@sha256:f0ff32d92e7e54d2e411f688693b94d420c153d4b325c6e73ea0a5a6e4ce8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:33` - linux; amd64

```console
$ docker pull fedora@sha256:f26b82189550e597b0507c86a093411d9288301c479cb1ea05c6f16bead6ee6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71643182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5950517e265271fe84cc4b7dbd3d9128111fdb77da19676d302e9da182dd4bd2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:44 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 21:38:01 GMT
ADD file:fee9df5309c80d5beb7a0bdf951cc2956da9eb4bcad7fb0210c31314f376182c in / 
# Thu, 14 May 2020 21:38:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0e51c574d5686a95c924c763307acf89ffdae5303576b220175b523efb0cd684`  
		Last Modified: Thu, 14 May 2020 21:39:05 GMT  
		Size: 71.6 MB (71643182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:33` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:e11922dc049aae05c8509bf9411a55afef1fe87906f77febf0de2831a7bbfaf0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71792936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0af930c2c542a675935b680e1dfe0a80397b44bb3229d191d7f8adb6fa34d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:01:35 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 20:26:40 GMT
ADD file:ea1e2b10a553d248e54503387c4afe958caa0ee09aee23be39a1ac295fe465a5 in / 
# Thu, 14 May 2020 20:26:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4c95d0f8fc948ebf7c0a53f5d7975591feb65f55189c1b7be7199682e6833f51`  
		Last Modified: Thu, 14 May 2020 20:28:15 GMT  
		Size: 71.8 MB (71792936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:33` - linux; ppc64le

```console
$ docker pull fedora@sha256:be7b77539915626bcbfc13152c171ff03dd6dbfa72239d6c2b31367ad567e9c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78768915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d65ab49d340118d75b08c599c3fd49328477d9a9f2cc080055f1fab7fa068e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:42:50 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 19:24:48 GMT
ADD file:4e0cae3cc78df1587b6f6d959e15c020afdbb47e97e8eeb143232f1ea07172e1 in / 
# Thu, 14 May 2020 19:25:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:116dbb0ae4b42e0581b59cbd704264806be495971e3f6b6effccaf44e9518e1b`  
		Last Modified: Thu, 14 May 2020 19:28:48 GMT  
		Size: 78.8 MB (78768915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:33` - linux; s390x

```console
$ docker pull fedora@sha256:da5ab2238f13a9189b1f4e167cb89bd8c475b0dffb86b7dbd84c369e00e152f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73791167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4323209fe15820ea8e5980fba4c3359df95e711b626590b4446108b816b0f508`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 22:43:17 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 19:48:37 GMT
ADD file:7feba5175cb32e93786f5cddb08342b5383f22c968b77255705018d5efb97e16 in / 
# Thu, 14 May 2020 19:48:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:58d502d459c452899430ab5be4f1c4f85fc0c230d280618f53b5bb85ed808cbb`  
		Last Modified: Thu, 14 May 2020 19:49:31 GMT  
		Size: 73.8 MB (73791167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:latest`

```console
$ docker pull fedora@sha256:e69b5a62ce23c673885bddc94e6679c9b2af683059637ceddb9cff458537a326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:df6e2e0f4435151ea77a444965b485ae23380a3d239dfa9f5e83d422d2d524b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70725419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a8d315e6208e83b094dc86933051bf53944fea3c372a63f8cc7d5ad8c582895`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:25 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 21:37:40 GMT
ADD file:27dd871d276a768f643c130f569d5dc14a6f4cb63b24ba645f0498ce76e72ea5 in / 
# Thu, 14 May 2020 21:37:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0169c1449c1683326a646321d0823c58e8fbbfdce158268222f416211963facc`  
		Last Modified: Thu, 14 May 2020 21:38:43 GMT  
		Size: 70.7 MB (70725419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:3635f8a7897fa899385a1567808059b65b301607c8b3bd75cb6d5d4efb1e60bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70934825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533f07d9c4c129a737fd3fc5feef28f52b7e8e869cc8e0e904d274049e15660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:00:50 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 20:25:59 GMT
ADD file:ba47c1c95d41525b403821b60e838677be5971e000b116d1fc12fb7bef8f2bf1 in / 
# Thu, 14 May 2020 20:26:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e3c512ad26c648010d2cd374aab5cbdcd2367f89fbb5930fe480e919d803f7ac`  
		Last Modified: Thu, 14 May 2020 20:27:50 GMT  
		Size: 70.9 MB (70934825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:58d4a665ff9790fe974253be98c0fd6ae095b786b02793451a0153afaa449d97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77814155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814461ec3c5c4e664200a9a6b9edd0f2ae01a8f7553e2bef639c72838a979d78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:39:03 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 19:18:18 GMT
ADD file:312e76f1ff504b57f4f8ea0ab465c6bf4f26c898f9ea987e02d179a9438b9dca in / 
# Thu, 14 May 2020 19:18:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc7b791f437427423c6e2dbe6244fbb26970c9e69ee5dfa492b0a921f047f9bc`  
		Last Modified: Thu, 14 May 2020 19:28:22 GMT  
		Size: 77.8 MB (77814155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:fc88cbd231d2756d094c14b99bc386366818aeb829a6b1268464917740f1aca0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72968816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427ad744d0b765a0562c3ebfa4e801e330e57ce613acdc4b3a4149f7feae1e2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 22:42:59 GMT
ENV DISTTAG=f32container FGC=f32 FBR=f32
# Thu, 14 May 2020 19:48:18 GMT
ADD file:3d8605dea411a4d92995ac5caa4187b4e09cb1b7d9f49b8d17189ceb8e445fe2 in / 
# Thu, 14 May 2020 19:48:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6742256fd3528d6e61f867c0b40f24e2b98c0b6ce874729132a81d34b9ab60d8`  
		Last Modified: Thu, 14 May 2020 19:49:16 GMT  
		Size: 73.0 MB (72968816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:rawhide`

```console
$ docker pull fedora@sha256:f0ff32d92e7e54d2e411f688693b94d420c153d4b325c6e73ea0a5a6e4ce8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:f26b82189550e597b0507c86a093411d9288301c479cb1ea05c6f16bead6ee6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71643182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5950517e265271fe84cc4b7dbd3d9128111fdb77da19676d302e9da182dd4bd2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:44 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 21:38:01 GMT
ADD file:fee9df5309c80d5beb7a0bdf951cc2956da9eb4bcad7fb0210c31314f376182c in / 
# Thu, 14 May 2020 21:38:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0e51c574d5686a95c924c763307acf89ffdae5303576b220175b523efb0cd684`  
		Last Modified: Thu, 14 May 2020 21:39:05 GMT  
		Size: 71.6 MB (71643182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:e11922dc049aae05c8509bf9411a55afef1fe87906f77febf0de2831a7bbfaf0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71792936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0af930c2c542a675935b680e1dfe0a80397b44bb3229d191d7f8adb6fa34d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:01:35 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 20:26:40 GMT
ADD file:ea1e2b10a553d248e54503387c4afe958caa0ee09aee23be39a1ac295fe465a5 in / 
# Thu, 14 May 2020 20:26:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4c95d0f8fc948ebf7c0a53f5d7975591feb65f55189c1b7be7199682e6833f51`  
		Last Modified: Thu, 14 May 2020 20:28:15 GMT  
		Size: 71.8 MB (71792936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:be7b77539915626bcbfc13152c171ff03dd6dbfa72239d6c2b31367ad567e9c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78768915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d65ab49d340118d75b08c599c3fd49328477d9a9f2cc080055f1fab7fa068e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:42:50 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 19:24:48 GMT
ADD file:4e0cae3cc78df1587b6f6d959e15c020afdbb47e97e8eeb143232f1ea07172e1 in / 
# Thu, 14 May 2020 19:25:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:116dbb0ae4b42e0581b59cbd704264806be495971e3f6b6effccaf44e9518e1b`  
		Last Modified: Thu, 14 May 2020 19:28:48 GMT  
		Size: 78.8 MB (78768915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:da5ab2238f13a9189b1f4e167cb89bd8c475b0dffb86b7dbd84c369e00e152f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73791167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4323209fe15820ea8e5980fba4c3359df95e711b626590b4446108b816b0f508`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 22:43:17 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Thu, 14 May 2020 19:48:37 GMT
ADD file:7feba5175cb32e93786f5cddb08342b5383f22c968b77255705018d5efb97e16 in / 
# Thu, 14 May 2020 19:48:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:58d502d459c452899430ab5be4f1c4f85fc0c230d280618f53b5bb85ed808cbb`  
		Last Modified: Thu, 14 May 2020 19:49:31 GMT  
		Size: 73.8 MB (73791167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
