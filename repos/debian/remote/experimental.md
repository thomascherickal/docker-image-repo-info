## `debian:experimental`

```console
$ docker pull debian@sha256:0ad97f7b28385fcd31d3934866875f95697afd1cd4caebc9c5d9b5da98b66c5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:fc4faff077aeadd107f6d5fa759c3e1ddd2d3927cc16587379c0cfb7269a5fc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52340511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616c0bd1d54fd38e78576b9226a5833959ff331a4dc0f54f1c24037b03fe0a54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:08:07 GMT
ADD file:721780a83b9ecd1c3ea680c963dca8e8ecc345481bf807aa4dab082fc5322443 in / 
# Wed, 22 Jul 2020 02:08:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:08:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9760f327e5ea357a0446f3036ce75f6309673b69b16167e5cf89184fcf56f228`  
		Last Modified: Wed, 22 Jul 2020 02:13:06 GMT  
		Size: 52.3 MB (52340292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedf91c2851bbdbaad1cbef3750342726b781edec0a70d369a4ed6e0fb5184c5`  
		Last Modified: Wed, 22 Jul 2020 02:13:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:53c690972b9aee6a2da6561d4b2c5573b73013a1cec8c643b3167db688850033
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50310330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c261cb10e216bff3ac7059b5ee5ba58921e146d7db8514e834ea14ed6add79`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:28:42 GMT
ADD file:f160eb43f8519d63f02cb8c986f08ac4e34493cf7b9c997a50a1cf4b473fffe7 in / 
# Tue, 04 Aug 2020 03:28:52 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:30:45 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8417196b4b25d0dbe68d885fbdb3dbe911dccfe7243a47b6ec7edb19c0b673eb`  
		Last Modified: Tue, 04 Aug 2020 03:40:06 GMT  
		Size: 50.3 MB (50310104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1304b2503e7894e87582fbaf2825fef6c2c5500843315c3b7540ee5dd925a98b`  
		Last Modified: Tue, 04 Aug 2020 03:40:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:a306cf2d188f22e52e1e628b6829b6a8648a3783a92886490d4451f74499e3fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48083095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1222156beba1230e8b494e4bdee37245255093038bfba86b57fd8be6e9cfab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:02:39 GMT
ADD file:60d4d05f6e1335855bf7a1e73b0d06b72b2b97cd06baaaee75728e1d0b76aead in / 
# Tue, 04 Aug 2020 05:02:41 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:03:15 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3ecf6deadaa2d830843dac616e6791e9bc7d129be6066401e3ff5d9d6b255554`  
		Last Modified: Tue, 04 Aug 2020 05:10:08 GMT  
		Size: 48.1 MB (48082870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced2a68047527c89c1b83ec3f61f097dcd263f5a24625b9d4c88660e08b658e4`  
		Last Modified: Tue, 04 Aug 2020 05:10:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:460d599a218d561e6a80054274c5cde546324bc4bd43a875fea9ec5c4d4e236a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50751034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a44a175021f956584c863565355e1e7e7547836e614289d609af59809bd8ed9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 07:01:36 GMT
ADD file:305301b12fd36716f47341a3d8aca1f79f6dd3b72bcf527c0ff1d6e26ccac305 in / 
# Tue, 04 Aug 2020 07:01:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:02:06 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ec16dd9a3e137a732e91c640cd5b8969b8379fd0637f64ae1d75ee74ef1065da`  
		Last Modified: Tue, 04 Aug 2020 07:07:35 GMT  
		Size: 50.8 MB (50750810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af18dda4cd880be658ad3085d64cf39bb9d1e5cb6d2de3fdffee7068f9b6260`  
		Last Modified: Tue, 04 Aug 2020 07:07:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:9f3d842bc195930ac0ef698cb799abf58d9e1fd5db86695b791653c9519b3c3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53490602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e04c88bdc151b06be3d8d6ed1418868cf5321747bf0b235c60cb27a92b65c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:40:55 GMT
ADD file:002745dae517e6495edfa87687988e5d99a487c6585fabc3230544cf23d4da62 in / 
# Tue, 04 Aug 2020 03:40:55 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:41:11 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:28bd8d820f4effe1d6d9b47d3ae45c37b178357376debbce3b36a0e76b276a39`  
		Last Modified: Tue, 04 Aug 2020 03:46:40 GMT  
		Size: 53.5 MB (53490382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b844ef4ea57a45f8dc8ad1bb9622b97aee7a93f309560a7b4620befc3f494543`  
		Last Modified: Tue, 04 Aug 2020 03:46:57 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:242a36acef25373a3b7abcd9481e23324aee8b5e1dc091c83e6f5593f8917650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51146890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b48bcf37d6ebbff646f0c1228b2d21e288caad694ffa47deeb22cd612e64879`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:45:09 GMT
ADD file:cabc54924e7d8efcf5da7d964e11ae38e48625cd51f908eb05a8833f7085b7d2 in / 
# Tue, 04 Aug 2020 06:45:10 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:45:32 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f57d3adef193f736c46304dac2bd9143c6c125f99e72a3d8cf79c19a8f1aca6e`  
		Last Modified: Tue, 04 Aug 2020 06:53:35 GMT  
		Size: 51.1 MB (51146667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf46d63be921e4d4bad80e8f6c75e7f0f7d7d9c59f22563cb885ea0d2a38bc8`  
		Last Modified: Tue, 04 Aug 2020 06:54:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:0493f5502a7fb943b1c733dc270454176ceb3d409df757daaae4b94c4aa05919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56196988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6130a1109b0cad790f4ea5bb6d5079d93bac653765e4e86b8e6338e517fe6df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:48:16 GMT
ADD file:84e5acd8e8dda481d0f0f809cd601b85c2e41c60736b14ecd2462bf8342e6c30 in / 
# Tue, 04 Aug 2020 04:48:23 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 04:48:54 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:86d3defbbb312a5f09abc9482a18708c1630b5e641a9ebf202e0ab0009278770`  
		Last Modified: Tue, 04 Aug 2020 04:56:13 GMT  
		Size: 56.2 MB (56196763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92b06a5dfece4820322f8ac8b2e17f017e0ccc0e2d76543f39d196d0adfde68`  
		Last Modified: Tue, 04 Aug 2020 04:56:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:b97d78d7a3a3c05d6318ea98ab41d08ee7688483c5751e25bf0c408078f760a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50989909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cecec4fb770fe6058e4a9088ca9316b057428a5a41bc75b2785c6c951d10ba1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:18:32 GMT
ADD file:238775756e52141121b66ba51576ceee22305a02064e8261d22b3456f304742a in / 
# Tue, 04 Aug 2020 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 01:18:48 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1a10cec4db9a5323183a623bd9e0474e42e07ec7f12bb35f5241e88c12d5e0f0`  
		Last Modified: Tue, 04 Aug 2020 01:21:29 GMT  
		Size: 51.0 MB (50989689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393f1bb150f06b334cff987be5d2d8f1704d0244fcc5645876eef9e641e052ce`  
		Last Modified: Tue, 04 Aug 2020 01:21:45 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
