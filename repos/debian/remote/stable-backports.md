## `debian:stable-backports`

```console
$ docker pull debian@sha256:6fd5844361c05c624b56ce4b9d48a2e40757ccac85b0088da2eab7962aed792c
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:44df27f451fc4b74ba866891dabbc79ddf8636421405699797b9dd85389f7303
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55041535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5b553020391c64a7775706b31a75c52b71ff648c1b9916468de539993be3a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:22:13 GMT
ADD file:34ebed4832a7752758a57e6d077a2eedb22731d166f8b77e0b9f0339512d0705 in / 
# Tue, 06 Dec 2022 01:22:14 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:22:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:19a59d88084261156beed7ac55ecd91558f40d76259b7e7cd7173d88e6d3ab72`  
		Last Modified: Tue, 06 Dec 2022 01:27:09 GMT  
		Size: 55.0 MB (55041313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d179f63ba7e30fb3d1c5c5319b60be1d59660909942493af3132f51c1c9f295`  
		Last Modified: Tue, 06 Dec 2022 01:27:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4437d971e6c7bb5a01d2b1e01e6fc9a4de212f0a9c38093f8a4a4d5e5a156e0d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52545029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e5134f54511de2879c6dad2b3817906a4f47157677bb29eb69dbdcf57fe97ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:50:05 GMT
ADD file:59fb9d758fc3ce22925cad8c3e6656e994e9fae9a37f70145cdc0219b1fbd2a8 in / 
# Tue, 06 Dec 2022 01:50:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:50:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cc47e2cad097381f4c9183b162a2981f5606b7863cbf8a89175d2520e9bff8af`  
		Last Modified: Tue, 06 Dec 2022 01:55:36 GMT  
		Size: 52.5 MB (52544808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa587e95c1b265fc5d3923b8ea89d27342f5a0086275b1144aa9b2a26b7568f`  
		Last Modified: Tue, 06 Dec 2022 01:55:46 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:45fa1daa8441f3c2d7b3e15a99601bd2f64f0734cf4f1366035996db44131e27
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50207278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce5d80913f2e885a6f0cc754adb8f416b385b680621fb64cdf12be35262c007`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:00:44 GMT
ADD file:34f9baa882dfd11b8d0ee9cc3d1c369289f5d47eb1f07aaf8d8b18eeea6477be in / 
# Tue, 06 Dec 2022 01:00:45 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:00:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5d1b0930d4cad36cd9f85cc4f500e9c114edc3ba6d1080757eaba32a04c42d53`  
		Last Modified: Tue, 06 Dec 2022 01:08:32 GMT  
		Size: 50.2 MB (50207056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1272971beef6038619d65d41bd206309b4ac86e92592f66c3fb0adeb44ef6c`  
		Last Modified: Tue, 06 Dec 2022 01:08:42 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:97391aab8dc58d0ec6e265e234e917eb78375c94741fa61eea0aa5718ef7ad7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53699371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cf2eb596d94142b2cfea019cb3933f50849c103e2db3ddfb2e46e5d42fc26e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:13 GMT
ADD file:758ca4d53492adae96ec2aaa1ea3c794f43083eca557a2e01e8b81d915c02ceb in / 
# Tue, 06 Dec 2022 01:41:13 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:41:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e5c57f815a1ca5f6cd30e9cb0cc0d6870e7cc286ebb9a31541929bdf11ec4516`  
		Last Modified: Tue, 06 Dec 2022 01:45:48 GMT  
		Size: 53.7 MB (53699150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66f136dd30c52769c1a05666de1b74e9914589618c6a515c3a816c99098d48f`  
		Last Modified: Tue, 06 Dec 2022 01:45:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:6ef61ca0efebd5b94e489462729b6c50435b4a976462bad5559050b5d6769883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56022608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c0ba455953e6686ec0a1d88e4391726f757078341251d51d9d6433e0f2c4c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:26 GMT
ADD file:a443dfaae8d0f9292fe3697cb02f3ceb3749f79f691672825ec5f3efd7fdd674 in / 
# Tue, 06 Dec 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:41:33 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bd17635423722978b706617da5ee23821e711a5c6e21efa6abc76d52fc979193`  
		Last Modified: Tue, 06 Dec 2022 01:48:04 GMT  
		Size: 56.0 MB (56022384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bdc3851df8e3b153e143a0334be4ab12c41f41c27d0bd644f415992b24d5d`  
		Last Modified: Tue, 06 Dec 2022 01:48:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:6112e847620bdc8277baac4d100a0b4a45500c0ffb47f76beb4e2f82d4b753d7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53260834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46da262e4e9b4cf3463f2db39c77987dcaba8224a8decaf03117cd987043dfd2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:57:15 GMT
ADD file:879ab6f79e2fb8d3fd17adfe0473c543a636d57831277f7d7f0626ea24e560a2 in / 
# Tue, 06 Dec 2022 01:57:20 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:57:30 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6634ea6ae10263eeb0de0e54f17261eb4245a26bfcb5e1a46bcb04ed57e6fc6c`  
		Last Modified: Tue, 06 Dec 2022 02:05:32 GMT  
		Size: 53.3 MB (53260610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b8957c5de9e1d401c198cc62df9c1a2040c537895d315499c07ef4adb1b51a`  
		Last Modified: Tue, 06 Dec 2022 02:05:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:c46cdb75d221fa9c49602241b584de73ab2dfa71ad06612068cd1d80ca3b7ef4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58913350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49a33992f80fbb6a25db4f6d21c87ea0a109850bba6a8171829e2da6289cec9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:19:04 GMT
ADD file:52359c01b57648275662cd3780e749e801fc2fb35889ba101416aa560bd9dc78 in / 
# Tue, 06 Dec 2022 01:19:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:19:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9e0e7d92200dbf05b61c73eedc3538266a8a5696ba36cd3dde0f961483c6415d`  
		Last Modified: Tue, 06 Dec 2022 01:25:31 GMT  
		Size: 58.9 MB (58913126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e2a8187360c6dabd2599e8a325cc05890d32c24f6510a650f7792a00a6f728`  
		Last Modified: Tue, 06 Dec 2022 01:25:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:372b4b1d7683abf5e4e66dfd35b24199a36e7119953d034cb7f0cb50682db1e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f7277cf0c011a02c82540fc2920ec52c2893b612b29891aec10638ba4bf9f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:44:04 GMT
ADD file:8c4ea37efa7dd75ec75b961a8b78219f331b5e48424492afd8d42558b16f9dd0 in / 
# Tue, 06 Dec 2022 01:44:10 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:44:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9fe7412e88822f809fce61091bc947285ba4905570a884732c61f03a6ed3354c`  
		Last Modified: Tue, 06 Dec 2022 01:49:25 GMT  
		Size: 53.3 MB (53272907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fca5abea6f5f2b3a43805b8e9d8559d74d3c5a7207f861c7f618a157d3b704`  
		Last Modified: Tue, 06 Dec 2022 01:49:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
