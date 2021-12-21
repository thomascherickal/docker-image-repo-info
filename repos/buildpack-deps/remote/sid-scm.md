## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:ad7b7944d747c8b9d48f2346d19fc84efa5e94b18efab40eecb3bcfeabf0f148
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:113f37df301ac3654f57906a732dac2907f2f4967f7d564578a03bed515e0438
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128697003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc357b4462639081858f52417d922dabcf25d6610916747fc72b03fb3da7575c`
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
# Tue, 21 Dec 2021 01:55:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2f1da4768c8ef0bf34a53ed37a7a7581bb0aa27f68e2047d84c74fbd9e6bd604`  
		Last Modified: Tue, 21 Dec 2021 02:04:12 GMT  
		Size: 56.7 MB (56718041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1783730181df97e59f6d8c14c4276b564fa279a7cb98e0e5021369e5b757d2c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123402292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7829c469a1887981bb88d9005cdec6b84bccabaf5e6dc2e698490175ca7aa080`
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
# Thu, 02 Dec 2021 03:48:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ced16911b039c1097a2b138cf1e729c67a19c941b575a03dee7c08a1c42d3e6f`  
		Last Modified: Thu, 02 Dec 2021 04:05:17 GMT  
		Size: 54.4 MB (54384666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:503309f2088e071dc6e55fe3dcccb818c5409a06396d9a1b27e5cf40f6ac7a91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118395575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b1a9d4f39bd3aa441ab5035d64758f0d14f2cb21e097708974c7431baca348`
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
# Thu, 02 Dec 2021 11:46:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:80273a3f397b2e47f3a65064b16f0b619eb3a2129a44b15d1f347c8ef553ea1f`  
		Last Modified: Thu, 02 Dec 2021 12:06:43 GMT  
		Size: 52.2 MB (52247072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7c273dc7de4dce59b5f8ed00982cfc63f668bd2650e1547c4057332ece415f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c84209633428054b32d1092ea786c9601b1ad02e80d7a9bac0747c1f885ec50`
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
# Tue, 21 Dec 2021 02:15:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:9ffa7de7b15c6883e577b019809e1343d6f6d9c4e790ce8ea84b0c42300324d0`  
		Last Modified: Tue, 21 Dec 2021 02:25:19 GMT  
		Size: 56.8 MB (56755865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ea5f96a7f8642240fe331691f522f13bab0a908479b739f6e6bb6c71e2539537
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131664208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1257c6b5f9744bbfb62d2635144198d35cef81b181fcdbf2f0f73cf3e254a1`
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
# Tue, 21 Dec 2021 02:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:edec29419a6219e77259f3179317cfa40969486314c93fb7616fdede0a463d5c`  
		Last Modified: Tue, 21 Dec 2021 02:29:21 GMT  
		Size: 58.1 MB (58133925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:550260958aaef481861f912e39f70f7fdd1c1e7024e058fae634214c71f755ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126152857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8612d7fdc52c7272cddbb0a536022d9e70fb09534335f4fabc83d266172e49`
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
# Thu, 02 Dec 2021 04:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f11f0ae65985544fc4af9dfed32cf43717ac87519a70907b32399aa3b9bdc13c`  
		Last Modified: Thu, 02 Dec 2021 04:32:35 GMT  
		Size: 55.6 MB (55554324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ce119a9ed018af6e2bbed0bfa383e0551dabd07b11666cd30af0ba0933b6f6c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138632547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b52653939a4f57e58d6c3936e632decc51270b79a642a6f46866e106822725`
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
# Thu, 02 Dec 2021 12:42:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:990ba6858763a274b899da9a34d5f84598bd4e6dd076b319a268ef7fd61d7416`  
		Last Modified: Thu, 02 Dec 2021 12:58:06 GMT  
		Size: 61.4 MB (61393717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8963a3d61e4c3d8f556c008a03bedcef239cb984ed5d4cfe38da92e01d9a5ecc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119734335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e04c96d11a2d683bfeff1e5e487338b2d884f84026a93a03bdae943cdb8907`
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
# Thu, 02 Dec 2021 04:03:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:7b46552026ea3fee87ea1959d63905f5dc028cccb4ee43e623210e771c78f3cf`  
		Last Modified: Thu, 02 Dec 2021 04:39:19 GMT  
		Size: 52.8 MB (52817111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dcbe9f0dfaae59dab269d61bc7aac9b220b8a11ecf87e7d68363616bf33a5275
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126239873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fc06ff58e120b7c90b2b3c3223a6dd61273bd918e5ee96c3f702159fb331957`
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
# Tue, 21 Dec 2021 02:12:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8554ce38b98712645df3c9898c381e1ac40835d50f37d436f4f4ad142ee4a654`  
		Last Modified: Tue, 21 Dec 2021 02:19:27 GMT  
		Size: 56.1 MB (56095731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
