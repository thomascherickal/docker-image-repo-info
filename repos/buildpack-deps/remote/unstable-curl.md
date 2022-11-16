## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:19e89efd35038ef8dd2f2fa30a4af5bd8940da8cbcd4ea2aedda2161b2dd0186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3dd97354753d00b7d50045606037c25ce69a6d50d6bdb36d8d891d9b1ec080ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70696505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afb86bcbc3cc92f9e8bd1142361299cdac4e2abdf942adc1db58a550f47c96e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:42 GMT
ADD file:ace32e845b2ef519c79a725518e909bcbe50ecb496c1dfc8e96fba83ffaf685b in / 
# Tue, 15 Nov 2022 04:05:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:27:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:27:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6bf34ac41ed5383f401a5e77ae46b55249a145be0fe8eb1bf8f0e4f7febfb2a`  
		Last Modified: Tue, 15 Nov 2022 04:10:16 GMT  
		Size: 50.3 MB (50311341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f3b9f46f2031bd413417a1f8fa2105dc29dead8d7a2147b9f742ed2892b77e`  
		Last Modified: Tue, 15 Nov 2022 10:33:48 GMT  
		Size: 9.0 MB (9017772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90be89ed4a456d300e722fcd8f6c47b8e993b6a5037babce8a1e9d84a98721`  
		Last Modified: Tue, 15 Nov 2022 10:33:48 GMT  
		Size: 11.4 MB (11367392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:38a9b9c598a27fc56851dabc393c6e67e8b296ad02f1c656343864375e369666
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68770559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c5a96396ede69f2d6b03b0782e907a9516662142c06edd3c217531aa4118c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:31 GMT
ADD file:08f8312faaa666d9d1d3cdf1e0ac577979317e8784c264b29b4d3399045d2adb in / 
# Tue, 15 Nov 2022 01:49:32 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:44:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:44:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:351340891f63641ac5516af46a2dfb6b370ea5971d604352dfe16a498646eb52`  
		Last Modified: Tue, 15 Nov 2022 01:54:51 GMT  
		Size: 49.3 MB (49284160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989d5b3af22bb23168efd5d127277e94392a88454e93916c8136bdbbbfdb6c07`  
		Last Modified: Tue, 15 Nov 2022 05:49:45 GMT  
		Size: 8.5 MB (8471398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae7d5b628dfd536fe95d650285c66873a6d0e49fe2d657c2e7317203d6f01c9`  
		Last Modified: Tue, 15 Nov 2022 05:49:45 GMT  
		Size: 11.0 MB (11015001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:128155a05d3f0ee18241f126cf486c8874335c1cc1211da205d755facfb33ba2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65869782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc6d24591d16eab2378a7ba18a0d6d97d1a628103c100ef206cff0d32de86d7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:44:42 GMT
ADD file:c9d57eeb50bde8da5c06a8e258d811f84122cec325dcd8c9c1f0af577a00b5ae in / 
# Tue, 15 Nov 2022 03:44:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:21:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7d8a148f561149045bbc5d86c167ced3751471156eb66153a1016778d252dd2b`  
		Last Modified: Tue, 15 Nov 2022 03:52:03 GMT  
		Size: 47.1 MB (47101515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bbf5804490f04cf07c9ae3465612e6d50992dee8569dbd438cc057a10043d6`  
		Last Modified: Tue, 15 Nov 2022 12:30:56 GMT  
		Size: 8.1 MB (8119685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112e7e52d2fd4f92051b7dfa6935fbaa1f6507fcfdd8cf186668717e83c3468`  
		Last Modified: Tue, 15 Nov 2022 12:30:56 GMT  
		Size: 10.6 MB (10648582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee5e36107f8dbb0014f2be3fb5a9b6d8fb6b903885b498baef286d9d66d650c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70553982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34321eb368f5c3a811c2bd715f2b1f5eda6d3f63239813faaf0467cafb0a4ddd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:54 GMT
ADD file:ba227e9990636bcf4ac74991aee2f89f076de2adf7a651c75b55b2dc145b5340 in / 
# Tue, 15 Nov 2022 01:41:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:39:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:39:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4831e9d6ed52920992a4dda63cbeb8f430d77a27377294be499a02b93fb1e3b`  
		Last Modified: Tue, 15 Nov 2022 01:46:00 GMT  
		Size: 50.4 MB (50371180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28af2f647d544013c2979fcc9bb3234c113dc9496fa976cc4a2fdf6d0622b2d5`  
		Last Modified: Tue, 15 Nov 2022 05:44:45 GMT  
		Size: 8.8 MB (8849884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70069958d3a3ba34e8ab2a47caf5d5f7b8a3be5ff9bb2a50385ea0deceeff91`  
		Last Modified: Tue, 15 Nov 2022 05:44:45 GMT  
		Size: 11.3 MB (11332918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7b60fdf2e5aa3a99a594d6da2ea2cb53184e8bcfa6815d516fc48db2e8cea206
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72130417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b61ff377e076884b3e6cb24d188ca8c72a53f41936346cc8d4ecc2c1738d321`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:30 GMT
ADD file:6c7cf2ddf77e13ddd1b27b3e2895b29bf27b8fd6d38de6f5fa7330138f69523b in / 
# Tue, 15 Nov 2022 01:42:31 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:07:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d85d48acbb26d22f92c31ab4d483ab5c9fc0a7db5f67806b2c05a4460060ee4`  
		Last Modified: Tue, 15 Nov 2022 01:48:49 GMT  
		Size: 51.4 MB (51364090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342a208cb77d0844c504e83c807857939a67fb80f38ffb6fb74e683902d17e74`  
		Last Modified: Tue, 15 Nov 2022 07:13:55 GMT  
		Size: 9.2 MB (9195422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e99437fd05453ca2e9063e277126421e73474415f3eaf15d08239e2c8b01f8f`  
		Last Modified: Tue, 15 Nov 2022 07:13:55 GMT  
		Size: 11.6 MB (11570905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4d928f26cc9acd47ee8834614266a88bf1a34b000293aee0f9cffbe125fd1478
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69835077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c61b4112a60db64eea6c67e435864bc06ac8f02b128d3be8803fcacc7b2db23`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:14:16 GMT
ADD file:c60a8c207626b9bb85c6ab0f734c92f0094d59427717e2d7624cb29ccda64e03 in / 
# Tue, 15 Nov 2022 04:14:21 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:19:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:20:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:facbd376e86382e65b5fd1d879de9db0a46c5412257cfa0e54979c08f55d5d76`  
		Last Modified: Tue, 15 Nov 2022 04:21:57 GMT  
		Size: 50.3 MB (50328430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb7200d19fe8446547c31e404a6f0d1dd78af22a5857faf3bf52bb0e2edc230`  
		Last Modified: Wed, 16 Nov 2022 02:33:53 GMT  
		Size: 8.4 MB (8383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1225c18bf70ce7954ce372d2f190193ac1c43b5e95b22043f776ad430a14d755`  
		Last Modified: Wed, 16 Nov 2022 02:33:53 GMT  
		Size: 11.1 MB (11122840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d42043980bc5da1bb62b215e0d0f2987e586fa8214a997a275dd248819fdad36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76096486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aefd52ce3a5525cd361553f73d29257be1c8057d88294ad05487cfc67657961`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 05:19:03 GMT
ADD file:c691cfa7b342c661a15e7340e21b9cb0cb8e6a644d7f906a4ba51b0cd2067dc8 in / 
# Tue, 15 Nov 2022 05:19:05 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:00:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:00:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:719747a616fc8430b4c2e7997caed399c462d6f82d9391346afb14e534b4e95c`  
		Last Modified: Tue, 15 Nov 2022 05:24:50 GMT  
		Size: 54.4 MB (54373524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccec34f678290e1c230c4ab38c65ddeb9cffc3a03963ed9534a7e0832531920`  
		Last Modified: Tue, 15 Nov 2022 12:10:01 GMT  
		Size: 9.6 MB (9596687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946af2283f978ac052c25eaa609fa290c33d729f2bdeb836f2a9969a8c0bd01`  
		Last Modified: Tue, 15 Nov 2022 12:10:01 GMT  
		Size: 12.1 MB (12126275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:20837254e0924117334eafd2ce6a296c897e796ceacc170d92b82d8540a87493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65429748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cdd599eca8933f09bec0ba7d28d27e9dfd0a4b3e75c6cea7bd6a207fdc09ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 02:10:35 GMT
ADD file:3605614f06115edb2ee0a2db052ccf985f2ee967592a4a9eb4f53585907a0c01 in / 
# Tue, 15 Nov 2022 02:10:37 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:57:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:85e0ffe5757d11394c39fa959f3a2cb0a9d1e43dd8d00be2c77fd6fdd43a4041`  
		Last Modified: Tue, 15 Nov 2022 02:28:37 GMT  
		Size: 46.6 MB (46576018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55dc9b61880194396d69e084a5b3a8cf11c21be0f9286759993ddf4345099ff`  
		Last Modified: Tue, 15 Nov 2022 03:27:59 GMT  
		Size: 8.1 MB (8110952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa050e3d5eeb4149cde6a3c170a41a310d6c07d1eaddc43ac45cc21d7d888e`  
		Last Modified: Tue, 15 Nov 2022 03:28:00 GMT  
		Size: 10.7 MB (10742778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dee08d165923ab59dc8bc44a9591bd55105c09b1dc568907adcf56c58e68dc53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68602611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8c1af47551b217b3c5d46038f09bbed68024be4cb8016a719a4c82bed954e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:43:11 GMT
ADD file:47253af7a4fe925d592c8b6d41b8dff6122bbdd083ebe6ff091bd90271f78b19 in / 
# Tue, 15 Nov 2022 01:43:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:27:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:27:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ba49eb7f21a2367672851b25b6c120e1a153fdf9884b643d9b288f026a56ddcb`  
		Last Modified: Tue, 15 Nov 2022 01:47:50 GMT  
		Size: 48.7 MB (48716895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a177a53296ae0f27e3066a0176da64ce91aad46f8e4ea7f8c96c9311b9a66820`  
		Last Modified: Tue, 15 Nov 2022 06:36:52 GMT  
		Size: 8.7 MB (8651091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd00d59dc2ed724777bd708f1d6bc0056f53a561c1d8223416db44c865f6d040`  
		Last Modified: Tue, 15 Nov 2022 06:36:52 GMT  
		Size: 11.2 MB (11234625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
