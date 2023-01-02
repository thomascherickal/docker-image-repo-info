## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:b418d48d6ecffbb7f8a746a9d443e2f46653b3aa3d4dedbcfed481f655f0685f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:537a203490e6436af51f38d65a697e6be7a373cae0d72777340c630efc58b40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81864419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab9f8894c5e5bfd8bdfdd53b91e385c9be0b1d0a3db00eaaac3ebc25a8927a4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:53:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Dec 2022 03:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae2fe226e32be2bdda7461072a27e452330d588e627c7410d3e0c4df49ebb7`  
		Last Modified: Fri, 09 Dec 2022 04:07:48 GMT  
		Size: 6.6 MB (6617788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d279765cf084ae227e518a350e7c71778a38e42ebb7040fbde05048ba430b66`  
		Last Modified: Fri, 09 Dec 2022 04:07:47 GMT  
		Size: 3.0 MB (3026158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4fca8757762a9887ee7058668ceb80ab0ceb2e86e0843f27d7e25f4a161512`  
		Last Modified: Fri, 09 Dec 2022 04:08:03 GMT  
		Size: 45.5 MB (45509014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ad75fcc4a0f8065eb8c22c33a64a663921fb6b730cce355b24d6dade1fabfbcd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71270980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86295192c240152e01b0669ad5d8507ae79648a6fbbbdf9d1de96d1cf36dfa75`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:33:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Dec 2022 02:34:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999222233ef373db15e3b18cfbd5729ea9165f86b03b197c2b9653d10ad60cb`  
		Last Modified: Fri, 09 Dec 2022 02:53:39 GMT  
		Size: 5.7 MB (5680158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbada3f9c5cad5c160f7d50062ce28dbb088541f9145ee0ded5d455697032f20`  
		Last Modified: Fri, 09 Dec 2022 02:53:38 GMT  
		Size: 2.6 MB (2585946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf6f3661c5451c4c063868ed002e72ce892a8adfec34b523ad6a4d2b01d6916`  
		Last Modified: Fri, 09 Dec 2022 02:53:58 GMT  
		Size: 40.7 MB (40699669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:595b7540788d41e7b4c7076e52f152d840e71da5c37147e0b44d772e03781848
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75891388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a54942c57a17de76b99dc5450ae4641cdd151d583fcd2d5c4a88753d50947f8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:26:21 GMT
ADD file:0acff7d2bb94db4847afdf5ab7b4385732c0a38fd82b0057ce0459f2b5d04042 in / 
# Mon, 02 Jan 2023 18:26:21 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:47:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:47:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 02 Jan 2023 18:47:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c347df5277017bf1ab15f258630e012d44bb79c509675d9464f96570668efab0`  
		Last Modified: Mon, 02 Jan 2023 18:27:02 GMT  
		Size: 23.7 MB (23735210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57589a61e75b6fd9c40b958bcd242697d3bd9c18d4e46b2ab119920727081ae`  
		Last Modified: Mon, 02 Jan 2023 18:57:37 GMT  
		Size: 6.1 MB (6054448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fe4f939a742980b846ab4256c36fd2e683a0409f5c4655aced05555c4bf9ee`  
		Last Modified: Mon, 02 Jan 2023 18:57:37 GMT  
		Size: 2.8 MB (2790412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846d548556b4af418a2bea61c5b5aaa5f28e8fab62286fa92db02592dc6d346b`  
		Last Modified: Mon, 02 Jan 2023 18:57:50 GMT  
		Size: 43.3 MB (43311318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:20ca6f0a35d8bd9c60e0233850977fdd3e65888c3688a84670eb4f3826c22a6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84193455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17d0b1d2c98bb24c0ff9c18db59b3e5b08473d290abe9fe6fee7c08fc7c5c7a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:00:42 GMT
ADD file:dc76519390168deb6f9bb6052d08c6e7840908a831276d99bb19c6c245f8517b in / 
# Mon, 02 Jan 2023 18:00:43 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:22:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:23:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 02 Jan 2023 18:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1b284dbae22f155bfee2a25073c97c9758e66aa7129a455cb533d8e2cbc873f9`  
		Last Modified: Mon, 02 Jan 2023 18:01:17 GMT  
		Size: 27.2 MB (27165399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd588f5ab18433db51d33fb54b32dbf18f5af8fb4dbd30b3407f93e99ff057a9`  
		Last Modified: Mon, 02 Jan 2023 18:28:46 GMT  
		Size: 6.9 MB (6902109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf514bf8c4c2f919659a2f58d292672576181c783d997d3caa71f5818bb613`  
		Last Modified: Mon, 02 Jan 2023 18:28:45 GMT  
		Size: 3.0 MB (3042082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a83431373780b1960b3bc18251eb91b21ae542545bc96ec68e5b0f5a6aca46`  
		Last Modified: Mon, 02 Jan 2023 18:29:03 GMT  
		Size: 47.1 MB (47083865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8d0f407d20de376ffce102d38eba931594c36d65e27e2920ff5da4619d260674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94957821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2e46be44aeb7b0dc1eb993dee72f1d367ca8ed6dff60837ba5054a528af4d2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:15 GMT
ADD file:05ec256cb279f6d94111b2413d31c85c4e1ff1365bce34d2fc4aa2788885fa06 in / 
# Fri, 09 Dec 2022 01:27:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:20:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:20:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Dec 2022 03:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29d5a8bf9800ea1d873fe104fc2b0b6d4efed1269ce0f9a80e4d65e96d3246e2`  
		Last Modified: Fri, 09 Dec 2022 01:29:45 GMT  
		Size: 30.4 MB (30442475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385b911dcd17dcd21857c45f1580921dc1ef7a6bfbe01898fef3a628772fa8dc`  
		Last Modified: Fri, 09 Dec 2022 03:50:15 GMT  
		Size: 7.0 MB (7036031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e182844a761cb72bff2c8199230ea0379f9a69184d085e6a53f7c24e9f815c`  
		Last Modified: Fri, 09 Dec 2022 03:50:14 GMT  
		Size: 3.7 MB (3740619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fc42bfb15dd85b269039f92806177e1e72f17da34dbbee0f5d01dd6d5e8d5`  
		Last Modified: Fri, 09 Dec 2022 03:50:41 GMT  
		Size: 53.7 MB (53738696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c6d8334db26c8ecc68ee0e5e5ff520431d2e9f582b647911476a011ba9079f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79701144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:702f8b625c1c13cbe925d505d9e901588dcd16ae7130cbcd71491632780a07e7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:52:21 GMT
ADD file:c2fcdae7883d865c232dfc26d514c111189f6940ba74273c78067624cd02c962 in / 
# Fri, 09 Dec 2022 01:52:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:35:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:36:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Dec 2022 03:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3fb013d46f2fda49d6c671f39f55c3330f927a4c55ae7e5096daf0a638dc38ec`  
		Last Modified: Fri, 09 Dec 2022 01:54:45 GMT  
		Size: 25.4 MB (25371298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d3308c646e5c998e89d5d8adcbf8cd509d32cca837db45b2d5c82b50e285a7`  
		Last Modified: Fri, 09 Dec 2022 03:54:11 GMT  
		Size: 6.3 MB (6308863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abb84decd56d62b11ef05936ef3afa942b0ac06afa5119cbb7104d11e4f6934`  
		Last Modified: Fri, 09 Dec 2022 03:54:11 GMT  
		Size: 3.0 MB (2976730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca50a5cd722b7d90ffdf0658e6250d7ef874451be114b087c7c41f5854a2193f`  
		Last Modified: Fri, 09 Dec 2022 03:54:25 GMT  
		Size: 45.0 MB (45044253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
