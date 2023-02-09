## `debian:experimental`

```console
$ docker pull debian@sha256:60ea1184081e897a3d6a3cb0405b5107f7f761c1def94a99ba18ddaaed7a60d9
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
$ docker pull debian@sha256:bdee4a377688191cd604c903e555fbb8ebc924a3ebea260b660f94838cb96b55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49234730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7794fc647d06c81e5d190e5030c3ff622f3e0d18ff9f6db2ccee38e15b8b5a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:22:51 GMT
ADD file:56a6a49aa813afe1055b9163c91129d3c10461355637680ecf096ef775592f67 in / 
# Thu, 09 Feb 2023 03:22:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:23:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6db77e56f2a0b0aa1e9a5de31a4cd69a282b6cf2481c7a84242e1bcb7d6d666b`  
		Last Modified: Thu, 09 Feb 2023 03:28:22 GMT  
		Size: 49.2 MB (49234511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af90bfc3289c54325ebbd744cbf63c2637a3ffa4eee1f12e4970fc911789d3c`  
		Last Modified: Thu, 09 Feb 2023 03:28:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:9215c9972f2e7b1b1342dd6a2caebee2a65d69a8f5a7eb4f3c6cc1935451f69a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1ecfe735c526cf2981370208c40b909a893104a622a5256631533c5627ff06b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:02:02 GMT
ADD file:7bfd7547d6a26fb6099d06f79d79da7b24a066fa5653edeb1d00ef2abd960ab6 in / 
# Thu, 09 Feb 2023 02:02:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:02:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b06d379532bc5b3ca4ac0683130115e7f1789aec62e79fcfa5d1d3d3c2da1dc1`  
		Last Modified: Thu, 09 Feb 2023 02:08:08 GMT  
		Size: 48.2 MB (48168669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfa7a9197fea7f947656cdc44a2acd386930874401d8e1ad3ebc196ea9967e`  
		Last Modified: Thu, 09 Feb 2023 02:08:36 GMT  
		Size: 220.0 B  
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
$ docker pull debian@sha256:7e67c95d17c757d8f4fb80a15e101cd0e2b0021e43304deb58d8cd1fce11486b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49272477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4e3f0f90b33222d9a87592782b60cd60f2755637b78c85560c2b1f46a46bce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 04:00:22 GMT
ADD file:c62def8c6e575fed884255a2f250d84af4b3f2a43fe7139ec4c820c78b3dd973 in / 
# Thu, 09 Feb 2023 04:00:23 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:00:34 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6b1797164b31ab32dbaff37ec5348050445a28bcad8538f0e9cbe02f528db6ac`  
		Last Modified: Thu, 09 Feb 2023 04:05:33 GMT  
		Size: 49.3 MB (49272258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25381c18702e5923d1ce3d2960f7d98b50a506553db95d46c91588b0cd74eae`  
		Last Modified: Thu, 09 Feb 2023 04:05:54 GMT  
		Size: 219.0 B  
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
$ docker pull debian@sha256:62ba174e8e2f575c50ab2c45d01e7a396d01dd446a103001e3f120e4dfff277c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49094483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa283049093ac699beae3c7c914a1b433fb6800399379f622365d0fff35cf1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:49:42 GMT
ADD file:d66b7879da96c52ddc9d32b677f67f6f36cd8d58f06b6fce3c4c8720b80418da in / 
# Thu, 09 Feb 2023 02:49:47 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:50:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ed54f16bbfa6ae7109ae525fcac7fae8fd6ff2d232ff21349cb18e393290aca2`  
		Last Modified: Thu, 09 Feb 2023 02:58:13 GMT  
		Size: 49.1 MB (49094261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4bf8b3630a4c4950dd6d9854e5179d4d9e2572d1aea943c66b630153abc0f4`  
		Last Modified: Thu, 09 Feb 2023 02:58:51 GMT  
		Size: 222.0 B  
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
$ docker pull debian@sha256:8dd2352eb6e9e45194168e322f485918dcf0c9213c94e4b23b5c69cce1ba7fd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47605717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9548917f655bf29614914fdff2fbbf2eb7723b75a68bb30fb8b5a83ceb1168fb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:24 GMT
ADD file:a9c6323e382aa32d6b596f1c61f55f06e55357b5ad0ec8c4027bd649a9183d73 in / 
# Thu, 09 Feb 2023 02:43:26 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:43:44 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4f6aa1d95f253f3246d1d60386fae207367e7878c935165536d9a95adf2070f1`  
		Last Modified: Thu, 09 Feb 2023 02:47:43 GMT  
		Size: 47.6 MB (47605497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0889a005301a1bf2439763c04be432e801c658228a3ad297c33d4a4081b47d`  
		Last Modified: Thu, 09 Feb 2023 02:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
