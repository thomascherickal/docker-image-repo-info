## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:578db6de3b4f2c03445f7033b44df05504e73dab301be6ecc0d55fb9ccf7148f
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a2c11cc136e04e9a17eb0eac117518009dfd9b98463b1ec6fe02f6ed6ddc9fb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70929631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d539c19a2e4d67dc27f9fde21f2265749bb74412a8572776b5cb51f3fe859c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:10:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:10:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f297180bbe0db88491e987de8d4d906a7563841410d6277d4c2521f468f99fc`  
		Last Modified: Thu, 22 Jul 2021 01:18:44 GMT  
		Size: 5.2 MB (5153121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e579aa043ff0aad70960242128139ee1794c78c546a95105867ece202df88e`  
		Last Modified: Thu, 22 Jul 2021 01:18:45 GMT  
		Size: 10.9 MB (10871661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4816282fc7fdacd2af72ceb5ea9de50be9ee6134c76639bc9864e7987d74f20f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68077662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64abb049076e775a8d6453119cb655d67b7f5752b031b098568d25eda42fb8a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:48:40 GMT
ADD file:a5e191f39728e6e12b8f32edbaa7920930ceeaa50bd5db8a28faa1325a03c877 in / 
# Thu, 22 Jul 2021 00:48:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:58:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:58:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:54f61193f2822104b288f4b662f2a516401b23e0fba11d7ca2215f06378c96fc`  
		Last Modified: Thu, 22 Jul 2021 00:59:59 GMT  
		Size: 52.4 MB (52443094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fe553c5962741d3f2886a01d834839adf275ab459fc0e141cb7923436d736d`  
		Last Modified: Thu, 22 Jul 2021 02:17:54 GMT  
		Size: 5.1 MB (5063630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3979ca68793ff901e46109197cce75ef32b748868c9828a1553e9884e1646bb2`  
		Last Modified: Thu, 22 Jul 2021 02:17:57 GMT  
		Size: 10.6 MB (10570938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ddfdf5e8380f8ef257e9c89fc47013d7cc22d71e9dde4f7dcd9dfb3f652075ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62385276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588a1e4f35a98591d5bd72165b43fb04a6de8ca064f41f1a3a6009a0bb4a4ced`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7bd34e1a723b526268abc85d400a08d415e43d9375dda9b43ee2769c9dfd9473
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69605536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28f30cff4e180130b1e29d79daaaebe65deb5e2089aa65daac21c87ecead82d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:37 GMT
ADD file:6733d7f2201aa0027287de4f81a7cabfb79c331e290d9d1f16bc68c8c0ce1473 in / 
# Thu, 22 Jul 2021 00:39:37 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:14:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:14:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2fd60d6781333dbb2e2b453027f2c16737edf4afa6edc775fbe4983c9196c83`  
		Last Modified: Thu, 22 Jul 2021 00:44:34 GMT  
		Size: 53.6 MB (53590358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475276876369c675045edd5275dfaf6d54f4ca13a77dd33835b145e4f6dbfc4`  
		Last Modified: Thu, 22 Jul 2021 01:23:42 GMT  
		Size: 5.1 MB (5142492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1a8b85717d6fe3eedef14320b0bee76ceefdae31623ffa13a264a78ae675eb`  
		Last Modified: Thu, 22 Jul 2021 01:23:42 GMT  
		Size: 10.9 MB (10872686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9d914aa662e0a57a699a0c20bd1ccdd39f9fed977aabc774d04ae69e09ac6bae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69545171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de77084f6a59989e7e7d0d5f5b6cc3be4bd09c3685e19e98dfb8c3425513ce40`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:33 GMT
ADD file:574afb2f0b9121fa552563f323a2edd9a3aa71fc927a280c3eb9cbbf944a12ff in / 
# Thu, 22 Jul 2021 00:39:34 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:05:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:05:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:276c935c592dc1b2a80709bfb684b8cadd019d62fed321da14653e74bc260bd2`  
		Last Modified: Thu, 22 Jul 2021 00:45:59 GMT  
		Size: 51.2 MB (51206749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74777b942e5ddcca1441a21360061ce9f880ebd5f5020bd1f8480c09ec3c9a1`  
		Last Modified: Thu, 22 Jul 2021 04:15:32 GMT  
		Size: 8.0 MB (7998524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f821b4d53bda0dd46941c09587233f0b5d34c76bd3efb4d2d0766dddea8f99`  
		Last Modified: Thu, 22 Jul 2021 04:15:33 GMT  
		Size: 10.3 MB (10339898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ebced0a8513721147abfc40542be919bd4aae2522a75ae4856d41b93514796bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69144289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e43642fb3e135fb9af3869d9467c8beae3e5bf070f39b69b0babebfd123da788`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:32 GMT
ADD file:0528720276c3b3b11a00595363f8a514e2655bcf1e4d9b8ba3f79621e44f0460 in / 
# Thu, 22 Jul 2021 00:08:32 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:37:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:37:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf851126a635ad4c2c2a139ad19f922e1a4ce737641a782c32519868f02d804d`  
		Last Modified: Thu, 22 Jul 2021 00:14:07 GMT  
		Size: 53.2 MB (53156287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03208a775bdcf86ef328e8eaafb6230b1df65f5e3f7134dcb25e12a4148a24e4`  
		Last Modified: Thu, 22 Jul 2021 00:50:55 GMT  
		Size: 5.1 MB (5114712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afb8c727f6f423fc30a90decf5892b3aec16edcd914824275b6e0b56e6a3dd1`  
		Last Modified: Thu, 22 Jul 2021 00:50:57 GMT  
		Size: 10.9 MB (10873290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e9110d2d67edbf0545468e56c98257668a90b6cd4205a0b8a98f352e5c409393
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75840865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d29d127b80c7e86e00b1763127e3b7b3d9988cc00699696c65ad7ed2e0755fa4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:09 GMT
ADD file:aadb38c47e4a40c11e7ad3b380075dadabb62c20584e02f089c2e5c957ce04cd in / 
# Thu, 22 Jul 2021 00:17:19 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 03:44:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 03:45:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c0acfc4b0736fe9b7465e9b5f83f277c5a237585bf07da22048883229ecafad7`  
		Last Modified: Thu, 22 Jul 2021 00:26:21 GMT  
		Size: 58.8 MB (58813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847221653bad212b7cc4f12cc2ae7b27ddbe29dce9a8988bdf32b8df41945d4f`  
		Last Modified: Thu, 22 Jul 2021 05:10:01 GMT  
		Size: 5.4 MB (5401706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92fec3eb594016967ad2f4e5bbef1754a9733c560b8449f5e56969c8486d27b`  
		Last Modified: Thu, 22 Jul 2021 05:10:00 GMT  
		Size: 11.6 MB (11625843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:160f9f554cb8757e9becfe92860e894d25480cf2bfb006d2ad40589c1f78ed8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69081504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe594321e46d1328b0aff023a390f600246bc71c44172641a3089a0b02fd8274`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:34 GMT
ADD file:0a2fe191e4bb0a90f32a0829f6d49407139fa2c3517cc2097c51a94786075a8e in / 
# Thu, 22 Jul 2021 00:41:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:06:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:431c45f9c46bd0833127af2c090d5f6776b5c421df2849de5f3071102212923c`  
		Last Modified: Thu, 22 Jul 2021 00:47:15 GMT  
		Size: 53.2 MB (53183556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661dc83d23d8e8891a8b01ec648db5ba5f59655fd1afd8c0be9ae256c3f9840a`  
		Last Modified: Thu, 22 Jul 2021 01:26:41 GMT  
		Size: 5.1 MB (5136979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fde1e2e331c02b4294f5f9f803a4aa4f31be7389c20abd265788d916aa771a1`  
		Last Modified: Thu, 22 Jul 2021 01:26:41 GMT  
		Size: 10.8 MB (10760969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
