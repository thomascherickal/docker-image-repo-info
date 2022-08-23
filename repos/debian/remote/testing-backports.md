## `debian:testing-backports`

```console
$ docker pull debian@sha256:fb3efd0e54da25562bbfb516d179cab30a3c47fcbc4efa746c03549fe7c530b6
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:065300942d15b1ebc37d42fc9e6289d3314d074f9f6e177f01b1099abc8fbcff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52725936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975fd0fe254189d5a73a5f3caa63807c47e71dd3658dc1d2481e2ab73b979ccc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:22:16 GMT
ADD file:46ac30e868d9fa053938dfd03bd5a6d46502ac44f64d96a4c75a40348ab45066 in / 
# Tue, 23 Aug 2022 00:22:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:22:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bc2ca2f3fe9546b1f10765241eb47f197756a844ebd3f82ecb85477801779ba5`  
		Last Modified: Tue, 23 Aug 2022 00:27:47 GMT  
		Size: 52.7 MB (52725712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041ff16a1c23fe5925f1940b68819d80c38456ce721bdfab893552e8df3a1a6d`  
		Last Modified: Tue, 23 Aug 2022 00:27:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b55b1fe6dfdef73f5a1819aa408335a09842d47563fa35dc8065981c63281c2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51813177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d39af508475d719a173c664ffafb1b762868fd41544bd09c6eca5d80b04cffc5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:51:19 GMT
ADD file:fefd6319bc7645b06adc5a3cc3360ba34d8d5161bbf0e5099d6dbe791ca6ff2f in / 
# Tue, 02 Aug 2022 00:51:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:51:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:35bd703c054d143fd433e87c9be3d87896581f5d49d5cef9706e64f10f8645cd`  
		Last Modified: Tue, 02 Aug 2022 01:00:29 GMT  
		Size: 51.8 MB (51812951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee28164ac26bd12b6d3bfdf92ad9191796b1beb3bb6709c70a6aaee4afb2ac3b`  
		Last Modified: Tue, 02 Aug 2022 01:00:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:f5078cf6c62077090d8615989b70347455f6dcc0333deb3100510bdfe6fd40e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49527902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1294d63ab9c53a79984356618e5b4f346bd4cb7b84356e3148005ff44cd4ddb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:55 GMT
ADD file:5221fcdb61cb7dbb8b99d9e2475042bc115d4af4c9768a2a2ba1b6f0607ff29e in / 
# Tue, 02 Aug 2022 01:01:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:02:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3642840c9ce0a15019a46ef32c9f75784bdc0fa3431762d6d89abb0253e1d1ff`  
		Last Modified: Tue, 02 Aug 2022 01:10:33 GMT  
		Size: 49.5 MB (49527679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1705d78a40e54d9786cdaecfba036c139131ad6588bb3c7f87d0d76ff850844`  
		Last Modified: Tue, 02 Aug 2022 01:10:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:53224dfacc1d475ef70de7a821d170f645d3757b0acff9b8f95509fccfa54d0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53097677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e271fd753fd0f6af674c933fab878285cc1a5734c43e438436f0f7dc229ad403`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:19 GMT
ADD file:8309f8f759274ea54e9869e94cfc7314acc511bf22afd94208c9212647fcfed4 in / 
# Tue, 02 Aug 2022 00:42:20 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:26 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f4d21a79611b04991edb746aac3133d30f3ce393b36a5233ec78a5d1a940b4d4`  
		Last Modified: Tue, 02 Aug 2022 00:49:23 GMT  
		Size: 53.1 MB (53097454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471298f970fbf97a2fa1556fe46ff8fe4a4a5a3e919cfedb754080b5742a645f`  
		Last Modified: Tue, 02 Aug 2022 00:49:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:71861969a9f575d655dd8970e7f344b809459caac2c0f0b70d8594675b2d0904
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53974288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:020aa34f7c04fe3300d301b668c16b0771a76bd54b5fbc3b2029da91097c58d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:08 GMT
ADD file:90dad3d854300b2f1bb77145f76abaea2e0ddc867c4a7c016df5fdfd41f769b4 in / 
# Tue, 02 Aug 2022 00:41:09 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:15 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25171fbf3413be3802586f297db8e2ee841ca94ff0bf194ae2ad188cce56c0c6`  
		Last Modified: Tue, 02 Aug 2022 00:48:38 GMT  
		Size: 54.0 MB (53974063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3981419cc0f934b7dc182d248c6c35ca139660bc75e992b5ff16ac46e889fe92`  
		Last Modified: Tue, 02 Aug 2022 00:48:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:00a0b943ca8239fa64cf723d4582429321a5972222072cbe7405fa03d2c14cc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53119599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e037922a85e4a5eacf097d342491014b01d0d0920e6160ea6e286179cd7e93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:14:12 GMT
ADD file:f3e9e580221d3e94f0fb61e58fcbf318bc042add830bcdd71dd0983d138c3b0a in / 
# Tue, 23 Aug 2022 00:14:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:14:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d67983489079eeb3b8ecef40d659bc0761c151e192dc6a219e80b494d3ef1685`  
		Last Modified: Tue, 23 Aug 2022 00:22:47 GMT  
		Size: 53.1 MB (53119374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54e598f2f73878c653030f8a3e0d9ad2e90e0e2b6ac805e5f30e37094a4c9fc`  
		Last Modified: Tue, 23 Aug 2022 00:22:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:0729f3278e4b50a82bfb2dc3abf54c3becc271f504c5db3e9993502f20a24a2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57221991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be94cbbddf3c7a7c1aa4f2af4e11a590af77fd72035bd0a337c83e0430a9cdc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:8941088a90db67589cb3aab6915d2fc931aaacc65dab7cc04095d31a230e93e3 in / 
# Tue, 02 Aug 2022 01:19:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:03 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1b23178950ef7a327250a58d404509202a87d952f5f360e07e4510ab9ebe8d42`  
		Last Modified: Tue, 02 Aug 2022 01:28:49 GMT  
		Size: 57.2 MB (57221766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8851874edb53eeb2a26977a213db1c69cd745db362e3eca30c61bca32bccd8`  
		Last Modified: Tue, 02 Aug 2022 01:29:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:707996ccf2735568be16291762734f7d60cbb2d92e18fade969345a04c18306c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51514764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe05473727524549a15e8b501ddc7030f31dcb92633f299d95a8a0f67b26af6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:44:26 GMT
ADD file:14adc5a49c231f53b278b34139dc458d505fae39b33dd3ccd8f058026d67786c in / 
# Tue, 02 Aug 2022 00:44:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:44:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e87031236155e98c3fa5eea947cead096d1cbfe02f008ed7b25b5dc4e17795d2`  
		Last Modified: Tue, 02 Aug 2022 00:50:50 GMT  
		Size: 51.5 MB (51514538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45035e3c6d148b150c55c62898d82dbda3c9ac96a61d4b696949ba77fe1b1cdf`  
		Last Modified: Tue, 02 Aug 2022 00:50:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
