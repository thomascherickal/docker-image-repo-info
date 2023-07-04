## `debian:stable-backports`

```console
$ docker pull debian@sha256:6b5afec09155d6277740892b93169c1729e7d9a99c06a6c1827d73e99c15fab0
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
$ docker pull debian@sha256:9549d4169dffb69d5a6862f4ca9653fbcea632cfc5896f7a11b9e86bb07e198e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd641eccc2ffb64d9725a03c185c561c561a7c72dcca71c485fadc4984beb126`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:57 GMT
ADD file:2d80384df822d5fe48a3eb5a1d6e2813dab3ed51011f67e5359eca0eb3b24863 in / 
# Mon, 12 Jun 2023 23:22:57 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:23:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8e696805849a2e6064cfbff6bd7e8752c3955ecfcc394ce10f2943b69ddeae59`  
		Last Modified: Mon, 12 Jun 2023 23:29:01 GMT  
		Size: 49.6 MB (49552061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebba3624d174d6d8e8b8e37a83a320b88b92f69c5a33f722755b0ebe4bfa5b6`  
		Last Modified: Mon, 12 Jun 2023 23:29:09 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:babf895d3ea280fe191ecdf7a9932bcd705890639af081a7f569aaf341afbf1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47402957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2ac8f1bbe838c17afe4be2928b58147acb8ffff5d2749f24d5ab0a5d211217`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:24 GMT
ADD file:4560973449ae95ba135b1d2a4749ce4d278066080d92407b8fac46bc17e195db in / 
# Tue, 04 Jul 2023 00:49:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:49:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a1441b766c0384e637ebb6bcf7156542cf9e9a87c03d36822c1081d39c369d79`  
		Last Modified: Tue, 04 Jul 2023 00:54:02 GMT  
		Size: 47.4 MB (47402733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eacccd25a8db7c434c06efb03b120ad7f207524d6fe2551274faf715d3b74`  
		Last Modified: Tue, 04 Jul 2023 00:54:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:26ae0aaa0539df8eee4df5f60c72cdbb324536d7b7180001f89699cbe8855f0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45236446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8b5302cd8505b9d6fde743fb043d478cd468be6175f97f074cec44409a3f47`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:00:12 GMT
ADD file:79a37c77c46d6158e0050823174255b2fbd19b7b2a6321b195fc725519a2e82b in / 
# Tue, 04 Jul 2023 01:00:13 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:00:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0fbd4a02f7e9523396cfcce42fa09a0e010c6757aac4ee88a5814ba28b86e098`  
		Last Modified: Tue, 04 Jul 2023 01:06:13 GMT  
		Size: 45.2 MB (45236225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724686e9580217c87bac7f99dd29b7e9ff7ec915783bfb903225ef27183802c`  
		Last Modified: Tue, 04 Jul 2023 01:06:24 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8e9aef91ced7e28ac78845687dda565f56292fd52224a672ab81d767d74d5c35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49573325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87e6a28ce7cc70f731cd8d3501440f9fa1a461213225fc83e3a8b99deca4267`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:55 GMT
ADD file:76ccedd08f6076c61196ba172598919c5cb492a37200d89dc38b9ac64773c764 in / 
# Mon, 12 Jun 2023 23:41:56 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:41:59 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:201f12241830e10a2ee382f339d807e6172604f8f9a00cb5685eff7709e14726`  
		Last Modified: Mon, 12 Jun 2023 23:47:00 GMT  
		Size: 49.6 MB (49573105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a5bcf81b77c3602c55e08fc301ff326139f5843415e20f2d97698d72b26d2b`  
		Last Modified: Mon, 12 Jun 2023 23:47:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:44bdba25080b23c5d98a4f9e4ad7d4ec23476960580ce9e6d33785a0240651f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f4e368cb1efa9d87aa97e4acf049aff8aa880e990cf004b1b1272d0bc530a60`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:46 GMT
ADD file:f3b8fa150a5f56d1fb0cd028438a756c047fd1206e6f64adb7a5d07a774ff9c4 in / 
# Mon, 12 Jun 2023 23:42:46 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:42:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf1797067776bfc36afbe4cec136987ace6988740236fce395ed53c4160c32df`  
		Last Modified: Mon, 12 Jun 2023 23:49:59 GMT  
		Size: 50.6 MB (50562415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4565479e48d146414f89e6428a0ebef9712c8469cbe756e72ddadec557b76`  
		Last Modified: Mon, 12 Jun 2023 23:50:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:1da34b7cb372129ea379af1a13403db9bcd28207f77adc4508c6e0c8c901a4da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49541744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f92ee205fe2b381cd2845abd9a66c9381306cea557bba4f2ab2014876ba23d30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:14:21 GMT
ADD file:93ea736f2b2b41741de1c6ca3785d162c63a26160d3698c2add5f6558ca8240d in / 
# Tue, 13 Jun 2023 00:14:26 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:14:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:952682bb40dbd11034b55cb5306916fdc08a21bcdbc932acab150d9239a16e07`  
		Last Modified: Tue, 13 Jun 2023 00:27:04 GMT  
		Size: 49.5 MB (49541521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfce5f34a33137920bdf347c6acea432ec9fbb93713886ca2edbbe15e83034b`  
		Last Modified: Tue, 13 Jun 2023 00:27:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:aab9835d311d075ae9ae40eb2b570fbb0be73bed507ac72b084c82653169f7e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53536968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7de7cfd26e3a0d65d7f73bee7505ff0e424ebf4b8a77a43c58ababa8bcc3b12`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:09 GMT
ADD file:3875b90349a36444c097f6769f32b60747df7c851ef905a424ca63970b60625f in / 
# Mon, 12 Jun 2023 23:20:12 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:20:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:287c881a610dbb8ea39494c4b227f1ebca1d5c64ae09e6f374312ce5654be9e0`  
		Last Modified: Mon, 12 Jun 2023 23:26:52 GMT  
		Size: 53.5 MB (53536744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9adcef5e62612cd89146695b840336735f782e286de08ff596d44e114d2ce`  
		Last Modified: Mon, 12 Jun 2023 23:27:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:20fa200851441de7e46128c847ce816baaedd6c4f7627879d2bb1442d16f7080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47921826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e95475b03a07062f039dede2d536cdd10bb0fdfa787925d3df9b294604a8b1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:31:21 GMT
ADD file:e6c31ca69f32f487301af39887a5d65243daee02dc039b2b6d61b4f80e76f47d in / 
# Tue, 13 Jun 2023 04:31:25 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:31:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f8e437bbc64097b93d7e8c3fbfdcb94d6bad268266bf36102329f869bdd48916`  
		Last Modified: Tue, 13 Jun 2023 04:35:47 GMT  
		Size: 47.9 MB (47921606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eec4d3bb4f8fcda543dff7f55a361e6cfa093c7749b9078277b88475c49b94`  
		Last Modified: Tue, 13 Jun 2023 04:35:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
