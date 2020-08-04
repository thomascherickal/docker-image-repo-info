## `debian:testing-backports`

```console
$ docker pull debian@sha256:d90e3b8cdb393862c09fead654c4446af09558ab6297c51620fc565a11cfcdc3
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
$ docker pull debian@sha256:ae3b9eb2947bcd89648ab9b14b1c67d736e1f6b247743c0966e81d24f7f2f35a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54102749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0575c221e2cb39bbf3ea7456b42551564b878315035ba6aef45885607898f499`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:27 GMT
ADD file:f87e67a50d51914c2d4d77ad9fb2395ec8f720b21958111ea5e493ea7b788d12 in / 
# Wed, 22 Jul 2020 02:07:27 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:07:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:73b408cb748b0d1dd55d6ee6f4be6beddeeaefef08a2f1733d219cfa7c8eaf22`  
		Last Modified: Wed, 22 Jul 2020 02:12:41 GMT  
		Size: 54.1 MB (54102525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f72e30863d53058c856c7b0f2fda777954df739578ba0dfb268ec1d85acfd0`  
		Last Modified: Wed, 22 Jul 2020 02:12:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a2cc3c61b5465f2e3864b836a4a4ea018f2fd411a6a7971ec71509a6ff886f7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49784730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bda10c44cb33e62a133ad0f79884e41c2c45caac32d10fadbb10fae58ca8d41`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:26:11 GMT
ADD file:187c521285de33d9024f13e882a0a77eb73fa40812d206146aeb6ffee3b41d93 in / 
# Tue, 04 Aug 2020 03:26:19 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:27:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8aae9c3601b98cd2570242d799d9ee7afb8c97a1007181ac9ae997042c2d08b3`  
		Last Modified: Tue, 04 Aug 2020 03:39:19 GMT  
		Size: 49.8 MB (49784505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9731bb2fbee23630f5645430701e408633f38b3e0a3eff143404abd5cf00c36e`  
		Last Modified: Tue, 04 Aug 2020 03:39:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c13d981aaa6f0876c9c686ee1e5f124b6a0d3246b53dc2c44537b8552d0bc7e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47570702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4eaca4d22fa2edd4d94e6f75e27175df72c18b4a7355220e3b4c79e72c8387`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:52 GMT
ADD file:c87cca340a64bf8c47ea42d353b472eba58c679d0346ca265ea40e979d8adc8f in / 
# Tue, 04 Aug 2020 05:01:54 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:02:02 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6de6f46d5cde63d39bdf0307e4aca1b00858eca00dcdd17496279110ae989555`  
		Last Modified: Tue, 04 Aug 2020 05:09:25 GMT  
		Size: 47.6 MB (47570478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34156550e93302068ca3a8aa04b9ba4643af4343fef8f7419717aa6bf10c2d3a`  
		Last Modified: Tue, 04 Aug 2020 05:09:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8e5b52b11297053536f05db76a56bb461c4b01752c49da06f7e5135de24840a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52886612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae35224232a4dbab6a55829918358ee0fb21b8c52d8833a7e8cf59396417bd5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:44:29 GMT
ADD file:a9b119b35a33d56fcb58f91ca0224992754db12e0d3b07747c62963bc14659c8 in / 
# Wed, 22 Jul 2020 00:44:32 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:44:40 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3bd06a7da77e986d495b6461507cdfdd810e88d105914958d9602ec1c748e59c`  
		Last Modified: Wed, 22 Jul 2020 00:50:38 GMT  
		Size: 52.9 MB (52886390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975caa11307587ff7b517f133d2aab897aa065b4912de425edbaf12e649b4e24`  
		Last Modified: Wed, 22 Jul 2020 00:50:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:7dfc7661280267803ab00a0f46399357ddca4e879c7ce7f7402cc61eba12e2c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52909923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f233e4f2ed10742f1784c7cdb1d70498d2314abc4200142fd3ebf17c1817b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:40:26 GMT
ADD file:37d069bc693b5dc1cf3f5afa51967bb38b27e28e870341db5d25eee7577a3c38 in / 
# Tue, 04 Aug 2020 03:40:26 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:40:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:12dc0ff6b6c89bb67e2fe16bad31f939115457037b3e5b626ac0a1fc9a1d54fb`  
		Last Modified: Tue, 04 Aug 2020 03:46:09 GMT  
		Size: 52.9 MB (52909697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c31a0415abd39f740f099f54b68250970a832bc7a0c6dd2c07d19638e1e384`  
		Last Modified: Tue, 04 Aug 2020 03:46:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:161d5511764a45757fb64fbc66942a0b87783b4d3a2efb242b05ab84e94b5232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52358461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d19275715372f216365dc5b67037dcf0450c32f38723e7ed44fb98681f46d16b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:12:10 GMT
ADD file:6170f72ada5d54a8b7725b870aa32e806e97d30933df763c1dc542416c33f968 in / 
# Wed, 22 Jul 2020 01:12:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:12:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:babe0f7eb7118a9688658059be0e678998946b8d163e6b35731280563ea134b2`  
		Last Modified: Wed, 22 Jul 2020 01:20:08 GMT  
		Size: 52.4 MB (52358238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8722ef5676fe8b8a672e963b63c8a4d9834887ddec0ff03c83e9426e81fc4f81`  
		Last Modified: Wed, 22 Jul 2020 01:20:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b4d26727d87d305166a5a928f7d79740a7dd52d0d209b3f548924fa90390eff7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55656136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78805455d57b37879b9217945a4584a9f0a71bea9ded801e9ef7ca3ca35acc65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:47:25 GMT
ADD file:9716ddb36e63999f28bcc07b306d92cd35c4756a6acde3756dbea757b729c977 in / 
# Tue, 04 Aug 2020 04:47:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 04:47:44 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd5f9f7e65334c771d2f0cd8807ea5d5471b03ab32cd37132f270f6823fa6f2a`  
		Last Modified: Tue, 04 Aug 2020 04:55:20 GMT  
		Size: 55.7 MB (55655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b474f6d62bf8aea2bbe1eea581efe6282977066d7245e4700fdb02efb4c679`  
		Last Modified: Tue, 04 Aug 2020 04:55:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:c106c833bb51628dca35b6953d6eb5ccf8ea2e4ee94a5f24e24fbd0a72ffad65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50416994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f077bfea59d9d68ec196db0dbc6b46607dfc48b2e45ae2efefffaa2c429e253`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:18:08 GMT
ADD file:87c6bc96e112611ea9270b13a2a63f740c69d75d0d16c0633bfefe826cd3d1c0 in / 
# Tue, 04 Aug 2020 01:18:11 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 01:18:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:427e125cbccb0b2c09e8ac1181fc23797930ffb9685be2271427231984a38365`  
		Last Modified: Tue, 04 Aug 2020 01:21:03 GMT  
		Size: 50.4 MB (50416768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373ec860ecd6bfcb3213600ca8a0ddfdc08e143796892174a3408250bb46938`  
		Last Modified: Tue, 04 Aug 2020 01:21:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
