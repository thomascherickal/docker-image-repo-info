## `debian:testing-backports`

```console
$ docker pull debian@sha256:6c1ec928c31593e59e09bd34337a169a26f30853faf73949dc6d01f91d8bd9fa
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
$ docker pull debian@sha256:d754563fd3fff3cc6871651e0934aa9effb5e4779bd31ab75c2d1260b3b53bac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51782503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4dcbca9d16489ba40b4ab6dc3ead2c0f0b6b9424333459611550127557f276`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:55:32 GMT
ADD file:c3d9b07c84acc04860039e8339afb29fe3d85823c6d0d51433d882c41c3a86f6 in / 
# Wed, 22 Jul 2020 00:55:35 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:55:44 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c8eaa6fc367fa7db4f78829d37b2688ff4745ddf82960397778a0156fb0fbf10`  
		Last Modified: Wed, 22 Jul 2020 01:03:53 GMT  
		Size: 51.8 MB (51782279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b35d83a65f9d4f6170b998fd56748ceec80a007ac7f4ea68d6dcb1a1724a9c`  
		Last Modified: Wed, 22 Jul 2020 01:04:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:54ce1ec25ae452da0779513ea5f147bca491a5997eb535a2ab6d0d23aa06b206
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49462012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd8877bd8ef0f4082a3fc82f0324e74edc914ea6135b9876a407f5f2236e6c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:34:19 GMT
ADD file:edb4e3dc41f3c894cfc1bf1568489659e5237d6d150ec796470ed7cf5d7297ed in / 
# Wed, 22 Jul 2020 01:34:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:34:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8aea71a18c347980dd222396f60781d6b3bf3702b6eee6ced8303ebaf53b205`  
		Last Modified: Wed, 22 Jul 2020 01:44:50 GMT  
		Size: 49.5 MB (49461788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a345e231caccb7f6c3a9a83e79e2dfde07d560c9bac76281819e49eb1584cc4`  
		Last Modified: Wed, 22 Jul 2020 01:44:56 GMT  
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
$ docker pull debian@sha256:8b1f8689753fff69bd3cd010315536087090572ebab0654654038a169448e21d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55225246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e829f99e3aeccf5645b6b6d46a8b593e5d56804f0e829340a0de140065ab7436`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:12:54 GMT
ADD file:82cf3ba5cbfb4f26c6c9cd1df8899b379fa0af4c99c0ed9359e5bae1250270dc in / 
# Wed, 22 Jul 2020 02:12:55 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:13:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7bcc3c67bd550d63ce5e94e3b620ca418058cef47f331a804894816e4b9ab305`  
		Last Modified: Wed, 22 Jul 2020 02:19:46 GMT  
		Size: 55.2 MB (55225025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81670c71815aeae5c8f4d952ed6b1d2f37212d2b3723235618c35f970824b07`  
		Last Modified: Wed, 22 Jul 2020 02:19:50 GMT  
		Size: 221.0 B  
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
$ docker pull debian@sha256:9f8326ac44f3b4b7752b72c30b7dcebab397251d07e6a5840131001db3c2f076
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55148225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c373533d52677fd080889073e02ac7e6b68c290b55db8a9f30b0dfa0cd18dd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:56 GMT
ADD file:72fcd44a3cd61718c43b8fd4856b710ec66a4c58ddc118863a85dfa8016f5c8c in / 
# Tue, 09 Jun 2020 01:26:00 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:26:14 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9ff154698924dfd0c8d74f3ad2e91d17dd68ef0c5b54849d3f7241b9df7886b5`  
		Last Modified: Tue, 09 Jun 2020 01:38:19 GMT  
		Size: 55.1 MB (55148002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ea13e8fbe40b418e3c7399599ea434d641e57442e16c2a12e599cbce90b7f`  
		Last Modified: Tue, 09 Jun 2020 01:38:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:30c5ed692e66441cfb52344ff032434266ce988de36e0fa43ffcb79e52cdd63f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52406464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edb6b262f656e4caed9466c908735c569b4b021c298de5abca3c14a5ee189ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:50 GMT
ADD file:700924a8b1e626458101c2eeb1df45c86a8b29d13fae72a662f4be9b2767bff4 in / 
# Wed, 22 Jul 2020 00:43:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:43:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:020c9a31aa02f6680318d96f88af1fffbb55b96bb0bcf3cff6dff707e01af3bb`  
		Last Modified: Wed, 22 Jul 2020 00:47:00 GMT  
		Size: 52.4 MB (52406244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7217dea3badf3f5e5f9c80b5084197449bffad95c79708e7961391666c137399`  
		Last Modified: Wed, 22 Jul 2020 00:47:11 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
