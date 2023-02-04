## `debian:rc-buggy`

```console
$ docker pull debian@sha256:dbd010c14b55ee01ae5aaa62100963519dee1feaaad9c32baf2d41258d14350d
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:96186c9a90ba837abbcb7a69cf883c610eea307392b21e754dc25a69b41e29f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49040975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f64f7b5e4b2a62c039f5705d804ae60f3f62b6ca59af50cacb9458f15584113b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:41 GMT
ADD file:3bae49887734af64f153e9e3668684efface6dd04ba31139b3d6b3aeb7589128 in / 
# Wed, 11 Jan 2023 02:35:41 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:37:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a0e522725e09a558b80e5d58e7b360150ad3fe901915db5358002bba7e461b9c`  
		Last Modified: Wed, 11 Jan 2023 02:40:40 GMT  
		Size: 49.0 MB (49040747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0236c185ae78c3240c4787f67aa6df295e8c95cab2fead8c17840a9a1788318e`  
		Last Modified: Wed, 11 Jan 2023 02:42:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:e45350d3cddce0bcfef4d1d26147347c1824041091062ed32935d5f69ca4c21b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47996664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26208c18a4d621dc557c8931aae53d752f188c5e73bcc7ffd292e81b1f466c51`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:53 GMT
ADD file:12eddccc39577b9f5e10835b6a2c5edd0b1a49ad547e20f5e2640f434b8d2a42 in / 
# Sat, 04 Feb 2023 02:46:54 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:48:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9756a18a5cc1d83f45eef500c448fdd88a17d9e9c99f86f02056851b6b5ac543`  
		Last Modified: Sat, 04 Feb 2023 02:52:12 GMT  
		Size: 48.0 MB (47996437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30f6faefc38142cec8b4216b6effdbcea0fb0295bd01729381354a299427b7d`  
		Last Modified: Sat, 04 Feb 2023 02:54:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:8069f3a4c65d5b90737e35a799992a3d841d743a904018ddd77ca50f50ce0095
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45836857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:051b55be8f1456cb7f21e1d96f7ad9f5f14ba7a0a79214fe6ad781e29b0cb051`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:01:58 GMT
ADD file:45e9dcffe5e042927af8c1ae4e6393b33fda2a9ad194140450689e4f039e0e20 in / 
# Wed, 11 Jan 2023 04:02:00 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:04:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b5f9150f24704ac05df76d4317fa7947141130d434993eb229642f2806e580c9`  
		Last Modified: Wed, 11 Jan 2023 04:09:46 GMT  
		Size: 45.8 MB (45836631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f5755810e3160f6d6a34dfce6f696f3fd80e3d9aad1e73a14ea2de79230bed`  
		Last Modified: Wed, 11 Jan 2023 04:12:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2032e97b3f0a8a25e0be5795ab0775aa428a61549873361cdb23ea7b12964f67
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49084778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d6d5d998d3b07e7a06e37e78cbe7cc23cf2361875ca92d531cf047a4540299`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:58:15 GMT
ADD file:b780242785904e4fb27dec85c00f7e10bcc0dbb0d7006b133d9038c4328c7d83 in / 
# Wed, 11 Jan 2023 02:58:16 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:59:13 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:57ec0bfa7127b6c459b1b1f099459b850b4fa150e388b2c3ba10105c4a746caf`  
		Last Modified: Wed, 11 Jan 2023 03:02:47 GMT  
		Size: 49.1 MB (49084551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8f54d6fffd7f9efbc59f7b8ca852f84b118247c51ead2cb2559956fafbf5bd`  
		Last Modified: Wed, 11 Jan 2023 03:04:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:0c20287972a513f52d007bfb24e16cb39699bf96364fa9f396e546b533e993f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50082715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb9372979b08e590d69938c93fda2bf8d2373af14b00987a7243b64b70094b3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:17:15 GMT
ADD file:70daac43e15ae08f49ca2f191e46f20fb9df90f6fa25b199b61103e75ae43d16 in / 
# Wed, 11 Jan 2023 03:17:16 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:19edd03a92bb4010fb5a10c8cc739c02db9ae484e4e25247ce4b7e0977cf1e9d`  
		Last Modified: Wed, 11 Jan 2023 03:23:48 GMT  
		Size: 50.1 MB (50082487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d33f1d0574f79005ef7150607ee520e2dce730cf61e94488503b1774cdca13e`  
		Last Modified: Wed, 11 Jan 2023 03:26:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:068a18c515ff172ff1e06cf6a2f700a2911a49001173e9b302b76e9cb87bb424
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49043292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc519613ab9b933e289e63199e53a1d515335cae8f41b97e8882a052b9753395`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:35:05 GMT
ADD file:a772415cec37230670450044a3962179f53657814c9c0e8bc6ef502ab4fff614 in / 
# Wed, 11 Jan 2023 16:35:12 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 16:40:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d8fe537e863349284188081cc926e1cbc3d1d09a758c86969580374a79f6a9a0`  
		Last Modified: Wed, 11 Jan 2023 16:44:00 GMT  
		Size: 49.0 MB (49043063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cc016b6692f5b5404af2b637d6e8bc29ecf8cc527b171c7f064832cf5793f9`  
		Last Modified: Wed, 11 Jan 2023 16:48:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:b81a2ae7544164802553d5a7256de1479db74742d7e006386763eeddb5dec982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53077937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957689fa1f5fe125fe98ad5bf35f9abb993bbc302b3a3b2f9a79538c1f96473c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:50 GMT
ADD file:a8a466b916dd8b82163da9263cfb32eb757c2a0eb173228a5ac8ef05bdc55653 in / 
# Wed, 11 Jan 2023 03:49:53 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:52:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:35c8c29d2bf600cd3a311b3649ac4076a0670c35cc296f1f28d2622bb6dd54d4`  
		Last Modified: Wed, 11 Jan 2023 03:56:03 GMT  
		Size: 53.1 MB (53077709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc23022fadd181f60df94ddd1f8d6aa4380dec996f59a2ee2c7c99c00094e65f`  
		Last Modified: Wed, 11 Jan 2023 03:59:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:396baea5c74391a26569e622af7cba15323dcb930e7b8ade037a46a1942be3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47408312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b53c57506061236fac904d37cb0aec6ab70000d8ef43f54e0d5f8f8c6386bd2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:27 GMT
ADD file:93877457106ba25112f38787099a736e27572cac3ea286b62bb0cea369e7334a in / 
# Sat, 04 Feb 2023 04:06:29 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:08:15 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0eed18e15556323b9c6a0c2e3bb53a6d5526fb5398a405780091330bc1da9c2c`  
		Last Modified: Sat, 04 Feb 2023 04:10:42 GMT  
		Size: 47.4 MB (47408087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca5006adf5d328fb9c12a4e31e5fc0d928ec04887b032e597638ad67010a9c6`  
		Last Modified: Sat, 04 Feb 2023 04:12:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
