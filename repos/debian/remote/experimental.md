## `debian:experimental`

```console
$ docker pull debian@sha256:3c75b9a68719384f1af49ce7f63b09d0fd67e07c17f6cdac298700f0d3121bb9
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:92914112fdd2515dc5245c482a1dce4b657bc6530a929841b53163f8d38376ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53231770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ac843354230700447f24fdea80134c0cc3206b4e37685c6eb17129c659bbcb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:21:49 GMT
ADD file:e1ccd9ffcd946929280f13a1fdd8453422c372ec5095af01b7582fe9b94b134d in / 
# Tue, 02 Aug 2022 01:21:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:22:00 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1af40c44782bb0d73ae2ce06f593a656ca94f129c1cfa942ac79d1d0fa34f32f`  
		Last Modified: Tue, 02 Aug 2022 01:27:42 GMT  
		Size: 53.2 MB (53231550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa039adf7b12797d7ee69e807aa415d804a1c885a8567e5722867e7bff2d17be`  
		Last Modified: Tue, 02 Aug 2022 01:28:05 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:65bda137ef63b6b3b342e7c9cb06b77a4f717221fddbf5842a778f5cb8ecbb2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52021628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bf43d48b8acb770ae16c12f63dc174ed8451a2bbf51cdf58f0945107a3345a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:51:50 GMT
ADD file:8165c0d978757c272b0fc9aab3bf8bc8644579a857290a6ba3d25f5e06be2ad4 in / 
# Tue, 02 Aug 2022 00:51:50 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:52:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c32afc4cc9c9df6d376376afbae71bc1e87837dd8838c5d55f5854ba7298b657`  
		Last Modified: Tue, 02 Aug 2022 01:01:30 GMT  
		Size: 52.0 MB (52021404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13804901e30c4db3bf34c853bc1b62a7f18ab26005b2da85a952728ef852af2c`  
		Last Modified: Tue, 02 Aug 2022 01:02:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:47a59dd79c99d0396ea8c2319b0b2804dd4227a552e2df587e27f9bcd36ca001
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49735552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9344370ae235d094c05fe6ca1ae1a95fa40393664f3dad7f4973cad5f528e447`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:26 GMT
ADD file:938fb1d62b5f37e34560628bf97a9d4b02fe5c41d5aa62171e22f61fd6820e14 in / 
# Tue, 02 Aug 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:02:41 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:25465063d4ddc9b103f13125cd4fdd8eb57bdc4e5ad39afe15db8f828d80d508`  
		Last Modified: Tue, 02 Aug 2022 01:11:16 GMT  
		Size: 49.7 MB (49735331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7071ec524d8a3c1f295379d1a6441356a595ace9a7c3a0f8e065b61cd265975`  
		Last Modified: Tue, 02 Aug 2022 01:11:42 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:58e8138be5496b8e39af0d52a9560cb08b32ea8408971b0d687c37e81d337eae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53312003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9881d82d4e8ede46b1c4a370dffaa02c73b4e485e347e2bceb4c97cfa162b26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:43 GMT
ADD file:f319e3ad56cdacf4f559c33e21c65bc34192203c7cfe561c49951febe8d41d11 in / 
# Tue, 02 Aug 2022 00:42:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d7f89fc086c7d917b11f43154b1526ea2314922b905525b6bd85dcd4b7ad7e96`  
		Last Modified: Tue, 02 Aug 2022 00:50:22 GMT  
		Size: 53.3 MB (53311783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2758a8c5115b90983ff91e9450cf9b37718bc7dd5da83f326213a388a9526`  
		Last Modified: Tue, 02 Aug 2022 00:50:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:9c6767364508033bf234cf39b17b6eef7285da5f9a70091ebba1620033b1d277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54195289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9542ed6f00ef909f4d84470f0a8f4cd531f9336da9b31ef20d1e76173bdc5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:33 GMT
ADD file:86aa5ea5e610e7d9bd402025a337e0f305b103598be63b78b6b0cdea7a3df4de in / 
# Tue, 02 Aug 2022 00:41:34 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5699b5f3fd16f897714b4784f589776f740c6550b1714d3050d6370b669db263`  
		Last Modified: Tue, 02 Aug 2022 00:49:25 GMT  
		Size: 54.2 MB (54195065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0841e5987f50cdeaf45bf3836fa418307c90a4e91ac439e2fa3451c95b330918`  
		Last Modified: Tue, 02 Aug 2022 00:50:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:f8f65b765ed22f4c8a4e1e4f6219065ae0594504050a343fe22004adfc8bd1db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53306201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aa78c40209069477b7b835eb68ccaa20157f50fbea21024cdd88f859c06828`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:16:50 GMT
ADD file:94302ba72cc8cc0f6c7af918826d11ca5bbec2b84a09539af388d185fbe71819 in / 
# Tue, 02 Aug 2022 01:16:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:17:37 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c5ab9923f233d5341bef65f0365d352048771be65555262282517754d4cf560d`  
		Last Modified: Tue, 02 Aug 2022 01:28:09 GMT  
		Size: 53.3 MB (53305977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9242a5aa5a3926695d8cb8926e8f6e3a7ca9636e76f9ed8e75a79a8bf3b580`  
		Last Modified: Tue, 02 Aug 2022 01:28:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:8ceabf78899abd35ed519aad4d1dd26b176bb7fe4baf0bc6d0eba73dded0ae4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57440435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c42cf3beacaf18a40e1c51df95e38a13aa8ba31ff28414e192ea25b98aa5e439`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:28 GMT
ADD file:00f45e966a1bf81446cdb8892a3b57307803b4b3807e49c2216eb498d072aee5 in / 
# Tue, 02 Aug 2022 01:20:31 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:85140a3e683aba1b971bf67cd28210279f0d3da9cf83b37f47047f37badf66f1`  
		Last Modified: Tue, 02 Aug 2022 01:29:43 GMT  
		Size: 57.4 MB (57440211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe215d99685d0bf9c634711ca259fa19427e5788734d2972a6baec2e58df978b`  
		Last Modified: Tue, 02 Aug 2022 01:30:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:fb759c822a2a767236c10ce97f17200cc4f9e3233a016de1bd66f34fa6d1c3c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49420292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1350a73f116947137db366cb2158837da9b0987fe754bf5adf17de5e74c290b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:42:00 GMT
ADD file:5d7cde1610e3596cc6e5bd6e2709d2da5498a84ce4dc1cd58875013d036ff722 in / 
# Tue, 02 Aug 2022 01:42:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:41 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:17c85bc27a231cc71d33c8a35b65c89f666d96b93113889d22ff15d71c555006`  
		Last Modified: Tue, 02 Aug 2022 02:00:29 GMT  
		Size: 49.4 MB (49420063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9240d62cb2c78e90e11cc34834b14f173ca2b931d17f057e7921da39d4753e`  
		Last Modified: Tue, 02 Aug 2022 02:03:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:2cf3bb5edcdadca734a6b4cbdd3512205941b22d6f79ede0aad35e46219c3579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51734886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a25d77266bb510f6a354a417d2426e60d538f5f05f61e1e31267bc62cbe9c64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:44:54 GMT
ADD file:984d42e0d8c3e13cf8d8ee6608f0302c63c5b967b172fdcf3761d14a4b52a4b9 in / 
# Tue, 02 Aug 2022 00:44:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:45:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0185da9188245470949775bd4011291c882eedfed309ae9f441a1037dcf027d`  
		Last Modified: Tue, 02 Aug 2022 00:51:18 GMT  
		Size: 51.7 MB (51734667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4138c8d0e1ae99014aac269457329e461183d106799474d741363678a97449f`  
		Last Modified: Tue, 02 Aug 2022 00:51:35 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
