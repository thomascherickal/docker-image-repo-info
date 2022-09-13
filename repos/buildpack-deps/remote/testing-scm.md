## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:f1cd1c32ccfe10ced662071f711856a66d0e4f689905090930da7f1cc86e313d
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4066edbf6125dfd88f932e6de036107d3085343b924724c3ab8e798db091ca11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130873305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5921fc15ce9f46023b341216f64c67ef49cc4f12eb055b292e454327fd18afc9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:55:59 GMT
ADD file:3b3b943815afcac58f0e8a49af9b3ab289e32cdd69d4c6bb0c64665439c8619d in / 
# Tue, 13 Sep 2022 00:56:00 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:41:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:41:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:41:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97357bf36a88b062ffcf42d1d32358484d7f104afddf68a27fc780d5e4b35747`  
		Last Modified: Tue, 13 Sep 2022 00:59:24 GMT  
		Size: 53.0 MB (52983612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e85309d383df743b3da5b66b25c79bfd21de0eb43cac2ce0387409d833805`  
		Last Modified: Tue, 13 Sep 2022 03:48:52 GMT  
		Size: 9.3 MB (9295960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30754f9ad0f0e351d103e87943c636152b4e9d25a1db67e55bc77549647c36a`  
		Last Modified: Tue, 13 Sep 2022 03:48:52 GMT  
		Size: 11.4 MB (11379997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6c5b5ca6be88eed184a522fe2afbf51c23d1c68d147ed39b8ef3722d14b137`  
		Last Modified: Tue, 13 Sep 2022 03:49:11 GMT  
		Size: 57.2 MB (57213736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c82f1476eea82d2ecb8961416a811ecf4a61033ec6bfff0188fe28441ddc01e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126810502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ff8a52dde78aa5e6b7138f4b5fbaad35927f740732a78ab27e90277b551be4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:52:16 GMT
ADD file:fafc9bc142e136ee85605d8e97e30de6b77737818f595795657169b6296c2106 in / 
# Tue, 13 Sep 2022 00:52:16 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:21:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ac1aef77561a09b4a507bdfee90352851c4c589691168642e1962feeb17f470`  
		Last Modified: Tue, 13 Sep 2022 00:59:23 GMT  
		Size: 52.1 MB (52122539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56ddb0666c981767a214d7185034ecf5482eb3d4b80f732c8fd7c7af5cafbcd`  
		Last Modified: Tue, 13 Sep 2022 01:29:49 GMT  
		Size: 8.7 MB (8737254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7deb621c649cab11725cc4b3fc53034474e4320d371490f9e76fc97011296`  
		Last Modified: Tue, 13 Sep 2022 01:29:50 GMT  
		Size: 11.0 MB (11027333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4053bbd05f00bbedc4e093305a19c088463e15043657d86095dd7e78bd51b7b7`  
		Last Modified: Tue, 13 Sep 2022 01:30:21 GMT  
		Size: 54.9 MB (54923376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c50fdc3cc8971109d7e2fb62ae7f6e0654628f84a110f1113a842ee045e776ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121871444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3aaa5ae4912b2de292b9affa365fa17be839dbd9222323714858cc9d901bb30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 12:57:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 12:58:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a9319f004c20513b7f62d6d76d1b1959183b5ad5b488373ca6330a9d6797b`  
		Last Modified: Tue, 23 Aug 2022 13:09:50 GMT  
		Size: 8.4 MB (8402996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd63a2d6ab83a6d913419cd2a446fc94d0d9a4c654bf2a3c13dfe3a7116609`  
		Last Modified: Tue, 23 Aug 2022 13:09:49 GMT  
		Size: 10.6 MB (10589855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7d7ae465211d33c40484e48402566e419669463cab573010f1ab877df64a9`  
		Last Modified: Tue, 23 Aug 2022 13:10:16 GMT  
		Size: 53.3 MB (53323503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0155117db9306b41c236e921e5f76a0bd743851a0ef03fdd0375580ad644862f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130809998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5866f5d0d44278637ed443b0e5d5a0e8b808d2c70c50503fc468ffa7d2bf8b13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6e04486d701fe9f175abed959a5794adb184ded2d14ea520fda84aa445ba9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134148274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8346a4ca2444870e8bb65aff75d4d4cf6711229035f48bacd81de5aee6ec3ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f7817c9b6896e6e7beee09544e2b7726ce7ec83ec9446acd09427432a1a8edb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129262005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62602e152d0e490e4fe366e84430653941bfd900e0b1273d513c4d78932bfa77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:09:11 GMT
ADD file:3491a858e0f5d7985f9d29ad3567a39b0271d5794db146892787053625c3b44c in / 
# Tue, 13 Sep 2022 01:09:16 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:40:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:41:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:42:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b94700b51ec501e09ccd1e3b3962175f6110497a6ce43a01932cb0ca2718f356`  
		Last Modified: Tue, 13 Sep 2022 01:16:48 GMT  
		Size: 53.4 MB (53424305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc07918d1372f974586c63d6aecbeb7a19896ffcd4f48df4b090b4bb8ec36db9`  
		Last Modified: Tue, 13 Sep 2022 02:02:34 GMT  
		Size: 8.7 MB (8657983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623176abb726f5305a72b42bb4719f479242a849cee500abc5f6ce16b8f94697`  
		Last Modified: Tue, 13 Sep 2022 02:02:34 GMT  
		Size: 11.1 MB (11132895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a36d3a5288753ed417f0ab1efc651492f197a193aa9da65851bf4ee43c90c9`  
		Last Modified: Tue, 13 Sep 2022 02:03:24 GMT  
		Size: 56.0 MB (56046822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1ae72a86df0538f6c86e6177acda8b42ac2b5bc5b16f91d75bd6dff1d570c92c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141681548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e0dbaf8822ad89bf60827cb4b2f3927b1784af8cc2d1ff24f2e790d144376`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:15ece40adec41760dc41f7b3a006f8fe667b14dceb6d5f019801f95963aa5901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128455503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341fc23d036447e43c60634236bc8a266dfbfa6eedbb788ad16f069017db8c4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:47:18 GMT
ADD file:b7771dfd52d59914f02d6a960a15a002d38a4ce20bcf17ccc9e77d105dcc970f in / 
# Tue, 13 Sep 2022 00:47:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:23:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:23:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:23:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7aeb98a659275cb80ecf5c5010e17e1f9dbaeb66dc78b0b9547e7d2cef3ccbed`  
		Last Modified: Tue, 13 Sep 2022 00:51:49 GMT  
		Size: 51.8 MB (51793736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adaff81aad91f6a031b48c69591bd51c2d468d34936668cd86f38080d3798b7`  
		Last Modified: Tue, 13 Sep 2022 01:31:55 GMT  
		Size: 8.9 MB (8936273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bbf0d6341f90012fa26f17d05a3be32e377b717d69c402ff59b71d51d1585c`  
		Last Modified: Tue, 13 Sep 2022 01:31:55 GMT  
		Size: 11.2 MB (11237961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658ae34cf46fd9815e4fbb13d05a19b8ac18cf3aa6086b98784978217912fe58`  
		Last Modified: Tue, 13 Sep 2022 01:32:10 GMT  
		Size: 56.5 MB (56487533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
