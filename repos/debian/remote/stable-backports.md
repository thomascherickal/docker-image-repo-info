## `debian:stable-backports`

```console
$ docker pull debian@sha256:188c31b821e1bbfe2ae8259b86b50b057271e817a20ae43d84b4356ba3b10635
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
$ docker pull debian@sha256:6a834e02a1aa895e197df3bf087783a47d90b003244e034cc78629f67e66e7bc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52552058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233ed63fb97e65a267bc560946852c1207e1a13e1ddca74f258fbf805db56f55`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:01:09 GMT
ADD file:aadb8a3f3bb4d76da194ca1430801792db5486b4c6bb085361b661730817bdca in / 
# Thu, 09 Feb 2023 02:01:09 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:01:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5104b3c59ba30358f01df3920ae0670fa072d624e723c64d7d3110f14ec2258b`  
		Last Modified: Thu, 09 Feb 2023 02:06:43 GMT  
		Size: 52.6 MB (52551835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d99d99ccf74aed9d1b3c11b7b28d89f4a9229bb1172ccf1380f84e91a78476`  
		Last Modified: Thu, 09 Feb 2023 02:06:55 GMT  
		Size: 223.0 B  
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
$ docker pull debian@sha256:3c5d1cedec5848f4f782946f03e01e5dafde1934455076a1e3418343fd460a74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53267017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e48b897957d72e97c84ca7719e7526a3f8ad742d96cedf087230f9bec42fd2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:47:08 GMT
ADD file:39a6afae8c3eacac911f0dfb3bea652228471909c6f8ea7094123715128d81c3 in / 
# Thu, 09 Feb 2023 02:47:13 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:47:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b2ab1fb26b812ee53551d009c13311e13292f3f7e96ffa8b0b8641da27632c07`  
		Last Modified: Thu, 09 Feb 2023 02:55:42 GMT  
		Size: 53.3 MB (53266792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3362f40ceb2d402f3533305481d5c8ae9bc82245ec719db06d058ff895c8a7`  
		Last Modified: Thu, 09 Feb 2023 02:55:51 GMT  
		Size: 225.0 B  
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
$ docker pull debian@sha256:049e68bf86ae5120bade64ea065950d3c3fb41260c346c95eccc3df99c37f743
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c137493c6494a19ef7b0609c471a1f6f5761c0c75df49fb7316edbc212b2c79`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:42:21 GMT
ADD file:4057138fad7c5aecd192988c593dd7b997c8ade6e44621307639f5669b64cf3f in / 
# Thu, 09 Feb 2023 02:42:23 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:42:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c36299b95efe6adafeeca8401d4fe17de21c7947488846e43393351dd4e3c451`  
		Last Modified: Thu, 09 Feb 2023 02:46:46 GMT  
		Size: 53.3 MB (53278906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103511dc331478ea76f6238a7d8df7b3a487f3db791930cf0234df21a03bfbe3`  
		Last Modified: Thu, 09 Feb 2023 02:46:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
