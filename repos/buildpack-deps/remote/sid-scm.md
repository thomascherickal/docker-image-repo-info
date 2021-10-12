## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:4b8446a2f0c784de3396060f05231010a57f3d4d40e0604754d6c078630cf610
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
$ docker pull buildpack-deps@sha256:1f58ee2f9e6dcb549b7374b98a57f288bc6da93df3c7649f986dc05e046851c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127539357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493d09e443c411ea990d16617b8da4ef2865199ec8f29b3809b64960cdbd653a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:58 GMT
ADD file:2d684471f088173801ff86eaf94c1d858b74220b84642d73b02bd1bfe0d54b60 in / 
# Tue, 12 Oct 2021 01:21:58 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:46:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba87283d9c312600aafb7f4149986884d524aae42e0701a90d2fc23c85e977b1`  
		Last Modified: Tue, 12 Oct 2021 01:28:21 GMT  
		Size: 55.7 MB (55687470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcf62d5f60a89ffe69fdffb6f89c02e782fc35bf8d5766b9e4d46ebc82278a`  
		Last Modified: Tue, 12 Oct 2021 15:55:24 GMT  
		Size: 5.2 MB (5216552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669cb549c6380d94ce53b7413b60cfab218aebd91bdcfc6c970d908b333925a8`  
		Last Modified: Tue, 12 Oct 2021 15:55:25 GMT  
		Size: 10.9 MB (10900892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4cbc1206c2266ee34ccdeb1d5e8209dbeeff0f65a52a3af81a6c46546f37a0`  
		Last Modified: Tue, 12 Oct 2021 15:55:44 GMT  
		Size: 55.7 MB (55734443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a6fd6b6ff59a9e3a097d8125f6ca8b78882f804f0ca5bec557784676e4d379a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122358029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4f3e109e84ef325b2927539c9c569367e50198086ed8d72be40ef36742c34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c32603c083c8a17da7aab259972f866d5279ac3a296865f8b90a45b84a15a84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.4 MB (117409473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c26da540809364463bbeee54c11bb1ea3c207e47777d11973e86ecc00f6d770`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:32:13 GMT
ADD file:defbc06b1cc21db01a673f118d34d129435486fcb83814c5c987ff566c61360a in / 
# Tue, 12 Oct 2021 01:32:14 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 18:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:153dc8e6452cda134a8143d2ac887e7ebfa01c8568115d6b3172ca0008ef4838`  
		Last Modified: Tue, 12 Oct 2021 01:49:06 GMT  
		Size: 50.8 MB (50797066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bc8cfd03a1c715f9702494a8f0c4599bf04e51f4a7094befc758068725b5db`  
		Last Modified: Tue, 12 Oct 2021 19:02:43 GMT  
		Size: 5.0 MB (4984307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7905528e1493cb4119aa69a5a20f43d64dc225128ef6308ed4a2ea77a1684b7d`  
		Last Modified: Tue, 12 Oct 2021 19:02:45 GMT  
		Size: 10.2 MB (10249876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87677333086e2dfb5a81ca8e8c60b5923e629e363255c0419e6b467f805c4500`  
		Last Modified: Tue, 12 Oct 2021 19:03:18 GMT  
		Size: 51.4 MB (51378224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fbedc924372aeb77e98ef62e7fe4d264c1b4a4ffbaf9a07016430ed37c687b03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126689544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8607b15a9deffcdad451b776ae5c607bdd5e316477f47252daa9586f9a5f8ad6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:36 GMT
ADD file:830671e1709a0164ca60ad1012d3d0202e7e63c74bdbec7df54f308a4d4c8b11 in / 
# Tue, 12 Oct 2021 01:42:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:13:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ed37bc205e0aad196bfd6ba235a1a5fba10e02175afd192c816df6457d06c75`  
		Last Modified: Tue, 12 Oct 2021 01:50:51 GMT  
		Size: 54.7 MB (54702895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e12eb84409ba3f2dbf96f9e720e1db75055189af4f9c412b3be39768c371b5`  
		Last Modified: Tue, 12 Oct 2021 02:21:19 GMT  
		Size: 5.2 MB (5205920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39f86ea1fa7d211d3c24d9f11b0ad622d344241f5f4288b575d09a0e038e903`  
		Last Modified: Tue, 12 Oct 2021 02:21:19 GMT  
		Size: 10.9 MB (10899227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82855758df584636866eabeef61f652a1b64eb39037aa2155d68f7d9cfb5dae4`  
		Last Modified: Tue, 12 Oct 2021 02:21:40 GMT  
		Size: 55.9 MB (55881502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:733772bac49de30e8a05b0ad0e7d0340e5b5089313a4dfdb7f57a6d60552b79c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130503569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41174274a4fa2d6806ed55fabbfd91e97b22e8a8178e2412b0e819bceda895d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89ffe14200fdc5ef8d32d228027ec8f1cb4f4e336dc2f12e03c9542883696b94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124925003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8df2d03f5cb58b6b7196f8d8fc1afcdfd3bb588a4c45471bcb87e4b697d146c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:13:27 GMT
ADD file:27e1d46380432bbd287bef3c049b6707a409fa2f49f07e76f4826c6ee57cfca9 in / 
# Tue, 12 Oct 2021 01:13:28 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:58:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 01:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7afe2e09744237d99a12c5f86f33ba55800e5acee482662abac2c64c64a7824`  
		Last Modified: Tue, 12 Oct 2021 01:23:41 GMT  
		Size: 54.3 MB (54313468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8be3dfdc1ee7ccf4465ff4d91c782f9ad2d795bd9ea4965953382190a5626`  
		Last Modified: Tue, 12 Oct 2021 02:11:44 GMT  
		Size: 5.2 MB (5177464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f028726b389731d6d9e30d4ef26719ac3a44889d1bd0681ebbf11f085178373`  
		Last Modified: Tue, 12 Oct 2021 02:11:46 GMT  
		Size: 10.9 MB (10904218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2076aaf953f38208fdacaa4098bb05224c1ede12a74b5ecee28db74cfd04ac8`  
		Last Modified: Tue, 12 Oct 2021 02:12:36 GMT  
		Size: 54.5 MB (54529853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9cb107173cfcf70286b43387a62f73d446f950ebf1d6ec736c213caee43c6b07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137168656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ed13442782d0723cce8315405a10fa6890398277e8cfcef4bfff32c2833bec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:27:58 GMT
ADD file:975422ef5390ff94fc050a84a9840e39188158f1c74f7b6dfde93829787b7c8d in / 
# Tue, 12 Oct 2021 01:28:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:23:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3794e49fdef56187e1a7ffe8a3c0d0dda8a5b5c159e370831000df5e5f638479`  
		Last Modified: Tue, 12 Oct 2021 01:41:02 GMT  
		Size: 59.9 MB (59889168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3a771c64c6b854d6abde14ad239e8808ef66674301b6a066df68b719b9ef04`  
		Last Modified: Tue, 12 Oct 2021 04:44:22 GMT  
		Size: 5.5 MB (5468996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a4272fe59063922ad53af8014c08c537807fbc8a6fe125f51be34de8ffc53`  
		Last Modified: Tue, 12 Oct 2021 04:44:23 GMT  
		Size: 11.7 MB (11654490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97493787213daeca4485b87abed722776481493a73f647e2d70fc24c1d0efd7`  
		Last Modified: Tue, 12 Oct 2021 04:44:45 GMT  
		Size: 60.2 MB (60156002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f2acf63005fc73f02b0678a999e3e31dfbca393a9f818188f14615ede9992c47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118653548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1fc669a261b25e84dd46cfc237297d211aaf249adf92ee1123c9fdbbf2f545`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:14:22 GMT
ADD file:bd71d5680d1006cf090b0a295547cb405dc17469df91f3492267dbd5019f25c5 in / 
# Tue, 12 Oct 2021 01:14:25 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:57:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:01:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f088a81a8bb9ab030ef8f6d37a5e280f5ad79eaf2817310f6498ffe43ca2dac`  
		Last Modified: Tue, 12 Oct 2021 01:30:29 GMT  
		Size: 51.5 MB (51516608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3fde059905204e836dc3ffbe360b638f58c8c7dc954c038d591b1859643368`  
		Last Modified: Tue, 12 Oct 2021 02:34:36 GMT  
		Size: 5.0 MB (5032271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ba22ae6fbd86a3c7aed8e1c6ec2a2f1af7f4893efe5133d85c145066a77f8`  
		Last Modified: Tue, 12 Oct 2021 02:34:39 GMT  
		Size: 10.3 MB (10314713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173a27bd17e1f1571ed8f4073a4e420529a44ded0e627650b24d0a2cefa08d6f`  
		Last Modified: Tue, 12 Oct 2021 02:36:46 GMT  
		Size: 51.8 MB (51789956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:64115d1ef31465828e213f146ba1fa866d09ef5db130af77b05f936b718c2bb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125099980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb198261c1112c322a936ae8533c1922e9ac09b7a98672bacabdc866a7746785`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:43:35 GMT
ADD file:d0d1a83115052a10810bdba27eb855359796f604b655de31492b0699abf1d546 in / 
# Tue, 12 Oct 2021 00:43:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:43:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 07:43:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:979a8d8677c5949943057dfc51bfa612e3d365d71df4150210296bec00f04cf2`  
		Last Modified: Tue, 12 Oct 2021 00:49:29 GMT  
		Size: 53.9 MB (53940740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b2ee0930fe303c9ea2baf728cca61c84ba351c6472da4fd5385e62530f6673`  
		Last Modified: Tue, 12 Oct 2021 07:50:03 GMT  
		Size: 5.2 MB (5199342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92727346c90e0492705828b0c21131c81b3b275773725847689d7cb0a15efa57`  
		Last Modified: Tue, 12 Oct 2021 07:50:03 GMT  
		Size: 10.8 MB (10793861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe0ed031f749a2507ced21f398da3825f07398298d2a33454410b1e09d37b82`  
		Last Modified: Tue, 12 Oct 2021 07:50:19 GMT  
		Size: 55.2 MB (55166037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
