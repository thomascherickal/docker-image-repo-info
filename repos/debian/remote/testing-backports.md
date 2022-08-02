## `debian:testing-backports`

```console
$ docker pull debian@sha256:97570af555776835abf7aa60e6a253a2a5a95a8f4a4d280a4cc08a62cbf602b1
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
$ docker pull debian@sha256:d3529295b4a93fc688e56891f209be9dd054e15239f21996a0ad546654fc59e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53022542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9306f3112609fd2cb1be7071511c2c1c32becb3ffe41a50669c7e7ddb65f90cb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:51 GMT
ADD file:242a7253146210771956ed1bda9124125835ad9e76a50d745d06b34fbf5e50df in / 
# Tue, 12 Jul 2022 01:21:51 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:21:55 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df98203a8b21cb36e308dd353908ed338642491ef167d757bebb3297146a77a4`  
		Last Modified: Tue, 12 Jul 2022 01:27:27 GMT  
		Size: 53.0 MB (53022316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55606a532f98e4de0863bf1b4c84621d9149609bc2c7df29a52d5ce2c81109`  
		Last Modified: Tue, 12 Jul 2022 01:27:36 GMT  
		Size: 226.0 B  
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
$ docker pull debian@sha256:e04d3d76cefa9894eeb7fd9c5ec992db6ba7cac086ddcbd78c55d0130e3b9aee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52148484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c4dce7b040f3a8faeec2113652dfda1d57ba5de17bb92ad8af315618d7e693`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:46:23 GMT
ADD file:cafc20a19b7a947f5cebaa2e04c5fa4dc96b0580d9a70a92068aaed8a19ed722 in / 
# Tue, 12 Jul 2022 04:46:28 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:46:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:311579db3109ad3829a7cc600da26fe8f56d9ed46e904060a08b655b56a8a2d6`  
		Last Modified: Tue, 12 Jul 2022 04:57:22 GMT  
		Size: 52.1 MB (52148259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270387476bb72e24b888e96bec6b0501477db1a1856b866091c97de47163f093`  
		Last Modified: Tue, 12 Jul 2022 04:57:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1fabba15fbafdd0458418059d64c7f6b6b2b7957e40e8f8e19fa40785c398e5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57237826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309a1a57b178af283a61ee2399a9a988cc47e84a9d0823de5e9d2874315a9314`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:29:05 GMT
ADD file:50749df5dfe83d67bf06b74c10d8d4c0b6c50902fb0b3fd4b1e944bb4d04d838 in / 
# Tue, 12 Jul 2022 01:29:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:29:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0a914d717e21264ea59989c5b8ee06609e61159738242df44dc331a1146b94b4`  
		Last Modified: Tue, 12 Jul 2022 01:43:45 GMT  
		Size: 57.2 MB (57237602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78e09d38971941c3b2dee93582be52ac3ec39c79eafc1946be46d8bf478b917`  
		Last Modified: Tue, 12 Jul 2022 01:43:57 GMT  
		Size: 224.0 B  
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
