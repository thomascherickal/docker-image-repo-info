## `debian:rc-buggy`

```console
$ docker pull debian@sha256:ee58ec675f6ed2588edde6c8ff0b4e39719b09509f575741340abcaee2b55e40
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:34f6fe15e57ee65e8db1d275bdf75c54eef5e0f77b2f2ffe82fd6ac3292f5129
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52340558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe30f3c7b3c35195617977c1b1937fb79abf1ef122d621f665c74bc2711edf6d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:05:41 GMT
ADD file:388f29164844b8493d30bf1feffd1158559ab161886928f977604c10f983a704 in / 
# Wed, 22 Jul 2020 02:05:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:08:33 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:babaea2ea26ef0e3e4a90ecc928d26bf25d699e1dcba843f16b8a2f0a153b3d7`  
		Last Modified: Wed, 22 Jul 2020 02:11:28 GMT  
		Size: 52.3 MB (52340330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b98bca4adf1b0fb367e73524f31703023b69573bb6b5e88c57d5005bac9b10`  
		Last Modified: Wed, 22 Jul 2020 02:13:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:a567a9bc7912ea8784a39b4ab958ebf7217894a27078f4af27c8400979ad297a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50310348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ae4cc8d729662f9033867d30f34e9f1802d8c63d15d7ff09a5a16d7651ec04`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:19:33 GMT
ADD file:966adedb56b8840e71e14255f1e10c11506897b861f32a0c8c84c32338edea04 in / 
# Tue, 04 Aug 2020 03:19:44 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:31:41 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:70fc41871a830209ccc29805b1bb08b4058beb41df471ae13bc23555229a9623`  
		Last Modified: Tue, 04 Aug 2020 03:37:01 GMT  
		Size: 50.3 MB (50310118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7862b215bc7c69fe27acf21e77f38d1f7fff70594c79c316d51ed22f8ade01`  
		Last Modified: Tue, 04 Aug 2020 03:40:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:7273a34e018590e00400a2e4b39cc7017de3dbe4659f00deffdb182d5b6bd1bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48083139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80158e6d4047d8b860600c647f8fb8ed33abf413f4c9bbcbaeda18720d4e9631`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:59:26 GMT
ADD file:5793438e4679788bcbcd7ff2adcfe8f0c31bb4ceca63088d7c74a20cac1e87b8 in / 
# Tue, 04 Aug 2020 04:59:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:03:25 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7ebc2f87ea858cf67ec5ea8f8fcd77fa8fefcd9b35b71d1b3efa355f8289ce59`  
		Last Modified: Tue, 04 Aug 2020 05:07:30 GMT  
		Size: 48.1 MB (48082910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f81a418d127138e9fd2b61f4672cca54e0ae99a0e80dfc9fe8d3e5ddec17e02`  
		Last Modified: Tue, 04 Aug 2020 05:10:36 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d5bbdc4e919544701c97acde7b941dcab8bfdb79df875d0d778d1e152cd11b79
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50699779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69051a844be897cb2c3b46ccad8848d17e8df991c26869761ed0c14a13adc88d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:14 GMT
ADD file:0f4a1ab6b889d98f711b241dde31787e633494e233067fe98dce73de73c2d7f3 in / 
# Wed, 22 Jul 2020 00:42:17 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:45:54 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3af651ddf153ddf8519b20c192d158afb60045252366ddc81e15c938b792982e`  
		Last Modified: Wed, 22 Jul 2020 00:48:41 GMT  
		Size: 50.7 MB (50699554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68749f3989b54988d502731fab53de931d3b1cdee8b1932f31552c4296b9c0fd`  
		Last Modified: Wed, 22 Jul 2020 00:51:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:820abbae97c99183daf43e8d6d94304009b63e972f8c2c7c439cbfb930e8bbeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53490589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a318806264bdf6c75ec512387e04dbbf8ae81cffa669589ea2ef513fed52e6aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:04 GMT
ADD file:545a4c28d2d65f9f31d6deed3b22ae80dcdf0f0ba234b36acb715ebf6da67f3f in / 
# Tue, 04 Aug 2020 03:39:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:41:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5671e8963d62284adafd28133509ee2239373c96d0091ce2b4491327cac9724f`  
		Last Modified: Tue, 04 Aug 2020 03:44:13 GMT  
		Size: 53.5 MB (53490363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80a2367de079f8a4dd623d74183ef1cd363a896b59482f0f1e00af6ed7aeb40`  
		Last Modified: Tue, 04 Aug 2020 03:47:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:7f86547c82f2264d26aca71829cb17c0ad9b312b759b5a1fc75c58ba0ac94602
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51079098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:465397e5b9b712511d388011ea972a306d130e6511677447c6bd42062d2a3037`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:10:23 GMT
ADD file:ba027e751512c2bd75301e89e6e4ff2f37ba0d5a4dc18785ef0805c0c44217bc in / 
# Wed, 22 Jul 2020 01:10:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:13:39 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c1d6004a331270728a8745881ac080835166c19dd8097eeccdb751f6118875fd`  
		Last Modified: Wed, 22 Jul 2020 01:17:34 GMT  
		Size: 51.1 MB (51078870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8502524ecca370b2640c107e9e3d047770276ab2c0c0a9dba5a1482167ec9c9a`  
		Last Modified: Wed, 22 Jul 2020 01:22:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:4fc9ce71404a24e0ed4bf740139cd65ca260e75875b80bac42c78a50bf20c439
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56196967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:049c3d587f416f576298478a288746cdfd7d357a6c7dd8a2873f22bba75ccbbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:56 GMT
ADD file:4f9206295fed0198f64e3e8588d30592afb355ad315b7f02a90d92274b37766a in / 
# Tue, 04 Aug 2020 04:46:03 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 04:49:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:54ff323e52b64530253b6d180607b58565d781a9b132031a9baec3e1577690ab`  
		Last Modified: Tue, 04 Aug 2020 04:53:50 GMT  
		Size: 56.2 MB (56196736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f66031f5e2385727f99e208699f6d10108ec45c86b17b6786e69e927e9a0f8`  
		Last Modified: Tue, 04 Aug 2020 04:56:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:7cd84df58894b83666edbbd9a0267f1c3a7065af7fccfc9eb2760155b2d960d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50989903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faf5fc14276aeade613b9a7961171dde3bf169e7cef0c12fd34d74886aba1dc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:26 GMT
ADD file:a96b6121a19d104791604cd0cd10ee066e9d0f56abcc8f3f9cc1cfa691f2c4eb in / 
# Tue, 04 Aug 2020 01:17:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 01:18:53 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1776f15db22f5bcf0f222cdcea18411e8904b4ebbb37ce537b90d8cea466e2cf`  
		Last Modified: Tue, 04 Aug 2020 01:20:17 GMT  
		Size: 51.0 MB (50989676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb232e1eef173702754cf6bc85a74ce5bccaec93a13feaff5b1c68db6279ed`  
		Last Modified: Tue, 04 Aug 2020 01:21:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
