## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:a590ddff46a58a462abeb4c8d37ca4fcb4d0d2925cdbef377d1b09601e9fa644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0fc5aaca490caf0a79503055fbc391b8853d761d5a03215be8be60f41e47e8aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120140967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e413a2b1e4e2663e043d48670e90c2884b194881af04864d37af34f210e6ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1c44d4c649674b9e3e229b526b0a8c64d775b37ca77c49712dab1a29b053322c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109768660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a258170ac7140810e8320dd1407b51e91999966c0044a20c68c66fe1ea0b5f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:35:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0469c30b40a2c26072c228ab2795c38de425870b9ee85d29a32a2f50db3c4f`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 7.1 MB (7145345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5315d494a34df967f8f4db548d0b40754c70678b9357188c65dc0b9cfee4f7e`  
		Last Modified: Wed, 05 Oct 2022 00:55:03 GMT  
		Size: 9.3 MB (9344666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e83f2e93982c08cca0dc1dc3456b7bdfa7cdc43011e894195ad828de7550c`  
		Last Modified: Wed, 05 Oct 2022 00:55:25 GMT  
		Size: 47.4 MB (47363676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9f6e569fb46b186c92f83439bc018e32747d464f7d9b2d8807c7416ef1b64a75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119136130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609ea79261cd59e82ef55f8c7c01da32dcad5b2ba53f83090793c43285265b76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:72528f8ffef6e01ca828a63747681ae454b493b4005d786376fa35f432a95d55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122804720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b4069d89bb74ef0eca45c2e785bf7ba4d17172c93d68cd25f65cbd17f76d46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:16:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee1fc3722feabf994120ab8f7d4abab754206d1ca425b7274ce1db428f7a651`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 8.0 MB (8025806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019db6202a77d9f3c2e49a64c766b8b67d4290e0e66e1480fd8c576078914b2`  
		Last Modified: Tue, 25 Oct 2022 05:28:54 GMT  
		Size: 10.1 MB (10128021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afff7d2fb8bbf10afd83b8f08278ed493a12e50a8262a18a1b3fc227667ec4`  
		Last Modified: Tue, 25 Oct 2022 05:29:13 GMT  
		Size: 53.4 MB (53442950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
