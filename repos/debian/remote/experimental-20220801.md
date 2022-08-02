## `debian:experimental-20220801`

```console
$ docker pull debian@sha256:0f4637732426a80a7bc76c6cd3bddd18379c6dcf6c4b23ea99573a49856b2540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `debian:experimental-20220801` - linux; arm variant v5

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

### `debian:experimental-20220801` - linux; arm variant v7

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

### `debian:experimental-20220801` - linux; arm64 variant v8

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

### `debian:experimental-20220801` - linux; 386

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

### `debian:experimental-20220801` - linux; s390x

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
