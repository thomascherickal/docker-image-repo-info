## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:482fa2ecbefebbfa1b3d7b668fd6f9fc742eda0a634b38a770e9e5da1aff25c1
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
$ docker pull debian@sha256:75fc4cc00444e2e76b75065a38c7b8dff968b74f1f692fd210e9205b9950f298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49238849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9c2c5a6dfc3f7e63deb92185f48adef050a061c6404dcf5ea66445ae81798f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:08 GMT
ADD file:128de67bd32a4087af0c3417150a0e6d911dc0d017943fd4c2d7ebfffc549044 in / 
# Wed, 12 Apr 2023 00:40:09 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:40:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:82e3c316dee591406fde11a61d53a1b814e23b19cc3ee139d59cd3caf9125df4`  
		Last Modified: Wed, 12 Apr 2023 00:43:27 GMT  
		Size: 49.2 MB (49238622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5be318b063fb257e05c24aa7708b2cb63fdbccf51f83d659d4eca325ab3f6c`  
		Last Modified: Wed, 12 Apr 2023 00:43:35 GMT  
		Size: 227.0 B  
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
