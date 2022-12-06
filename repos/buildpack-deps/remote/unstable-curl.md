## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:87d88a033eaf19c59c5fd55289785da9b5e6a10944b9a145782deb97ea3efe1b
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
$ docker pull buildpack-deps@sha256:cb90d2f70c5df3903f617d8c027941c3095dc472547011b98dbfb5127673b1a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70698692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3426e28065a7daeb5d2125e796c04d273282ccd93a1b19ec774a8055fbb10234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:52 GMT
ADD file:643fde45a6d11f36b1178a022667e74288e58a263ac7999c7cb023cb3fcde3a8 in / 
# Tue, 06 Dec 2022 01:21:53 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:17:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f8db6e5cd5802a750fd04af4eb64a857f779b9c2333d2d830a50d7b2983365c1`  
		Last Modified: Tue, 06 Dec 2022 01:26:42 GMT  
		Size: 50.3 MB (50309617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b904b10ee4925c81495d781c9278243be45e6e2feb4350d4e8780c3c15c9d65e`  
		Last Modified: Tue, 06 Dec 2022 02:23:48 GMT  
		Size: 9.0 MB (9019750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826135e5b952effdf73fc4ca5766716e2efde4728890f709a8e0629212bfb80f`  
		Last Modified: Tue, 06 Dec 2022 02:23:48 GMT  
		Size: 11.4 MB (11369325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e6b513ed07692c4528997c944c4ea2337de9d8f172f57e84c609ea623f5a9c50
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68771521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefdcae0513f02784fa9385b4e14491ff71b367c11acb17a8a22634f221e6611`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:41 GMT
ADD file:2ae6125a895056caf86a0ea412a141fc00bb6485fece6b14db7232b3e06e9849 in / 
# Tue, 06 Dec 2022 01:49:42 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:18:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:18:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:597e07fd6304947f2f5075e2d3adcf596e2fc483cd39c89bb38d405526e7277b`  
		Last Modified: Tue, 06 Dec 2022 01:55:00 GMT  
		Size: 49.3 MB (49283811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a8179cb55c483e9ef86416325d19f993898e7370b10006cec49f11f48c47a`  
		Last Modified: Tue, 06 Dec 2022 02:24:29 GMT  
		Size: 8.5 MB (8473505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698a17cfcb2f3bf2de3db866fee5370a21c0a926022c6b4818c44705dce6b935`  
		Last Modified: Tue, 06 Dec 2022 02:24:29 GMT  
		Size: 11.0 MB (11014205 bytes)  
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
$ docker pull buildpack-deps@sha256:756b9b13d5f31e0bc0096feeb3b81adf6fe5e98aac36259196622bbb78cbe679
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70533739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab24b0ba5f3fd353729ce47b3a75fd2da88498fe5f4f28fb07dd5541a1917e4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:58 GMT
ADD file:465db2e68facfda9a8a0c90d74ca46eaa4c6678539ba23e8b95ed5245b4c014b in / 
# Tue, 06 Dec 2022 01:40:59 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:08:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:08:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4eadaf994967069fdc4c6fb0c34ba7ff8466eb883bc166d386d6891cfde0d540`  
		Last Modified: Tue, 06 Dec 2022 01:45:23 GMT  
		Size: 50.4 MB (50356726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b6dca1666ae51f05a8c2ea3d3c270aea8aede2271632b0d4e6e33edfaac3cf`  
		Last Modified: Tue, 06 Dec 2022 02:13:41 GMT  
		Size: 8.9 MB (8851487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d16d95c8590c9759323c93cfab8c156adbdc5842cd9eb963e118fadbdbf61e`  
		Last Modified: Tue, 06 Dec 2022 02:13:41 GMT  
		Size: 11.3 MB (11325526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ff53a117e9b60e29554ee7b36e4794ea15cfc5d01e251be1394bf4be3cc3cac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72116759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0d7a5dc53dedf29d74ff9f64cdd1909b99dc8c0dd4989d440df464a3290a22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:02 GMT
ADD file:0909d182d8916b1b37783d0c3582c9d3f3edddf6cd27e90100343ed0462c9c75 in / 
# Tue, 06 Dec 2022 01:41:03 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:10:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1cd5a2a4c5902ff854cd1178702a69271f9bf768ae5b99124c16b51e5c2d42a1`  
		Last Modified: Tue, 06 Dec 2022 01:47:24 GMT  
		Size: 51.4 MB (51358972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5c5bef3805a0d8c076d12c22f99b0c27a09807eb93eeb57ae35352e352cd30`  
		Last Modified: Tue, 06 Dec 2022 02:17:38 GMT  
		Size: 9.2 MB (9196899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbaac64d951183e4d1471ee19eeb170556b928f547c45a65c32e7c20445e6bc`  
		Last Modified: Tue, 06 Dec 2022 02:17:38 GMT  
		Size: 11.6 MB (11560888 bytes)  
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
$ docker pull buildpack-deps@sha256:25c291637498d71d9032e363183fc0f32a5924c683eac412cf1ac0d33dc5caa5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68579597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17309b002a4c0d69e77f76d6431aea17d6de39f73bd8d5da94994dfa8033c274`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:23 GMT
ADD file:9c101517ec1598b49e898a5a60ee79d12ae039f3da76a37f4b9ecc5211ece070 in / 
# Tue, 06 Dec 2022 01:43:30 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:377056d01f15b8c008b4b2d5e74aef86cd1b3c25771df79e7a3d4592cbbee6d3`  
		Last Modified: Tue, 06 Dec 2022 01:49:02 GMT  
		Size: 48.7 MB (48699631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592ad70c75e8b0ca75e558f3a54c3713a77da7920e04007e9375d34fc22d8ab7`  
		Last Modified: Tue, 06 Dec 2022 02:20:36 GMT  
		Size: 8.7 MB (8653107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee9f87d81b16e0ab87064ce67465efa2eb9ba18cfc708c866166dc66456f13`  
		Last Modified: Tue, 06 Dec 2022 02:20:36 GMT  
		Size: 11.2 MB (11226859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
