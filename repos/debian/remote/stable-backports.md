## `debian:stable-backports`

```console
$ docker pull debian@sha256:9f370179faaa68c318ead136c0769f675331e0c43f4076218df35325e1f1ddd9
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
$ docker pull debian@sha256:4b7100b67b57c579b07e1eaab7d1b5400cd21e644292e63675b1d660a6d66d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55025365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b738a931fc351e539618c7c653286189471093ec0e9866ed48d1889e480275`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:21:39 GMT
ADD file:d9c343f4dfe91e0e31ff144c5418c1ed52aada034a440c32ae0cf296c0fa9d5f in / 
# Wed, 21 Dec 2022 01:21:40 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:21:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:68be6800823f00619f0eb565e96687c02b92276176d6b9f8343d4051b74fff46`  
		Last Modified: Wed, 21 Dec 2022 01:26:38 GMT  
		Size: 55.0 MB (55025144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed7e1bb5912023bafa0f14c45871eb17eeb96cc1b85c250edd441c88d9cb56a`  
		Last Modified: Wed, 21 Dec 2022 01:26:47 GMT  
		Size: 221.0 B  
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
$ docker pull debian@sha256:9aab52a589fe9adb13fcae676a04bfae7b99c57300e7cc8a700dc807dfc78502
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53245305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff1625ba8424f4f61766c62a44446a217c11a7d2208c23a61833205b56486ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:12:11 GMT
ADD file:c78307398a21ca1a1eb99dad7c1e47578e8459d4a935d7f9d83dba7df1982d97 in / 
# Wed, 21 Dec 2022 01:12:17 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:12:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:06854a7b3b78f7102b75c303383d67d86ada6d9dff67c9ee5ca3200abeaa24f6`  
		Last Modified: Wed, 21 Dec 2022 01:20:35 GMT  
		Size: 53.2 MB (53245078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c90e6970b771356c4b72159d74bf6b3a025f3cceac9fd0f3b8747958bd15dce`  
		Last Modified: Wed, 21 Dec 2022 01:20:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:2ab361d2f1462eff62998668becc3a16cf51cdd45e465c97b1f845a724324fdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58897292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8eb595f963d86a2e03d4acb7d1ef9374d1a4e526bd789c511369845f5ae968`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:18:31 GMT
ADD file:da548841c930bdff2631803f71e8342f09fce4bef48c7ee19db898e27a783063 in / 
# Wed, 21 Dec 2022 01:18:34 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:18:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d49780a65e59eb79da041fcde3221638d4bdbe77fe9f061d5314ccad957b043`  
		Last Modified: Wed, 21 Dec 2022 01:24:34 GMT  
		Size: 58.9 MB (58897069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23d611550b60cac2f25538cef1b6e6367521bac888d980205368deb312cd06c`  
		Last Modified: Wed, 21 Dec 2022 01:24:44 GMT  
		Size: 223.0 B  
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
