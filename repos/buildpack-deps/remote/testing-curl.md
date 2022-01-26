## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:70d61737b46554e5d1216b6be79cd7562b47bd9587020cb0a2685fe036ccae24
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f3da2cc44789b12ac32ff890978391854bd16a112d7a853bb8ac6e80411c5945
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71756351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac940c831c1ac41a355f37cd6cb248e27d30d519ce8f6ae5dc87d6a88ac193d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:57 GMT
ADD file:049a34b0a455f2d6bb7472efc8b4fe28600f9b16fcf86c66e654f0d7f96c617b in / 
# Wed, 26 Jan 2022 01:39:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:174dc37d1760a198250a591524de55fe80951eb332d1b5fda14aa58b2d0274ae`  
		Last Modified: Wed, 26 Jan 2022 01:45:22 GMT  
		Size: 55.6 MB (55560743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ad4f3c5938976e31cd1193f27047d074e6094f3e599687768b82217ddd84ef`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 5.3 MB (5280293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ef7f4634c596ef4c86e1e87d912ed9ac6798192b66dbec54ebf05b66e5023`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 10.9 MB (10915315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:091330f426c9e0e2233be42519d54a92d9bd56ffa9bd645bc80b699d2b55fdd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68785328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687f0a5e0e48850c1d6887d982d9b8891e1d8ade867928873759b1ff5461fa22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:23 GMT
ADD file:2b96a854a3c9d11256be667f9d982d7d8b9dc55dbebd8b4b5fd405cb278a1c64 in / 
# Wed, 26 Jan 2022 01:40:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:63d07b82886a825f18700c37fbcff6322772ad2aa7c6337ed53204a0fa13480d`  
		Last Modified: Wed, 26 Jan 2022 01:55:24 GMT  
		Size: 53.0 MB (53020183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786dbbcc14b50d4e55a52a72c123614a491ab523193b076c2c3567fdc1888969`  
		Last Modified: Wed, 26 Jan 2022 02:51:24 GMT  
		Size: 5.2 MB (5182484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1bb97567a73aef32ddc428fed052ca711f5df4a1975daa855a68c2d3ce1ae`  
		Last Modified: Wed, 26 Jan 2022 02:51:26 GMT  
		Size: 10.6 MB (10582661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:78e899cd5f9ff4dcd9f56e8a3069127d9b0d84be511ff6414467d7424c2fd5e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65944870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd723f48462cffa5ea3a277e6b73f5a3ffaf5534aeba927dcce8e90a99fe89df`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:29 GMT
ADD file:0d5c36134a34929922dcd5c83256b9539a94c46d5b7dcd23ae6cc29721bdc320 in / 
# Wed, 26 Jan 2022 01:40:30 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9276ec53f1a5aac51c0a8a27bcc855b50a696f144903a4c1dfab1a458f7f7af0`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 50.7 MB (50662778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faba8178fd562af6ed1b6193d73a2eefb5dbc9bc34e5e155d0b644f8d23281a`  
		Last Modified: Wed, 26 Jan 2022 17:00:54 GMT  
		Size: 5.0 MB (5040739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de84da60e6b5c715dc34fc6124ae223b3288b8777242a15fdfb7dd0d91a9261`  
		Last Modified: Wed, 26 Jan 2022 17:00:56 GMT  
		Size: 10.2 MB (10241353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e0a874be6a4b6d4b6f74edad05600e3f8d3f16bd96a69f88208516718daace00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70481599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0139c08336b3e1cca84fac2747c6ca8933f56e35419a31d9b1ff6dce4d17e808`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:585d9a04ed59d36d1ee8be3ad5a7a488962b12f0b7d737826e25a7ab617521fe in / 
# Wed, 26 Jan 2022 01:41:53 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f9f8cc8e22fa2c53a109b770bcaab20fb907dd9957eb312d9f49000ff4185f8c`  
		Last Modified: Wed, 26 Jan 2022 01:47:52 GMT  
		Size: 54.5 MB (54535243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8a0926c8b86f048958ba5be5355985e20305f2a6df3fd52b867ac3cfcb7ee`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 5.3 MB (5269783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7042a90d872d1ef29a580051968c7437ef7f8f185841fa2ddf3e7bf37bb0593`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 10.7 MB (10676573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:eb298b385f89f18fdabcbcefde8df65ae1571012b2ba1497354dd4abcd62670a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73317908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b194a913a11dc86237a2bb1f4c00bb52b79fb7c1ed8edf4290be71c709ec681`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:06 GMT
ADD file:49bb0653fde7eea7609e6ad9bea8c405d8a514818936cff57f87f5fa321d2582 in / 
# Wed, 26 Jan 2022 01:39:06 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1308dabb988bd1e94f15ca40572eaddec8a0de059ca7c28b6a83e6821441d6f8`  
		Last Modified: Wed, 26 Jan 2022 01:47:24 GMT  
		Size: 56.6 MB (56598143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7ba5a7115e901688cba13f3ffc91e6ab2cedb7a7cff304d4bbb5606c507f4`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 5.4 MB (5412384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7645e93b83f1c523ab6c715a08bbfd71c80611ee830755b1e36db82d26c1eb2`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 11.3 MB (11307381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:967bf73e69c34cb93977066405f6856089ae2812f76dbedaebb5bd60f25e05bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70372086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a305aa32aaf93ceb021b00c3ee3956772b9970ffca8ab93e7d87a8d20322afa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:27 GMT
ADD file:cb994d31e0dc06b73ce5e197fffe27837867fce8ab87a858b9668290c97bd7af in / 
# Wed, 26 Jan 2022 01:41:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:45126d37a1c34eefb327242a121bbca1be988e1e2e1cf037fde7eaa131fd6db7`  
		Last Modified: Wed, 26 Jan 2022 01:49:20 GMT  
		Size: 54.3 MB (54262039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9463250f8710e43e5aff116a08f617cbc14f10997bd69f2bda7a81f002b2e7`  
		Last Modified: Wed, 26 Jan 2022 02:34:27 GMT  
		Size: 5.2 MB (5235335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20371ca4b02d263c2ebdd04847579505ac45245b979462f3374b0acdda280fb2`  
		Last Modified: Wed, 26 Jan 2022 02:34:29 GMT  
		Size: 10.9 MB (10874712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:67ab1b9d2312cc921dd8201cc2f794f9e66aaae65c6658e425e5d1b4714a1f5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77180005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a7f9a9fc27e8cb5baba34f3538b896dbcd82738a3fe90848a8b07fe6bf32681`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:815d918aa7e03d3a0e2d0dd87d7d9696feb37b5054d103e1ac83847b08e877a2 in / 
# Wed, 26 Jan 2022 01:45:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2fe2b17ea8278b5a905731f1d003664a61c7774f4a23cda61a596487a1b51210`  
		Last Modified: Wed, 26 Jan 2022 01:54:29 GMT  
		Size: 59.9 MB (59942176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4cbdc2b57b1d5abc56a5ce2448279d438e672ad3740a30808c6aca777b1ba7`  
		Last Modified: Wed, 26 Jan 2022 03:13:11 GMT  
		Size: 5.5 MB (5544663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46175642455b8055d9ddc0cbcac8518413ed6ae29f42a87871058a9c7df76e08`  
		Last Modified: Wed, 26 Jan 2022 03:13:14 GMT  
		Size: 11.7 MB (11693166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:251befcbef07f1981f6d2e9585cc814e80286d31efaf808cb5b17c0d83d929ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69903067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953933c309c0113106ec3a520807b7052e18c818dfbbe643a7bd8e3bb8826e48`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:21 GMT
ADD file:b56123b23454cb9db7a2a2e19c5219cf5643b8692bc247ac4212732f2a8d218a in / 
# Wed, 26 Jan 2022 01:40:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:06:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:06:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4155c67ca83ba1ee87acdfb0ff7b262e769e0a27829b9b44ca097c4ba1e29ea4`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 53.8 MB (53837097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610ffbd8c4fbe8756d41005ec7da9c699f84722392728547ac79401b01064e8`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 5.3 MB (5259010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed15a8cf3570b9b0ddac9365776ad36a5024968df38f3bef0cabb5d6a953eb`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 10.8 MB (10806960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
