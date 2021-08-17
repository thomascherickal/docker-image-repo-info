## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:f3620a232e75e1695c8ee5b071568cc9d19643ff8d11500049956639efb694fb
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ab39f3e341420cc3411166bb491cf3027d29b3fcbbd46732e08dbae64de333c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125497790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa631a2485826e940bff6455e809e8fbc7df712a207d0a9c86e80ba0d9f9a93`
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
# Thu, 22 Jul 2021 01:11:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ffdc07b7fd300200574dc6b90e8ea9a32d74f4ea4b636dd9345a7ba9eddb6d63`  
		Last Modified: Thu, 22 Jul 2021 01:19:04 GMT  
		Size: 54.6 MB (54568159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d79f445afbbd6acb2215a69f20541c9d56a1b4ba2e8ff84657bb88d80864b968
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120396310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c16b7b3d740373fe4ea90b519dea09beee43b722f52f0844a94073b1c940b28`
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
# Thu, 22 Jul 2021 01:59:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:7e97cdc24ec30abe03f9627670d9c6fdc1a0ab29f0b07f7fa88f04bf60d82cbb`  
		Last Modified: Thu, 22 Jul 2021 02:18:47 GMT  
		Size: 52.3 MB (52318648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2760c810fdf6cb356ae80d60757692017c9a3ee77cb4c3ed69db87a7f3696101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109742256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3078ae742bb9dbd8ee8c5e5bfc4522d5849e6a68bb2a3ff6d5d0243abb741690`
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
# Thu, 22 Jul 2021 04:15:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f14bda9bdbd404cfcf13425f9c6273b254196ada60d6315690312688674624a7`  
		Last Modified: Thu, 22 Jul 2021 04:36:20 GMT  
		Size: 47.4 MB (47356980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:aff370b4cd7e6a60215362153b714d056d5588089fb1ecfba0309ace4f9d5350
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124276344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abed20e14679d3c1396ffd7fd24e687a9cf8abd0840f542b99d5ff2d4c55797a`
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
# Thu, 22 Jul 2021 01:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:194bb6aa613f903b9f28f6985407c4a3ef71b0c952902f6fc70c211f30b77af6`  
		Last Modified: Thu, 22 Jul 2021 01:24:03 GMT  
		Size: 54.7 MB (54670808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:59d9b8aed9f4360c5a06431b5068bf51842c7e73f4f67a1dca814d0f8ab55ae2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122983094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a91a520e6d1f6f0876eadc1b1dc9a61a17ca8750c842dd76cd95763eb639fe`
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
# Thu, 22 Jul 2021 04:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b349e22a93ae2ec7a8fb4830b9b80b272c758fbff384a0410f5c834c9c26a681`  
		Last Modified: Thu, 22 Jul 2021 04:16:00 GMT  
		Size: 53.4 MB (53437923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9ea087b587f4c562df0cdaf23b305718e546280c076ef138de90a484e2b74ac1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122443159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d90ed3c23ce5e02d984742168710ece78b02f6547631e776d5fe7626584f1da1`
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
# Thu, 22 Jul 2021 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c1798d788f2501ab1d9d5cc30f8b8d75d14f031ec0a34d2e5ef594c7e01a42c7`  
		Last Modified: Thu, 22 Jul 2021 00:51:46 GMT  
		Size: 53.3 MB (53298870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:847da11cb3dcc7ad31d69cd17d8e47b3fc855d797f8d36535d84ca37f46aa17b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134690808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b882a50cf017c0ec18a8a4536409e5c517bca228c11874099c4f3f266b6e8db3`
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
# Thu, 22 Jul 2021 03:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:134c811e4424a1c4ddbf1f572dd8c99171109b77c4669802dc6882335b1bff31`  
		Last Modified: Thu, 22 Jul 2021 05:11:07 GMT  
		Size: 58.8 MB (58849943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b230e053038544fd7b4eaa8c63c32358ec0d20fe0ad23f363f6c78d6e19bdd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123123383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e4ae86c0a5a3ff2b89e08111f4e22460aa27f292d94f71a44b73e9b6d4a0860`
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
# Thu, 22 Jul 2021 01:06:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e93975c70cfc2cdc91261d061f2a72ad8ea1d64b7834027ba9d534e3f9e10cff`  
		Last Modified: Thu, 22 Jul 2021 01:26:59 GMT  
		Size: 54.0 MB (54041879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
