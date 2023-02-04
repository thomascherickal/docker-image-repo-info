## `debian:experimental`

```console
$ docker pull debian@sha256:08c66b5823e81b756d08f1824cff7088005e6b28ff6f8e40c664d5231e6c2193
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:cbfe25e26c94fb57e59d415e8e9439d53939ecb00c329a4350a166324ddd13b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49039542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e23a1495e7c98283b4b0632d55dc38973413d730a97f1aaef11081987996285`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:53:59 GMT
ADD file:4db06e4435a59adb5ea14744326f2ad3075253f03c1051ef344d8d0857d3c4e1 in / 
# Sat, 04 Feb 2023 06:54:00 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:54:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d44f7830c06e423736d4caefd5f51705ff318962d6f48cb5fc0944c817cb9481`  
		Last Modified: Sat, 04 Feb 2023 06:59:24 GMT  
		Size: 49.0 MB (49039321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a837643bc1ddc128c385e13af7e3b3c21a59e9ab94c0cdb18329191c631353e1`  
		Last Modified: Sat, 04 Feb 2023 06:59:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:2c7e662f54edaa34010a489063493b4f6e3e9cfadda6bf794c02cb819f1e0ba7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47996666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcdb27cdd25fa0ba2b9af2fde68f944899becd379c9cd69f2f56f61187881356`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:48:05 GMT
ADD file:534c27eb76f803f42e515e864256cd12d48c66bf4ca93d3518e9613bbc45868a in / 
# Sat, 04 Feb 2023 02:48:06 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:48:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:efe88ad76b423ab908ebbbc5d07cd3011845d565716e73634fcbd0028219ae6e`  
		Last Modified: Sat, 04 Feb 2023 02:54:13 GMT  
		Size: 48.0 MB (47996445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824990dafb7317e617f7cc2aef25fe33a06cdda045d2af1b10c0ae124cd0fa9b`  
		Last Modified: Sat, 04 Feb 2023 02:54:40 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:82e501fb5cad4034e9cd142c2e2abd6a62c3112477719415bba7216b3f81e8d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45796254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b0b94f4c13e140f70e053dd3594f013c9184cd01edfb2499270af7149c14b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:02:17 GMT
ADD file:ef9529d6926117547c33ef2a0acaffc1212917225dd628220c9fa1f14a10401e in / 
# Sat, 04 Feb 2023 10:02:18 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:02:35 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:161d71555cb85d23241501aad935f14698a4354a80cd92d9ea1a3fdc49040389`  
		Last Modified: Sat, 04 Feb 2023 10:10:18 GMT  
		Size: 45.8 MB (45796032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb6cd7a451210fc180874d78f537b4da574e6cbea9d4992d3460845d90d518d`  
		Last Modified: Sat, 04 Feb 2023 10:10:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:adacc15f51b519d3585b281dc2ec37b807459cd9e065656175b69d61b5f7f83c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49065170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a847f170af14df549841f9815c3bc5a12318b9818b5ed304191373f0f1479f3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:19:13 GMT
ADD file:c51461e4cb318d03fdd196bae2f39e61dac74f902570f666611f54fe032922fe in / 
# Sat, 04 Feb 2023 06:19:14 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:19:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6aacfe4abee2d2520cb1099f57e1d43b2327d99130ee34d3e1c82a7e5d5b2bc0`  
		Last Modified: Sat, 04 Feb 2023 06:24:24 GMT  
		Size: 49.1 MB (49064950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a7fee9cd83a923852908a839bbf98eccf1ddcf24bf42289e478c611fc342b`  
		Last Modified: Sat, 04 Feb 2023 06:24:44 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:d5ddc3cf69dd888bfc8296355631c385ea97e1fe8f5f0f7c649ab67ba96e3836
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50095660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ecc439e4702ec2e33cf8f84323d56d7dd3db722716a0d62f6347bd4f1f2fc`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:51:38 GMT
ADD file:1306edbdd860959589ffbbe608453d173c81f480150e6091ff435578006f954e in / 
# Sat, 04 Feb 2023 07:51:39 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:51:54 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0e0329292b3dc3889063744e823ba71c611870538fdc9a1d5e939477f74d1b1c`  
		Last Modified: Sat, 04 Feb 2023 07:58:41 GMT  
		Size: 50.1 MB (50095441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13271431736b6d1927ba8cb06995cc6c9d0b7a2e34de204ef07312312cde91d5`  
		Last Modified: Sat, 04 Feb 2023 07:59:06 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:69b2b5e6981a0bb9272dd934b52ba8d0a600d4d37455d43dacb8e7e44788ee46
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49035753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095980f18dff9eda993631ba00c290eb736b9480ca60842d75b11db163afda10`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:24:24 GMT
ADD file:e816cc77dae72e6032c66320f609eeab0d357e3b1a6e695ae4546789d23ef5dd in / 
# Sat, 04 Feb 2023 06:24:29 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:25:08 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:82ac751e058e233e111bfb5d70ba5e0db751acec0817f9b4be0d47b69fa92d20`  
		Last Modified: Sat, 04 Feb 2023 06:33:00 GMT  
		Size: 49.0 MB (49035528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415a31d229555051c1ca8cf36f6cf60d113a35c33e36ea4c4b3dd6727437e27c`  
		Last Modified: Sat, 04 Feb 2023 06:33:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:f324a3f782f22020066d9bf66ec25c85399a18534cc21665f35bddd8ed793616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53052714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e6a6f11ecc16fd4cea2b8d2b95d8e68bd57e17fd57093e24b66e38aec1d563`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:28:22 GMT
ADD file:e300d5648c12b23196bcc3174d563518e71434a9f9566050954322d78cc0af88 in / 
# Sat, 04 Feb 2023 12:28:25 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:28:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:180c4f124629058d3f7190528192a6aaee853ad98b15175204188594d436be07`  
		Last Modified: Sat, 04 Feb 2023 12:35:04 GMT  
		Size: 53.1 MB (53052491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c80038793a062e5161009a13dd2af96752be4b5aa5d57983595fa92c7fdf30`  
		Last Modified: Sat, 04 Feb 2023 12:35:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:673f31991acef53cb58cec67247598b2392949c76a5b4d74f0899a112b59b634
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47408318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7802975822b68f2f940c7a2cbdb77efbfc6932683a63da0f03933069298cdf76`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:07:49 GMT
ADD file:3c9acfbe477ef9b7cf73ae31792916ba05d27b89c732e71d0daaff74ddeb122f in / 
# Sat, 04 Feb 2023 04:07:52 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:08:10 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:62f7571fa4c40757b40308fc2a271dea2516970f00b23711f52075edd81b8b5e`  
		Last Modified: Sat, 04 Feb 2023 04:11:55 GMT  
		Size: 47.4 MB (47408096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fe70fdcbd94cc004489e579a756862719cd7f0250c9f655ee35d6322365c68`  
		Last Modified: Sat, 04 Feb 2023 04:12:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
