## `debian:testing-backports`

```console
$ docker pull debian@sha256:806c13ccdbcbc874b62fb466d23b205d0088854a497287552675d01d1ac27d29
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:236413a765cbef90ca6c7bddeba348c14e217d415b11702ca4fcb756f491d569
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51906780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8065143cb1f6539ef09d6aa46c8cc913b46fc0ad665fdee676d3935d0807735d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:59 GMT
ADD file:9b259b9d58cb55d3126a7ca20eeb5e20e8b26291fc1b738051ff61c8ec22bd95 in / 
# Thu, 10 Sep 2020 00:30:59 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:31:05 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4363cc52203477cd66948034ae4a1db71cbfd27fddb648dd9c590161de1f8634`  
		Last Modified: Thu, 10 Sep 2020 00:37:58 GMT  
		Size: 51.9 MB (51906560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a74a9b0acf6b54f95754eb6c285efc14676c62fd6b7133a547ba9be02388bd`  
		Last Modified: Thu, 10 Sep 2020 00:38:03 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a23c72d98f550df2eb3d4428d4ec1adbd35d303924eeb77ad6be802eed920767
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49868342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:492fb4df30904c0e45ffdfadee87628c2bce6e33e1ffaf37a9582f3c68e212cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:59:06 GMT
ADD file:9d89e1d07fd14d8ca04ca47d6458c33d8d9f2ba0c3c993500d68aa22fdc91fac in / 
# Wed, 09 Sep 2020 23:59:10 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:59:19 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7ea9bc60ea80556170fc26b1e9b97badd365d415d8fc11db6b1f99a1d9e9b5a2`  
		Last Modified: Thu, 10 Sep 2020 00:07:41 GMT  
		Size: 49.9 MB (49868116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7c3194d65629bd9d33474d8b0d1dab35d919d281c75b90a733f0d3a686dcc7`  
		Last Modified: Thu, 10 Sep 2020 00:07:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b8206fe794a3c46d0ea01da5f16db1c96ae333c1606b1b0474c24cf46be2ff08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47622798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1209b97465fe070dab075dd306bb69e7a5fc1bd1af3173de2c513834e4b2b0a1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:14:15 GMT
ADD file:7d1699b0b544ffe1ea1fa09cfecee57370e2ded4c7ff50e0a080b9eaa6c574a8 in / 
# Thu, 10 Sep 2020 00:14:17 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:14:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:67f8b669b5049480f56c6fcad559f7090c9d5c691076d2136b7a479b7d84ef2b`  
		Last Modified: Thu, 10 Sep 2020 00:21:56 GMT  
		Size: 47.6 MB (47622573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860bc4156d1ba368e423545734edb0dd34eb8c0b53d60fc00dda2b9b02a36ba0`  
		Last Modified: Thu, 10 Sep 2020 00:22:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:300f1ecacb7ee6f87c1434c7724727197c8b64c52f34376874061c6e6fc0e04e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50825622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9826461fbc94cd354f2d1bb1f808cd9a96a59643e91c8d289210a77936526d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:55:28 GMT
ADD file:5dde8e807b0c71ebc7645a34be11d591e22056828b80451cd10b4e9e43d50f22 in / 
# Wed, 09 Sep 2020 23:55:29 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:55:39 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c3a3b210b20418d18407956d6d337463c452a063f31e10abcc972012479278c3`  
		Last Modified: Thu, 10 Sep 2020 00:02:26 GMT  
		Size: 50.8 MB (50825396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3de77037f2b9ddc9eed52858d15bc8761a082f044b3ebea379dd40e94e02546`  
		Last Modified: Thu, 10 Sep 2020 00:02:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:5acebfb2bf1c4eeaca6940152e02c0bb595cc4a4217721b75648def79b587c38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52969438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1414237291556ce015f93152eb146f4e00dacfd9c113fafd5c6ecaca61886c1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:44:06 GMT
ADD file:4717778122f15030613353290d420e247c19a07bceb732acabba3bcde7fcc61a in / 
# Wed, 09 Sep 2020 23:44:06 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:44:13 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ed79a4c52f758fe2a1dbd3cdc139b88fb1077c3f9938e63c0c0906b422dc1869`  
		Last Modified: Wed, 09 Sep 2020 23:49:26 GMT  
		Size: 53.0 MB (52969215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1016dca81137783ae3acb4181fce788a0a411797e73e8bcb4c5f4a2a2d397e`  
		Last Modified: Wed, 09 Sep 2020 23:49:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:c9a1b4420dad423628e6ebd6f69364984b4bd22bacda45056c98ca9ff88ef989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50550999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc551cb77ec5d96f55b00c307649afb2bb9f7e2962274950c078fdd45a9ca49a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:44:20 GMT
ADD file:a53836046b0070207f3bd1a278810d10133a25b6349c816dccf4b727a71faed6 in / 
# Tue, 04 Aug 2020 06:44:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:44:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3a0317c61d2d4f59c9c7065c26ee123ab008467a8954cde60d1d216013fb93c7`  
		Last Modified: Tue, 04 Aug 2020 06:52:09 GMT  
		Size: 50.6 MB (50550774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc0fd2bf7883f64c62cae3e1e3fb5469934bbd84462e1d01ee3bf8fb055a0ae`  
		Last Modified: Tue, 04 Aug 2020 06:52:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:09d236298bc6f86d098c570277f2be47bafcd4a1e40ab7aa8c71bc0ff2a6524d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55774643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3036e7f9cba22bd88926da1c64128aa15b714d68a458d6c9fefce5eaaa006a63`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:14:15 GMT
ADD file:1ff1c751892adb35acbc76e9c216d58059214a72e719e3789fb186911933fe1b in / 
# Thu, 10 Sep 2020 01:14:26 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:14:49 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4f06950a568456590fe3afbc7dc70475d0e9ea33f4901b4085b036db8288648c`  
		Last Modified: Thu, 10 Sep 2020 01:37:32 GMT  
		Size: 55.8 MB (55774415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a31ad48fc06109043b32f6c2c3bbb884676c2d918039aa158cb2e175cc5d4`  
		Last Modified: Thu, 10 Sep 2020 01:37:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:691c5fb27557a9357a3d942fad1fe36ef7d3dafc327029c8a180e93ccd93354c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50468804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a5ed621a18dc4431cf154e7807c4a23916d949f291f1b479c8e799796fea42`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:44:10 GMT
ADD file:6096c49e1a6995a7f589f5da5b267e3a4fecf47837fd27ded6c588f594eaf41b in / 
# Wed, 09 Sep 2020 23:44:12 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:44:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d7d204a73067c1e080e9483323a8740a8fe61e942328a1b2ee230a2df15dd727`  
		Last Modified: Wed, 09 Sep 2020 23:47:28 GMT  
		Size: 50.5 MB (50468580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66cc75c5ba8cb0753b03bf94e84fef77e0e2e4a8f742a7287172f4300905c86`  
		Last Modified: Wed, 09 Sep 2020 23:47:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
