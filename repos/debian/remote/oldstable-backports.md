## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:abc048b64bb21cd8256d652ce253248d8ada0c51603c1952088186aba74d1c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:85e201cd4b5e9a0661268899fb766cfbc905a3060c5f30c70b108837778aea88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b210fbc496ec238bad459f5d6616edd65acfa1e1c37941f64c01276471bc252`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:25 GMT
ADD file:4cb930e9734087a901749e455f5244654b460a84b00eed90eb1d9c2291bc164f in / 
# Tue, 02 May 2023 23:47:25 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:47:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2e82f76fc41ab7d9e1f846f491035ff27c2662e3d9df1310f7a469aa044f641d`  
		Last Modified: Tue, 02 May 2023 23:51:18 GMT  
		Size: 50.4 MB (50448700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be48503b426423d15697b120a1cea6fb2a6e9fb9359b3d777c0b409c158ef390`  
		Last Modified: Tue, 02 May 2023 23:51:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d6377fd8eaeee1f5f1cedfb7127edf7229b3ec15fce099cf57f19b77020290ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2792c36f822b8b77ec8a7a021b16c808e9937057ac6a8cc4373b7e3789acf62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:25 GMT
ADD file:dc05d2e6985860ec236215c4807bb9773703d87617c396fcf952fce1b03fcf33 in / 
# Tue, 02 May 2023 23:48:25 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:48:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:da453a52fb0ff3ecbf4850e32b06a4416f6ae0b031269f3698ca31fb45eed840`  
		Last Modified: Tue, 02 May 2023 23:52:30 GMT  
		Size: 45.9 MB (45916288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8891c5c7ab2fcaa53c5a039783c094c38d806d8682e05fb51d4e7ec8e1503e06`  
		Last Modified: Tue, 02 May 2023 23:52:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7d33839ab8727e4df057a53f1bd715fbd2312a2912fd6988091e24957ef9596f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49238866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79aa8c46ea3620bf367d93ead146410bd3350893c752263c66c4d449886b97ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:23:12 GMT
ADD file:514a65f521b1499e40d254739cb4e6b09e823d8765cf61fb6f27828e3327e9d4 in / 
# Wed, 03 May 2023 00:23:13 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:23:15 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ea56475286b82cf815aa665e668b303d75ccca035f62c1562536ea0009b0df7e`  
		Last Modified: Wed, 03 May 2023 00:26:45 GMT  
		Size: 49.2 MB (49238641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f87ce0855ffe2b2b8f10539c69a26352f4822f2a257246881179defa3be822`  
		Last Modified: Wed, 03 May 2023 00:26:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:f64442957058a9d46373c279c4cdf89284afdba3c002ce5b9711ede69ea967e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d72dae91cdb176387e4e927487ee5976b8a93c6484d188bdfc6579643939fc9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:35 GMT
ADD file:099b26e78227e4b857e7a408817ee87ea6b4e46cb9caa33ab6bfa2bee2586adc in / 
# Wed, 03 May 2023 00:01:35 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:01:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ca049d29cc6875c8001f0deebb87f02235b53510ccb460bd8e88e0d8d36e85b`  
		Last Modified: Wed, 03 May 2023 00:06:18 GMT  
		Size: 51.2 MB (51206180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdfec2cf3b848416006ee61d824335aa1547b4c2f90018901b3337b630c88b7`  
		Last Modified: Wed, 03 May 2023 00:06:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
