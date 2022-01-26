## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:ae3165a67812a4712caaf6d69c141f52bb2194380c549b71c478778fefcb0a0b
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:76226b581fb810b2d0620dbb4dad4b2295ce8ea49654b6c4a26c6200cb84f983
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3d4a95fc216f03ec7e2fe6f76be3d47567be8c866d683df117925b5fe0bab9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:33 GMT
ADD file:25a11783eaacfe66a70e9ec1f1aede8d3e7c1bc11a1af8b60bb43df5fa9734c6 in / 
# Wed, 26 Jan 2022 01:41:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:38 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c4736e7b14d9d26c8aa7fbc4b58f0e0d71e9700b7c8a80b9c2273e5c68d8524c`  
		Last Modified: Wed, 26 Jan 2022 01:48:32 GMT  
		Size: 50.4 MB (50437090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19585f964c8c557028c50d3bec586e4443780f11695f6e5485c92d0295f07aaa`  
		Last Modified: Wed, 26 Jan 2022 01:48:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:c2b1e5491f75aec2d09aed68c29808e882c0497c751c93bdf915d4964fd774a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b31d3b012b2cc6e050f4a63a72c14ad8855159450014bd1f80498e6cc09de52d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:22 GMT
ADD file:27a5cbb0ac569dba6256d913250adf5a631c44824dd3d57983099e6ec062784b in / 
# Wed, 26 Jan 2022 01:44:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:44:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ff59ed9d062a65563328fe2ceba75a22a175f3ddcbb473638bfd679cd1d725c3`  
		Last Modified: Wed, 26 Jan 2022 02:01:16 GMT  
		Size: 48.2 MB (48154325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd894d5ff8c0999d2d70aa9f33f6b3dd40ce0ce74d0fb3d9341e54b307dbcc`  
		Last Modified: Wed, 26 Jan 2022 02:01:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:869672ec51a4c8dd1b9de12a9926a8f1596fb04d167256b490006f4ffe815386
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84a0bf2e354b2db41fa45ddb079268d8f761a4e43b64ef2e600b2bd8a324ca3b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:41 GMT
ADD file:f51e16e716ee595cfc9a3e1fbc339d66a69d0bcc433e5e3b0bedb37e8fbc4400 in / 
# Wed, 26 Jan 2022 01:44:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:44:55 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2895d853898a5728d44bdec73a8c6543f8357b5c3681a30a48eb7cd394f5de72`  
		Last Modified: Wed, 26 Jan 2022 02:01:38 GMT  
		Size: 45.9 MB (45918164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a85f8deb5b0dd3c30f5c0413f05ad290e006344157dc2c7bbc0454dc3d40f`  
		Last Modified: Wed, 26 Jan 2022 02:01:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d35c687f6f7b9fa8eec2518d3a78ae805cddea67a9f8681cf2e31dffc08b1a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49223238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e27090f3e930c16257f2f5ed6fbd190d443c249a893a660131a393604f2f8c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:28 GMT
ADD file:576981e529603901d7ee5e086e487d6575c865a9c09fbb5da35c8fa4466728e4 in / 
# Wed, 26 Jan 2022 01:43:29 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:43:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fa6ae475adfdeeb3da9317a8aaffcb5f6a820e8709674f2ade59c20002813833`  
		Last Modified: Wed, 26 Jan 2022 01:50:57 GMT  
		Size: 49.2 MB (49223012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1fb1f1dc6fdf80d15756978c38724c970246f2e5884e477abaa8e60443d86`  
		Last Modified: Wed, 26 Jan 2022 01:51:07 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:e8878aa32572e22bc919043f395cd69b0d863e2fd3e76558075b507ab7fa7925
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5d899965439792991d7ebf7593f8f618b88e13ae0338d1752a622c63c32b72`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:18 GMT
ADD file:8e16c275a5bf9af48659c27c4d9b108a60ad6e7f404940ca38cbf683c6b4a233 in / 
# Wed, 26 Jan 2022 01:41:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:352446a33f0e756b816a1035ad9a9590cd475b46e60ce6acf66c9b507a43a72a`  
		Last Modified: Wed, 26 Jan 2022 01:51:36 GMT  
		Size: 51.2 MB (51207733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42cb1394c3fea8065d5b6059ce055654a9c8eded69ba1346eb53435c17dd357`  
		Last Modified: Wed, 26 Jan 2022 01:51:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:aee5e44aac6811ed80b2b71f15762234a83bbc94f1f39ab979ccf7cddf4d0ce5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbd8b591af4a0a1ec9e02d709a0470e7ffe83216a59b6cc0b172ee50e45aa58`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:04 GMT
ADD file:fe4e5028990e0d8abed8c9e423d5d59a9c8a58d0d6d7448ad5b1336419cd6d88 in / 
# Wed, 26 Jan 2022 01:44:05 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:44:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:352d680dd7acd9f6bfbf59211b09b5924bb813983c9933948b447ec138055c67`  
		Last Modified: Wed, 26 Jan 2022 01:53:31 GMT  
		Size: 49.1 MB (49079608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454e3c21529e8ee31c8deac70ac8cc565ed4985c3e08f312a3763b76c987fb`  
		Last Modified: Wed, 26 Jan 2022 01:53:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:bba781e2df1f10fd132e6d7702bfaaa1acf9b78cbc7f5911a1ea8f323880444b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54183952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13cc597adb78d0bfad4fbe8dff34883aa45f4ecb1281f1209fcb7daddbf7d2ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:06 GMT
ADD file:c9381d3dcb4bc076fb454e46a38cd07899e23a6f83cdcce5507dc8a8f1c05777 in / 
# Wed, 26 Jan 2022 01:48:11 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:48:20 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d99af03ceb1ca82be6f163068accbde4edcfc63de9c23d8858e719fdedf0f8d0`  
		Last Modified: Wed, 26 Jan 2022 01:59:51 GMT  
		Size: 54.2 MB (54183725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67fdc7ca052b094d6e80e6d65310f7d90d203578de93bab9e2ced930dcdeee5`  
		Last Modified: Wed, 26 Jan 2022 02:00:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:f49d2db2de8e300899703575de09a245adf0aa261497c80f168315875e2898b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28a71e3fab6742a573f16f10df365d1e93f06d6cdec63c3978fd75ebacbc2cd0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:54 GMT
ADD file:e0f435dc5c30ba3c3df4729eabe861359825cbe25e08e647b81d2516541b9696 in / 
# Wed, 26 Jan 2022 01:41:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a711970d2777111d626132190a64b42c4351f6770098b94f389282354590c289`  
		Last Modified: Wed, 26 Jan 2022 01:47:46 GMT  
		Size: 49.0 MB (49005436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5b841cf82e314a34bd25561aafca8fdc3a0f4dd37f82e841b0e093f9800827`  
		Last Modified: Wed, 26 Jan 2022 01:47:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
