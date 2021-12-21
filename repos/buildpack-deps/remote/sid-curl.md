## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:124a8ec747d12ef0a57eb90d88872cd0131cde688f8da5e4e9cd355da6267c6c
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9e8c5489263d3a0c33d1ccf0d1aa6cd69849aa552f8b48998b3444623981f2bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71978962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337c9767010b746d2cd95bdd0271a57eda89683bdd979326eadb8efeb5f016a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:53 GMT
ADD file:ce4b0836a3fcb4df3c14bacf996ad27dde10d17f63fbf745c09d6ae62c3e2cc8 in / 
# Tue, 21 Dec 2021 01:23:54 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:54:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c476fbbe1d7eecc32473e300b1659f1eaf7c11eff20d52cd6f7471c94062564`  
		Last Modified: Tue, 21 Dec 2021 01:30:07 GMT  
		Size: 55.8 MB (55798023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c6bd99048b6b72b33b515cda942b7e40ca1d3de2b2f9cdd7bcb90dbb74274c`  
		Last Modified: Tue, 21 Dec 2021 02:03:54 GMT  
		Size: 5.3 MB (5276774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492abb693e033360d88b0b5fc39af18ee3a635345217fb4fa41328e278d7136b`  
		Last Modified: Tue, 21 Dec 2021 02:03:54 GMT  
		Size: 10.9 MB (10904165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6b207aa33eb534d8fffe5e65a5268d4c08d6e58d13376d5e76371c47e151a1c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69017626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43071757ae58c014490249682962a4d7777efa95aaec0ba0a669549165a91c69`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:54:44 GMT
ADD file:358278336204ee1e51bf00f8c88d281c73e7e5d5b537fca1ddea89c9e69da90e in / 
# Thu, 02 Dec 2021 02:54:45 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:47:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:47:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:92d580f40fe8bf02becf360f6a4dc76454bfd66964c4acc0ddcd113fa0e9c2d1`  
		Last Modified: Thu, 02 Dec 2021 03:13:27 GMT  
		Size: 53.2 MB (53226256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638194516b96610900042221009a8c126b7644c26fe612397f2b2622bdfd03ac`  
		Last Modified: Thu, 02 Dec 2021 04:04:39 GMT  
		Size: 5.2 MB (5180320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b2f3d24644f1e0eec33ec3662f820a19dc6b8cfa47e1f1551776f80f739780`  
		Last Modified: Thu, 02 Dec 2021 04:04:41 GMT  
		Size: 10.6 MB (10611050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58d6ebc48938c932553bfa5409364ab35ffbc1967d5e2eb30ce13d259c056b1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66148503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1585f316366beb9dd39ea6881588dedecdd23014e2e6142eb7d694994b10a440`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:08:50 GMT
ADD file:9740c987db5f6d577c2e2575a0974eb1a867a5c79cca1eb79e7c19d112bea4d3 in / 
# Thu, 02 Dec 2021 09:08:51 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:45:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:366f7fef67fd1fee5779f5f26a7bf655fe3e0243c51566b5fc28b209c153a87e`  
		Last Modified: Thu, 02 Dec 2021 09:25:38 GMT  
		Size: 50.9 MB (50857401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63a2c21d88128fa3e4e629036fbd1d1d18eb72a94a41ffddfbc249ba7bfda70`  
		Last Modified: Thu, 02 Dec 2021 12:05:54 GMT  
		Size: 5.0 MB (5037501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c060d5561088295a9205a8a15042f3a66b6758e385cae2e07d3f2f5f58e49`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 10.3 MB (10253601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6031a1d48868123430f79c3b69e7fda462caac3a9389dfff4fca4f52e5b71f7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70718943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f15b4dc686153d9a24fab3d2557710fb2428d1c15c56136539f3c38e1b56fa2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:45 GMT
ADD file:7c4ba9d9936c0139eeef9f235c0d6840aa3c32d40904663e82e285a1b34d3a75 in / 
# Tue, 21 Dec 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff79c5138bd3b6ae9212e3b674731e907981317ed2018a35ca98f456034d18dd`  
		Last Modified: Tue, 21 Dec 2021 01:51:23 GMT  
		Size: 54.8 MB (54780864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04ea6899cdef9e4cb3add824a5c066cfe56407ffa977a94114981f8c9e02493`  
		Last Modified: Tue, 21 Dec 2021 02:24:57 GMT  
		Size: 5.3 MB (5263545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d6eba4116602817637a346f0e2c8ed4adf77ba0f6d395eb6b49df6d42761b6`  
		Last Modified: Tue, 21 Dec 2021 02:24:58 GMT  
		Size: 10.7 MB (10674534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c7ec0bd38ff25ecfe5683611d8c90adda8b08331bdf343e31a697e7254228543
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73530283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523f783917916abbc3c08c9911b21aeb61dc7282e093bdb81fb6bd2184291930`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:07 GMT
ADD file:7c506c9d86a63bd33b2bd42ba9e380551bac76c3ef7352900f2acd644f4c8540 in / 
# Tue, 21 Dec 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:17:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:17:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4134c3f595c8eb15f3af8157a618c36c51d0cf4948eb0bc00ce1697bab8e3d81`  
		Last Modified: Tue, 21 Dec 2021 01:51:54 GMT  
		Size: 56.9 MB (56851682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc39f58d3b3754f23bbc0ceaf7adab7ffcc255c02bf6a043aff6842dd0cd45d`  
		Last Modified: Tue, 21 Dec 2021 02:28:54 GMT  
		Size: 5.4 MB (5408518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6769abd0d85d00c570f55ee96473cec596d53c5a8292473578a15779b5e36e82`  
		Last Modified: Tue, 21 Dec 2021 02:28:54 GMT  
		Size: 11.3 MB (11270083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2ddb6d4de48bfb58a9788724b6c91ad878b576ffdf7ec7578dfdca2347874ee8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70598533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be14f7f4952f62773639e0a5f1e38276c775f4066645b7bd741e5799d1725f2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:11:25 GMT
ADD file:756c847932d446a78e78b1785e3773acc2f468bed861faa53b3a777f03b1273d in / 
# Thu, 02 Dec 2021 03:11:26 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 04:19:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 04:20:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:851a637e7cfa078b1e4bcb2543d21b6bd9e139295986a256dac39682452e1a34`  
		Last Modified: Thu, 02 Dec 2021 03:48:41 GMT  
		Size: 54.5 MB (54455441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ed4124392ca3477be2c7aafcf44d0c7a1c0ac313b6aa4db5e42c0fd0d27038`  
		Last Modified: Thu, 02 Dec 2021 04:31:41 GMT  
		Size: 5.2 MB (5235788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d46352d707f92ef2034e26342ca34e8d34141a50bef2663631e66049929929`  
		Last Modified: Thu, 02 Dec 2021 04:31:45 GMT  
		Size: 10.9 MB (10907304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6bc439b50a6635216b0d7d24a0416ef6ebf72bce3c177de8e157744fac45b976
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77238830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3a814b9414858de639e53830841a6a7be1fc4e57bc380ac884490a7e378e42`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:23:26 GMT
ADD file:0ba5425cea9bcdb1fac898f3ddd38f4505205a5b32c1288a9a4ecece03ec10a1 in / 
# Thu, 02 Dec 2021 07:23:34 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:38:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:39:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b9442172998188c0fffb75559bba82a9436fd970dbf2b25460afc71f86479c20`  
		Last Modified: Thu, 02 Dec 2021 07:33:54 GMT  
		Size: 60.0 MB (60041316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b299250e1b93acaab942bfa0d27e9d3870773ddfc17e10df4fd3d31f96f82`  
		Last Modified: Thu, 02 Dec 2021 12:57:42 GMT  
		Size: 5.5 MB (5538234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3154daa6ac50e0863a376a29692bd68a0e9a4a87862f71434ccc121a401f7b8c`  
		Last Modified: Thu, 02 Dec 2021 12:57:42 GMT  
		Size: 11.7 MB (11659280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b8766ac83de9214e56be0de79150e874f989b94f86710ccd092db997076b0130
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66917224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2dc1dc067727e389dd30fbb51f7bde517f5f47e9f294494346026297a2442d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:16:27 GMT
ADD file:2408c0186c2415b201c5fb609f218da02da0aec9aff7f9467433a1bcbdeb0da9 in / 
# Thu, 02 Dec 2021 03:16:29 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6a1cc4c4003753c168cfc12397594854587c6645c5f03e57779bd85f43632403`  
		Last Modified: Thu, 02 Dec 2021 03:32:36 GMT  
		Size: 51.5 MB (51509234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0400a63f68eccacb4581e73d2e13a149f13d2f96ede6f9a5041b48108f8267a`  
		Last Modified: Thu, 02 Dec 2021 04:37:08 GMT  
		Size: 5.1 MB (5089467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536bb4db4e00844c1bdf6f562fd2fb2840423d4d90c98e791568915c641acf0`  
		Last Modified: Thu, 02 Dec 2021 04:37:11 GMT  
		Size: 10.3 MB (10318523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:235a0b08c7d7a18538bca35809aed769fcfc902e8453a5e9d5ab3376a8f1fa7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70144142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4287ebad93a64b1bd72a9c20e0a98b3aa40aa5b57e28c386f8516bc8b948a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:37 GMT
ADD file:fef3d16fc616585749eed591688807817c9f37f8c4f5b1f6fa331e8abb0b60b4 in / 
# Tue, 21 Dec 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f8ce27066e069d94a5210461101ff67f39042687acc056c6b8f43da616f6b2b6`  
		Last Modified: Tue, 21 Dec 2021 01:49:35 GMT  
		Size: 54.1 MB (54090241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430eb3656cbd2e26f5882863248d1d470bb0f7b5019c000a75107367ebed5950`  
		Last Modified: Tue, 21 Dec 2021 02:19:12 GMT  
		Size: 5.3 MB (5256801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf00a1bce82700c975dc02484e483d113ef14013f902525638bf031c142cae0f`  
		Last Modified: Tue, 21 Dec 2021 02:19:12 GMT  
		Size: 10.8 MB (10797100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
