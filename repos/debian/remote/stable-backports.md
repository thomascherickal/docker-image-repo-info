## `debian:stable-backports`

```console
$ docker pull debian@sha256:f311c4439a27483637dd082b372b25baa21a11aaef2a8a89431e17f353a4bb8f
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
$ docker pull debian@sha256:c0ad7455d9769b3d6c9dde355ed857c64e56b2c63039c103ec0a906b926defbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55025493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503379b9041b14cc778eef5d1f5a303f54eca1c3bd95c1e68d3983507303cc8a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:53:06 GMT
ADD file:c57b74606b7634eecc0a835f02befbb3339986ee5bba24a3eb5d25963026f94d in / 
# Sat, 04 Feb 2023 06:53:06 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:53:11 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:768d70ecc534d6ae8552f275eedc0e2855dfcc566063472000e02a6c8457f664`  
		Last Modified: Sat, 04 Feb 2023 06:58:18 GMT  
		Size: 55.0 MB (55025267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe04631536af1147c19810fbffcaf484be2dad86697e08be327350dc664d50ec`  
		Last Modified: Sat, 04 Feb 2023 06:58:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:3792b29da5ab77f175fa8a3ccd5a162a065901793d1dd40ff7dc9260cc5f0fa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52530207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7f97f6a4c96ed9737015b769f8ceb94976c9fca49dbd3216268b72cada1c8c2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:47:14 GMT
ADD file:32b3bc749ff98f3b05cc3ebd80cafce40a3a1aaaa47a1c49068e9e04de08e837 in / 
# Sat, 04 Feb 2023 02:47:15 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:47:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5013c56a2968a9fd79b8dfc151bc629446aaba8a3aa785f8f1fffb7dcce1c4de`  
		Last Modified: Sat, 04 Feb 2023 02:52:48 GMT  
		Size: 52.5 MB (52529985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacc77b7f737071d4dc0bb6c708a30790b87a2226d05273b408bba6d4b34fb26`  
		Last Modified: Sat, 04 Feb 2023 02:52:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7edce6fa42ec2bc91eece482a9e1fed1826c2e236b91a5d256ae60663b5aef66
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50191045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90af1acbe2fd327310863b8a03fd942306a4aa9fd3363d98a9d62f2a703d658f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:01:15 GMT
ADD file:b37370e6ec4c1b0ffe5895847baf585c461727497dfd4fc12cf310f0095ef5c8 in / 
# Sat, 04 Feb 2023 10:01:16 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:22 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9ea613f26910ab5d440f99f6124b40a16dde8c13bb53b78e59b3f19ec79e7eeb`  
		Last Modified: Sat, 04 Feb 2023 10:08:55 GMT  
		Size: 50.2 MB (50190819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ba5277f091c8290dfdcd1c19ac9ef89adc3a16cfdcc3a8ee3073e4d54cde`  
		Last Modified: Sat, 04 Feb 2023 10:09:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e9ff77776c0386e95602011522556545132d90e2a6c081947a1761c91c3d99c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53682144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a3e3a7923e574aab2efba70da7ea43063be42477fd09cc84a6362224470743`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:35 GMT
ADD file:ba72175d63a0b7690203b541187731f85bbf2ef01cac30e1556b65e1e12366cf in / 
# Sat, 04 Feb 2023 06:18:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:18:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cbffa2d5fc1510685b83ba4452ac96d8dca75a897fb35533ae3c113c1999b34b`  
		Last Modified: Sat, 04 Feb 2023 06:23:20 GMT  
		Size: 53.7 MB (53681922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29f674b85045bda18420f86fac479116e0c72cc175767b67e81695f0646bfac`  
		Last Modified: Sat, 04 Feb 2023 06:23:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:6d874e161365e95bdcdf7b9a354f2c83e1ed47e8d6d396854741d75092cf61a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56005642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc5556024834208fa385eec702ada17a7e92330552565295935d4ea3b81b6a9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:50:47 GMT
ADD file:15fb6cf98045a4baa5e7cfc2167794b2c4c4b7bc9afff397ba6afebee28f76ce in / 
# Sat, 04 Feb 2023 07:50:47 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:50:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8b414227f9956ffeae64bbe7755bed1aacb9736e3ed8635931b9746f7b4cef3`  
		Last Modified: Sat, 04 Feb 2023 07:57:24 GMT  
		Size: 56.0 MB (56005416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ba1b2d1fc62f72dd39853aee5cb385c5a1e1bf3a0fafdcd18defd11b20e2b4`  
		Last Modified: Sat, 04 Feb 2023 07:57:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:af8741d76175e8b7ecf9284e8bc846c546102643a581f0891e86afce62c944e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53245386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01aaac098c07afb3091aa874fb06deeab58ab9337bdcb8d4525430248f60c232`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:21:54 GMT
ADD file:1b4dce0a3e850ad9499872dc1e984162ea586eafd30949e744d858e4ba56c3a5 in / 
# Sat, 04 Feb 2023 06:22:00 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:22:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1623d49b4434d22266ca96694f381462df382a6ca57df2bb4311e5cad0fe2919`  
		Last Modified: Sat, 04 Feb 2023 06:30:22 GMT  
		Size: 53.2 MB (53245162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0978d2824c5d0901f68db8297ed525594c585be4562e6dfdefda146a72743bae`  
		Last Modified: Sat, 04 Feb 2023 06:30:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:285105f12c585cd7886b91ae9b7f5712adb32a087e3b4ce0681e694aa3052328
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58897313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dafc1a0745f0f8facc3705dbd4ff388e401112bf2edb543f4d268a037899bdb9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:26:54 GMT
ADD file:f665bfb52f256def6436e276340615e82eab111f3c351ffeb4b10ea132b7c3a5 in / 
# Sat, 04 Feb 2023 12:26:57 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:27:03 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:33217245e40cb64e33aa1834c4fcaf0a1cc88d61b66a02de23e2368a0ffb439a`  
		Last Modified: Sat, 04 Feb 2023 12:33:24 GMT  
		Size: 58.9 MB (58897087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f664ca3e65a67e79b693a61523432ec183a6ce2a70d090c9024f71eb36d36c`  
		Last Modified: Sat, 04 Feb 2023 12:33:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:cd78ffd908964e365fabe9dc391c4dfb931980d4fb6f04a2e60cdf9ec7e2060a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53258616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b916594d446c7d2205f7f340e74d003dcd94bab72ccb81351e113d84aaf715e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:49 GMT
ADD file:c7b8ca5982a5cee5ae96568470d7225fa0c4a57ca26e18f23f31e9a73ed9e3b3 in / 
# Sat, 04 Feb 2023 04:06:53 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:07:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:250656082a622a9c5f2efeb2755f7eb2c9b21d07e998b8da068cc0fd898c6639`  
		Last Modified: Sat, 04 Feb 2023 04:11:04 GMT  
		Size: 53.3 MB (53258393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda9627baf5fb06d499529b1f1fdd0c9da7ffe4d9181bba52bf9207bb4d4fbc`  
		Last Modified: Sat, 04 Feb 2023 04:11:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
