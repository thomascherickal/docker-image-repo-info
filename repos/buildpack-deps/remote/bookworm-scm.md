## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:78eea2168c96c76387f60dad047ed4e094585dc56e967ac984363723997dbbae
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0101ec54c1af286e34d1bae192ee392409c02fe1d85b1adea275b453a7e7be43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127897878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8568dbd8b7443ecb0dc1f248fbcf0f0e0abb363990dc932a5d9f486a604532d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:23 GMT
ADD file:7d616c027c138495879d0578d333124a7a41f161d38339949eae9fc46a97bafc in / 
# Tue, 15 Nov 2022 04:04:23 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:21:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:21:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 10:21:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e44dba964a0f1646d06ab7f617603ef51c645dd641b4ce74411770449b003f3`  
		Last Modified: Tue, 15 Nov 2022 04:07:53 GMT  
		Size: 50.3 MB (50297005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65df78b7eb3f0a3cb19c3e7e1eee5c5f93e45ff73ff9fa0a57ea8d5bbf289837`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 9.0 MB (9017903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df801fdaea384702a5d171a41a11d9e52f28f2ef21d2c34c289602d6933bfc14`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 11.4 MB (11372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8830a043c9df19400a0998e5ffbc747e2ec2c6839411650f62fa97df03bab938`  
		Last Modified: Tue, 15 Nov 2022 10:30:50 GMT  
		Size: 57.2 MB (57210022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:79ba49fdff89658bc634a23986e1ab9b110161365b07da586b51e6821667febb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123725485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651e64b63c1ed99939727ef75a475df40f1f5e0e275a1d7f8698ccdecfca7c4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:48:32 GMT
ADD file:f5954c36a3601d3dcf67f8701fe7691c7a94bc36e88827c06ff7338a52d56c5f in / 
# Tue, 15 Nov 2022 01:48:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:39:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 05:39:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34757784ba8ccecfd4a2f549aff99cd98b7b291a61176def51827463bc77aa00`  
		Last Modified: Tue, 15 Nov 2022 01:53:14 GMT  
		Size: 49.3 MB (49265841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55f2cf20315f11c0568b2c8e64fa08c08d44cd3c2ed5e281caebe13320c93c`  
		Last Modified: Tue, 15 Nov 2022 05:47:05 GMT  
		Size: 8.5 MB (8471441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889ed4552e2f48445b3ae801a3f6bf662eac23614471014335840669c23ecf4`  
		Last Modified: Tue, 15 Nov 2022 05:47:06 GMT  
		Size: 11.0 MB (11025735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdcd3cad57bb08b27e14dae1282646677672ad58c572057c39db8a0145596cb`  
		Last Modified: Tue, 15 Nov 2022 05:47:27 GMT  
		Size: 55.0 MB (54962468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f1b2d751b14bfb50ab620f606982e91635699a9b2a4b19cbf8fbf19fbb5d6076
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118825922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdfd20c6b8cf024a0aa3d9760d5174a7b0aa43123845a9425a1f6683ac9c3f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:42:37 GMT
ADD file:7196c14a33cd1774b746a830598de6b6368174bf15faa83c36c244a6e27938fc in / 
# Tue, 15 Nov 2022 03:42:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:15:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:15:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 12:16:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:192a2a7ee5b2cd81557e51320bddd5cf2b318283cd7f7c0c0998525448fcf94a`  
		Last Modified: Tue, 15 Nov 2022 03:49:02 GMT  
		Size: 47.1 MB (47088370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf2f82dd6bc5c9f45ea459022b7744bc671cdbbf0e4a75b81f8f7806c95bec9`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 8.1 MB (8119764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a83154b6af543fb7c117afa8a800dcc4616a91acfe5de9000b91948e1dbd258`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 10.7 MB (10650100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9b01aff410cffd1e3702451f2b73f686cb7a9e4b7bd73491ff9630bb896eed`  
		Last Modified: Tue, 15 Nov 2022 12:27:39 GMT  
		Size: 53.0 MB (52967688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3eb912a1065df2981edb99051872d2296d6144b13dcb470f012baa87c96c6d98
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127615018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af57e892af23744fff44dccc82c38aa4cea19f6293d28b68ae46f61c978f5346`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:50 GMT
ADD file:de3ed89259c63b45a553c11db2206a6ca4201bfd264f04890af2c672736c15b4 in / 
# Tue, 06 Dec 2022 01:39:50 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:02:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:03:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d78ccc24e38e1c539440b7f90d65e136bba8366864c2b4a45e3956272709049`  
		Last Modified: Tue, 06 Dec 2022 01:43:02 GMT  
		Size: 50.3 MB (50307715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb26845d7157ae0fdc105d1666dd413b3f1236876c9e38fe497d4b566c5b8a0`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 8.9 MB (8851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee48d89e1a98c15d782346793fdaba61be0e798358172b68670681463bdd69f`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 11.3 MB (11325483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2882696f0c89ced811afa19b67056d882fbab71ccb7f7e31631ccdc1d1349d0`  
		Last Modified: Tue, 06 Dec 2022 02:11:13 GMT  
		Size: 57.1 MB (57130706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:47907807283ca26435ad4b3ae878332554fcca9ec9429713b54bac9730d2cf2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130744403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e54168a3c6d3359d7791522c4e690fb2e254bc901a1c445d21f76848b7de5b1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:38:43 GMT
ADD file:6064ead20e3d5415784fcb74157c3ba1b90982f542deb132e9dabb2a1712e396 in / 
# Tue, 06 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:05:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:05:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:05:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45070d389a5ecd4dae6cdcb3e06567c8481416cfb2efb085e318fb5e2d11393b`  
		Last Modified: Tue, 06 Dec 2022 01:44:36 GMT  
		Size: 51.3 MB (51301574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe8313be6a60f2abeebcfad5a2e4539e7d4b28618e0b019908926dd39c9c1bd`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 9.2 MB (9196657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4a90125b538cbb0d87c8c0d37737cdc01ed561a27c8ecfae4cc4f708aecc3`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 11.6 MB (11560721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4c1fe8d1b528c380407ded013fe72d397a8e0cc5e05d87cde0f468224efdfd`  
		Last Modified: Tue, 06 Dec 2022 02:14:30 GMT  
		Size: 58.7 MB (58685451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1a9c32deb64cfc3aa38e350c476bae25204ea0ebcf00c2ae22c40188810c165a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125912449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5529eefc951d396b1f096210cebef37e8025185cd3b4f22c0f0cd146b5f8f1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:11:59 GMT
ADD file:0d439a2fdede63b0646f17fe0578b4ebab24012a35c93e6e63e5c511ccce8fe7 in / 
# Tue, 15 Nov 2022 04:12:04 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:02:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:03:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 02:05:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52449a481885eb7aca2b2fbb088c8d233a6249a8aaaf65e32f8c268ad8340850`  
		Last Modified: Tue, 15 Nov 2022 04:19:19 GMT  
		Size: 50.3 MB (50314192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d29bbc0f4e1684560d462982ab292feb495140fdd75d13e6826460b19d90c0`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 8.4 MB (8383819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232356f6f3990a119f67b1a72642482a16966341b02a7f077b08d38e1d12852a`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 11.1 MB (11132477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705e4f6a2f0ed68bc3f782b429fc0c3d447a4f512e41434fa2668233d6417a9f`  
		Last Modified: Wed, 16 Nov 2022 02:28:20 GMT  
		Size: 56.1 MB (56081961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b6a1045246424b49a4f9124487b5776ddd5d09e6f241cfb06c77ed5cdfb7884c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138149971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53a46a877837736eb8e5932153b27e1df4ffa6620c3e2a318747bbf002a0554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 05:17:43 GMT
ADD file:b13da8e7ee4f9b71f42de64cf2dfe92a09d9d6be3537a8b151db32013e632fb4 in / 
# Tue, 15 Nov 2022 05:17:45 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:51:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 11:53:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24f3e6cef4f753f77f6e0b5b4e73cf7a7fdbfa85b11f29916d1d4fe28bee544c`  
		Last Modified: Tue, 15 Nov 2022 05:22:58 GMT  
		Size: 54.4 MB (54360800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e462c1bdfc268a97c6033242cd34635559a926155991efd84c30d93ce39ce6ee`  
		Last Modified: Tue, 15 Nov 2022 12:06:33 GMT  
		Size: 9.6 MB (9596802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970a93fcc7e991ae16e04be69f70dc91326e712c64e700b5ee5a6a3f14bb797f`  
		Last Modified: Tue, 15 Nov 2022 12:06:34 GMT  
		Size: 12.1 MB (12129037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32858cde7d5ae6256db15870fd4843b2b1d1b45a97333630926091c571385bc5`  
		Last Modified: Tue, 15 Nov 2022 12:07:02 GMT  
		Size: 62.1 MB (62063332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:435edd6684979fd14d47ca81cf6f1b95ea55c8529b4af451ec3ed814db6c1cb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124933533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d9b60c3d183ffc35f6413960a6f108663916e24f5a3368ceedcf37f2b0c4633`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:45 GMT
ADD file:45186e2067a128e8dbf3558a97cd5853548faaf7c2bb93ef1544ed66907fcf19 in / 
# Tue, 06 Dec 2022 01:41:55 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:06:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:effa21bde36181862f20d53853fc03e36421f6a13d6aad41051d593fe9c7c097`  
		Last Modified: Tue, 06 Dec 2022 01:47:58 GMT  
		Size: 48.7 MB (48664905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f5dcd56007991a3866c8b0bf2ee7220f18a57fb48ff74112e6c810f63c8b96`  
		Last Modified: Tue, 06 Dec 2022 02:18:52 GMT  
		Size: 8.7 MB (8652754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1216521a137ae490612192a50d936077fcb94da6292a8ef16485599b92a5ace`  
		Last Modified: Tue, 06 Dec 2022 02:18:51 GMT  
		Size: 11.2 MB (11226716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49291721bb021828aa82c6d2c7e2c9cc22d7fe71b2f0406cef91b807704ecbea`  
		Last Modified: Tue, 06 Dec 2022 02:19:06 GMT  
		Size: 56.4 MB (56389158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
