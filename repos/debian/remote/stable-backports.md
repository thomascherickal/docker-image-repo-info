## `debian:stable-backports`

```console
$ docker pull debian@sha256:b34cc0e8cb8883c8387282e2002683a1237ac12214a702bc49a922c1b7b7e8b7
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:36332bb99256ec6435b20a917ba1492e1027a0b3879160e638a7bf4cbf2bc6e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50390548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c3c786009f99b16a52b82e7d6f8f653c4d34339b15729f356ba34c34019cb8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:11 GMT
ADD file:e452c7756111c96e712dc2b42a59e87ebc8dfebeeff03939c62773d73c7ff71e in / 
# Wed, 22 Jul 2020 02:06:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:06:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3c77d565f42d8558a327c2abef361d045d9394c2bfacc64d8397fc382ff59f16`  
		Last Modified: Wed, 22 Jul 2020 02:11:49 GMT  
		Size: 50.4 MB (50390327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422792c8b6247385dfc23bc92c06e21ea0af03658b93b64489d074d84875bcf`  
		Last Modified: Wed, 22 Jul 2020 02:11:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:775f9452bd10e4809724cf3c7d10e6adc8ed9b1e13acd74dd06245be73db8670
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48107485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45092caf2edd1ffe4a511f9cea5023c6ddc0f08bb5591ed2335d43b0a8173fc7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:54:05 GMT
ADD file:28a6e5866f79bc0c602de5678fcdf59f1ac69879f95fbf47844848005c949522 in / 
# Wed, 22 Jul 2020 00:54:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:54:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5a8f255ec78cd58b9b23e8db246c7eb7e5324de7356a33931deeaebb9b18d529`  
		Last Modified: Wed, 22 Jul 2020 01:02:23 GMT  
		Size: 48.1 MB (48107261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7aa5e9c4b42f822fe2e9d054e7b589bdc7922d2000a98badc761828140ce8`  
		Last Modified: Wed, 22 Jul 2020 01:02:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:37ed3cf8c3ed9b6a8e7c69995df6e4c8ae81a5f9145e0163c8e5eed33e0b90ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45868943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac3053ec716e282abffa942353431acf4df22703783a029e51b9f5ad0eea0e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:29:32 GMT
ADD file:647ccee81a788e86f72aeb0d2f214bc26e5bba5b22f4c0c874f7de87718a2d26 in / 
# Wed, 22 Jul 2020 01:29:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:30:30 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aaa1a29525846b3248a44917d243b57b479e5d1c51d1c3712fb8f34c63ef91ec`  
		Last Modified: Wed, 22 Jul 2020 01:43:26 GMT  
		Size: 45.9 MB (45868720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed379cd860160620eb19bba859697f710c30640f4406324df39d0a7414c0492`  
		Last Modified: Wed, 22 Jul 2020 01:43:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:738cb4748a37120b78a14ffd564303bc58dec34700f6c8aaf19b6e72e05c3223
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49168674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6ca7bca92e54bbc886781650b4ff83aba4723988d159c29c48e5dbd8558e21`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:55 GMT
ADD file:e5c5f409a34580144c4a48398f533579576017b1e64f634dd1b7a9053684ad82 in / 
# Wed, 22 Jul 2020 00:42:57 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:43:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c108223a01e90fe2b99a3b49ab09c0bfcbc8861c8dd20fbe195b6d02666ca902`  
		Last Modified: Wed, 22 Jul 2020 00:49:14 GMT  
		Size: 49.2 MB (49168450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7893a9840050664b7374e1f43cddf4c80d2c9afa22d0df6fdfa16d616b90633`  
		Last Modified: Wed, 22 Jul 2020 00:49:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:ca9203e89f63544014a560c25f9f7e32eeb93d6f31a7ff6e94a20066604130c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51157418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b61457174ee81032d56486c13ca9a9581cb349d782542d9df30973c7dcd945`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:11:43 GMT
ADD file:eb1dc993629e59377ce775a2e4c53556ffb33fc211775c83443ece7ec18af085 in / 
# Wed, 22 Jul 2020 02:11:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:11:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c4515c49fb151354e7b46e6546c98d48b55c0cfdc954c7bec6562964fdcff04e`  
		Last Modified: Wed, 22 Jul 2020 02:18:43 GMT  
		Size: 51.2 MB (51157197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9e570ab67847997f9bf28aa2112d4be492b511a53d2d031dab66179def71fd`  
		Last Modified: Wed, 22 Jul 2020 02:18:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ba0d2344d84dcb94b60a5d8df21a7ffa8563a83935796633d060658d683af1c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49019684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be88d49fb825f1ea2b5c167a2605475f37ebecbeff39b2aecc3e413c6864b5e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:11:13 GMT
ADD file:6fecb51a7bb66cec9ed1357b9c0c8ae124ebc1cf311f36d68c758ea63d90c66b in / 
# Wed, 22 Jul 2020 01:11:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:11:20 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a42c4a92bfd9c0ac971bf10c5c0219bb408aeda37a695df459d6c5a16ec322a7`  
		Last Modified: Wed, 22 Jul 2020 01:18:47 GMT  
		Size: 49.0 MB (49019458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec375a2ac26c9d4b498d7df01b9718ee76d84c137253de698e97e3f8abd4bef`  
		Last Modified: Wed, 22 Jul 2020 01:18:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:ba699c900a8eec4f68317894be7ccde05391460b2344a2dea2e682cfd90014c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54143571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2819f23d53f4eb4cf797631a9d24f129490cfe848c9af96a5a707b9e4ac1c40d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:24:24 GMT
ADD file:abc456eb96e450d5cb22ae2f7c4460611b08f85c9330a356471b0ea8f044aa79 in / 
# Tue, 09 Jun 2020 01:24:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:24:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a2fcd8ce49cba897cab451e1620072aa9f85506fdb0a56326dc4b6c919560be7`  
		Last Modified: Tue, 09 Jun 2020 01:35:16 GMT  
		Size: 54.1 MB (54143347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831e748262469682dddb416c856d75dd50d7cba5dfeb2d1770d9872134f86387`  
		Last Modified: Tue, 09 Jun 2020 01:35:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:f25dadb7e7205d402c286e079554b059b88d24dd9efaaac7758a3e90f5cec55c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b407b0e2c7e23ac020861dcbdfcbd93f900440770fc06d9e29715690d073e7a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:19 GMT
ADD file:028a6d08144477fa3d0c4a0293820f8c254517cbc736c9721385dd9adff946ee in / 
# Wed, 22 Jul 2020 00:43:22 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:43:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af9a1672d8821b6ad785a536b82faf8414b8e1a2d75d7d70fa6477e18c5b65e9`  
		Last Modified: Wed, 22 Jul 2020 00:46:27 GMT  
		Size: 49.0 MB (48966443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64710e775883f70053af38c3260e9ce085fc7fc0ac1b3de11565f1bbef46dfd`  
		Last Modified: Wed, 22 Jul 2020 00:46:42 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
