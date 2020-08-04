## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:dbf9f9a4f33460eeb44f7952e97056b0200d56db8076d824a15efc35b737f8b2
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4d90f763d599b00e25b29d27ab052510e9c329109e385f939b5d5392bc392740
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70842736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e55b406fb3d062a11aa327481f39e2de7a119ced85eb98089a074170d22a0b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:05:41 GMT
ADD file:388f29164844b8493d30bf1feffd1158559ab161886928f977604c10f983a704 in / 
# Wed, 22 Jul 2020 02:05:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:09:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:09:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:babaea2ea26ef0e3e4a90ecc928d26bf25d699e1dcba843f16b8a2f0a153b3d7`  
		Last Modified: Wed, 22 Jul 2020 02:11:28 GMT  
		Size: 52.3 MB (52340330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a37a5f4c4c2303f8d9f818b910d8f9caefdb8cf414a4189c131fe87eac26c2d`  
		Last Modified: Wed, 22 Jul 2020 03:18:23 GMT  
		Size: 7.9 MB (7921724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a136692b9cb363269d4efa1edc43bf0b539b0495b6ab5f8229f02319829642`  
		Last Modified: Wed, 22 Jul 2020 03:18:24 GMT  
		Size: 10.6 MB (10580682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0811f0b7fe4a35b7680a6d2dc5903bf226d9044ec62c4a6f0707b401dbba2d0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68078676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5afb63e489b0d32237c72566b02e4ff1c8ed14f602c717f47b89d21ae8a750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:19:33 GMT
ADD file:966adedb56b8840e71e14255f1e10c11506897b861f32a0c8c84c32338edea04 in / 
# Tue, 04 Aug 2020 03:19:44 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:24:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70fc41871a830209ccc29805b1bb08b4058beb41df471ae13bc23555229a9623`  
		Last Modified: Tue, 04 Aug 2020 03:37:01 GMT  
		Size: 50.3 MB (50310118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c042826fa49924c4933b5f443c67da73885272c029983f30a8e5a154ae5b2ba7`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 7.5 MB (7501462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f2d1c9e043d778892369b2ac4ba55c261e45346581518d8e9c0923f580979`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 10.3 MB (10267096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5adb126559f397317c5f8579e98e2e1f60d55cfbe577b1b821a40e7e603ea9bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65206178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d85b1b53dd0e5f5e0c0d720a78c825d9947c359a59e39fade6117c8f700aa2e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:27:52 GMT
ADD file:3ab6a11382a4a9f69a874d734a83342969068fe2d2a62b325658fb5ac421f650 in / 
# Wed, 22 Jul 2020 01:27:59 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:44:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:44:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:04602b0eaf483684b8d51ffeb79a3e05e2f29421e1090b3050c1b163ef02f10e`  
		Last Modified: Wed, 22 Jul 2020 01:42:51 GMT  
		Size: 48.0 MB (48046591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663484832f716cffa80a12254c44159fcadc5117183e18db5726002b9044e907`  
		Last Modified: Wed, 22 Jul 2020 06:04:56 GMT  
		Size: 7.2 MB (7243496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3453c2f59de86c76b43dd0cf5ffaad07ce27d7ec246c4d7a72032197a5210d`  
		Last Modified: Wed, 22 Jul 2020 06:04:59 GMT  
		Size: 9.9 MB (9916091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0a8ef4e73d140ec302562a650384a262c0c993b49794922a30f31f033c692109
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc8434f98245925c03f22f2d68834302044c7db1b8fb9c120bfd1a919e0400f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:14 GMT
ADD file:0f4a1ab6b889d98f711b241dde31787e633494e233067fe98dce73de73c2d7f3 in / 
# Wed, 22 Jul 2020 00:42:17 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:21:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 01:22:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3af651ddf153ddf8519b20c192d158afb60045252366ddc81e15c938b792982e`  
		Last Modified: Wed, 22 Jul 2020 00:48:41 GMT  
		Size: 50.7 MB (50699554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbb2a684c92e31711be180ca45ac19643d88c12a51b2ffb58b6f120bc5ded2`  
		Last Modified: Wed, 22 Jul 2020 01:37:00 GMT  
		Size: 7.8 MB (7796374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdf66380a30dc7828150f57df61c812d1fd653b195e8f5d57dcfb885adedbf`  
		Last Modified: Wed, 22 Jul 2020 01:37:01 GMT  
		Size: 10.6 MB (10588039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c7f332933fb7e2b24c50062fe5eb80e3b38199fcadbcfc711056220834d1e366
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72492901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef7f458436b8df627585a063fbef57b6e618516fd1e7b7789e0fe7f841e29f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:11:12 GMT
ADD file:1c3529ea5c695a0705497b4510edaf2034b3d29a608dea3db741a4298a117d33 in / 
# Wed, 22 Jul 2020 02:11:13 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:32:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:32126ce0c55cb16ee9848f6d067e47a287f981a106ba123e3f2590544677f0e6`  
		Last Modified: Wed, 22 Jul 2020 02:18:12 GMT  
		Size: 53.4 MB (53433577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9e403cd592ae856cb4192dbfde1073d62172846377a957e99aa1612f15c17`  
		Last Modified: Wed, 22 Jul 2020 03:43:32 GMT  
		Size: 8.1 MB (8099028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23d35b0ead0819c716d1b9d778e65755014b69dde5807f1cf3a6c95a4a73dbe`  
		Last Modified: Wed, 22 Jul 2020 03:43:32 GMT  
		Size: 11.0 MB (10960296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5b7ab11513c31c67cf6f4e6dcff77a967854117020cd435dc8a0c02b0bba6811
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69127881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e64f00b8a1b428dc22779c0bbc1fae216f7c1d0458619e29949feebf8c794475`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:10:23 GMT
ADD file:ba027e751512c2bd75301e89e6e4ff2f37ba0d5a4dc18785ef0805c0c44217bc in / 
# Wed, 22 Jul 2020 01:10:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 10:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 10:39:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c1d6004a331270728a8745881ac080835166c19dd8097eeccdb751f6118875fd`  
		Last Modified: Wed, 22 Jul 2020 01:17:34 GMT  
		Size: 51.1 MB (51078870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fc8ab221636edeabd2df88a6e60355b1cd646986a8adb8b6e026bdb27a37a6`  
		Last Modified: Wed, 22 Jul 2020 10:50:36 GMT  
		Size: 7.5 MB (7450064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab2cfa46cbc90566aaca1e1931fc9c28d4dacc60e71e68bc28c5e245dc5a178`  
		Last Modified: Wed, 22 Jul 2020 10:50:37 GMT  
		Size: 10.6 MB (10598947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e10cdfc9179ea15af6420137258d00d9fb2b38e2b9b6ae9c1bcbb17839326f64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8975b9f62538715768da62d7deb42a5937d5c896fe8d1c29326a7b20c07f3a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:56 GMT
ADD file:4f9206295fed0198f64e3e8588d30592afb355ad315b7f02a90d92274b37766a in / 
# Tue, 04 Aug 2020 04:46:03 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:25:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:26:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:54ff323e52b64530253b6d180607b58565d781a9b132031a9baec3e1577690ab`  
		Last Modified: Tue, 04 Aug 2020 04:53:50 GMT  
		Size: 56.2 MB (56196736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6163322bc0beea20fbb00969be62fd8e2c8790b205e246ff0b8d2a3b72ed82`  
		Last Modified: Tue, 04 Aug 2020 07:46:38 GMT  
		Size: 8.3 MB (8347727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8dbc9e7891e1d54106baaa34d375e35b66be62a672cd47f7d6388f7ed7797`  
		Last Modified: Tue, 04 Aug 2020 07:46:39 GMT  
		Size: 11.3 MB (11327086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:139b8b9f378c8a5a5bae8d531018c939f5ae6f6bcb9dac0fc364a3093bc209ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69036220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b2d8abeeaa600153fd25d9a904766c625bc6a334a6a82ae0792ca8ca60f12d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:26 GMT
ADD file:a96b6121a19d104791604cd0cd10ee066e9d0f56abcc8f3f9cc1cfa691f2c4eb in / 
# Tue, 04 Aug 2020 01:17:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:24:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 02:24:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1776f15db22f5bcf0f222cdcea18411e8904b4ebbb37ce537b90d8cea466e2cf`  
		Last Modified: Tue, 04 Aug 2020 01:20:17 GMT  
		Size: 51.0 MB (50989676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f212bdfa67a70fdb2386f3fb1144782ba98880a13323180bd4a44055bb72ad5`  
		Last Modified: Tue, 04 Aug 2020 02:29:04 GMT  
		Size: 7.6 MB (7590154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376f4dbf2b7c1eaaff8920fcd760496fead3e0e754c6b5a9d4122863158fba63`  
		Last Modified: Tue, 04 Aug 2020 02:29:04 GMT  
		Size: 10.5 MB (10456390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
