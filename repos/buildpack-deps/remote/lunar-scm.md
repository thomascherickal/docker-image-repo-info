## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:cb5732379b56dd0b340123beb192890e474b438b7510696cbd2e797a5df0db19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:56146ea5d6b392e4dce8f44766d9251703f013af7254faf0f7b6c1e4149ea451
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80520720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ff34c476bcbe14e850955115eeec13acdeefb549018982b8a476d19302e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:50 GMT
ADD file:3a69ab43af761d2eea701ad591edccb2b1f84ff63a25059ad9d5bc53358dedc1 in / 
# Fri, 09 Dec 2022 01:20:50 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 19:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 19:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Dec 2022 19:27:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a13f57ee816c77bd77798d728a3d73246552cac763e9c613b26aecd8441e43e6`  
		Last Modified: Fri, 09 Dec 2022 01:22:25 GMT  
		Size: 27.5 MB (27505626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb206e2c65ae53b38b00dbe71e2c1e6bb7b54b88640624201c2b86a1f5847b8`  
		Last Modified: Thu, 22 Dec 2022 19:32:28 GMT  
		Size: 6.8 MB (6780053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d01a823ce10ce5db3cb9c09adcc98b1c550a3ffa8adab1c26c5ae3eda5c0e65`  
		Last Modified: Thu, 22 Dec 2022 19:32:28 GMT  
		Size: 3.7 MB (3657390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c43da0c86244888b0b84f7c0a7f0e0c892e4926cf101cce101bfd3af10574`  
		Last Modified: Thu, 22 Dec 2022 19:32:44 GMT  
		Size: 42.6 MB (42577651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0d5bd2ddfff7137145b367adc7275d6c45c4eacdb47e6eeb38185240ca9c180e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acf0f212fb086eaad8b87a6bc8374a610fa413867f48348083ac585e3b0cf64`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:59 GMT
ADD file:c32587e56b8bc2fc7216d4ae1555fbd250b1d9fe75287cc1695ef58d8473c990 in / 
# Fri, 09 Dec 2022 01:37:00 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 20:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 20:27:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Dec 2022 20:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a0077c0ef8989650a1fb4f37effd0a1fad1055621ccc056d7282a1831abf9a8`  
		Last Modified: Fri, 09 Dec 2022 01:39:37 GMT  
		Size: 26.0 MB (26028162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c164931ea1da2a0de524578266acb327c17a70e0d87f42535da4e05d4993a6`  
		Last Modified: Thu, 22 Dec 2022 20:35:44 GMT  
		Size: 5.9 MB (5949770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c1b49a8f9a05a169d8201bbead60565ec21f42041d81ed336ee1f858ae7521`  
		Last Modified: Thu, 22 Dec 2022 20:35:43 GMT  
		Size: 3.8 MB (3819824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b3d9c178b3a2b07116594452dbe60b04ff8358ccb42a8c1305da86b69af83c`  
		Last Modified: Thu, 22 Dec 2022 20:36:03 GMT  
		Size: 45.2 MB (45196874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:688987046263a0dc1facebbabc06e97ca4cb1e84a415dab25be7ebdc2bc3f7dd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77327688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41f816ac8483c35d193209b99e116910a22e0a32691b30fc2354ecffcb16d9f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:26:30 GMT
ADD file:87f1515364340e1c65eb76041a8285f4f511485c46275949dfcff1961d556236 in / 
# Mon, 02 Jan 2023 18:26:31 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:51:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:51:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 02 Jan 2023 18:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03a7a9a433574ecc00c891140ebadd82c8592d8f29b7d5808b6bb9a0234684b5`  
		Last Modified: Mon, 02 Jan 2023 18:27:21 GMT  
		Size: 26.9 MB (26855540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e6d0788fd51c380a42af1846c598400304ca8803209292d56b2a8630aa89d4`  
		Last Modified: Mon, 02 Jan 2023 18:58:28 GMT  
		Size: 6.6 MB (6607822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bccdee025930916817db2cefd4732712b388478bb27ef225f2967af645d3754`  
		Last Modified: Mon, 02 Jan 2023 18:58:28 GMT  
		Size: 3.9 MB (3857692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd231be0b6fcf816a7cf5925909097faa87172e6b776e9c3f5ab19f1aae8753`  
		Last Modified: Mon, 02 Jan 2023 18:58:41 GMT  
		Size: 40.0 MB (40006634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2f6d20352cf371b2502c7f4ae2c3b722b90817c0d58c46faf884372bb585af47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91456138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d08ce0187f7b9840e3ce3c7c186062b71cfd0abad0238fb1d061e6105ff6024d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:28:29 GMT
ADD file:fc908ee01c16840b84760d5041e467ede6748c61754d04faa691f9fb6ddf1686 in / 
# Fri, 09 Dec 2022 01:28:31 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 19:40:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 19:41:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Dec 2022 19:42:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08a75ad1a4a23cbc8eccc791fdfae97d71a324379cb275562275520611a56654`  
		Last Modified: Fri, 09 Dec 2022 01:31:25 GMT  
		Size: 32.1 MB (32104472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c870358a362895034ccb4359831dc39366f11c4609b717d9c3a44e0282b11b`  
		Last Modified: Thu, 22 Dec 2022 19:49:56 GMT  
		Size: 7.8 MB (7754835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0d292dfd312b20bb9ad0a639938aaa822a0e0a09f07b775ef818d1c3483fd4`  
		Last Modified: Thu, 22 Dec 2022 19:49:55 GMT  
		Size: 4.4 MB (4378575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7296a8f280368b3eaf64dc4cc52332f529dc23a9622eef822ef0bf1ac366c8b8`  
		Last Modified: Thu, 22 Dec 2022 19:50:20 GMT  
		Size: 47.2 MB (47218256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:e47f456250688f4bef8b5cc0558319ac3021bd6a5283dbedd6bcd19ea8556050
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79076811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b9a57c039c22e55b673448e753d372a13ca831dedca3d3a55bddb818349f3b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:09:01 GMT
ADD file:512505c2df26db88aeeb5025ff073a2d8e98d995422df61a5cad94d79ef22a42 in / 
# Mon, 02 Jan 2023 18:09:02 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:29:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:30:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 02 Jan 2023 18:32:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ada5e428c090bd736690979612e7bece7c31ff1f1701ca35de4d1899e835e69a`  
		Last Modified: Mon, 02 Jan 2023 18:09:56 GMT  
		Size: 25.7 MB (25669058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e756f227648e5a559b1f2387229c92d1fd4b83589d63631f0d177d76e2c6e34`  
		Last Modified: Mon, 02 Jan 2023 18:38:32 GMT  
		Size: 5.9 MB (5925890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb3fe222b3eac428f3f8b9fff7621e4aa631ace7d402b5590058b150e5b19b2`  
		Last Modified: Mon, 02 Jan 2023 18:38:28 GMT  
		Size: 4.1 MB (4141220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c4e43f4e9b3918249951c171418c34a155f22ed75ce4f308406d3e0f1de10e`  
		Last Modified: Mon, 02 Jan 2023 18:39:36 GMT  
		Size: 43.3 MB (43340643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2ad0df7ab017197cc643330fcfc73b3047421d48095106d668df0207cb3b1db6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78564212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7ffd5ce3b608d19caf11e78aa4b6fe52b044ed4ec021111e86071706d2b43`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:53:35 GMT
ADD file:34ba36266e3f51a04f8105b97312cec6ad0e02db549c1a40af7b2b9b8b4527fb in / 
# Fri, 09 Dec 2022 01:53:39 GMT
CMD ["bash"]
# Thu, 22 Dec 2022 19:53:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 19:53:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Dec 2022 19:53:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:40f085afd82295659f70518a511d2ea24258833fac78ee993694322605814e97`  
		Last Modified: Fri, 09 Dec 2022 01:55:38 GMT  
		Size: 26.1 MB (26064347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ff57ac87df71f9147afd569d5c780b3c46584d3ae2a7ca33d038e5b2603c3`  
		Last Modified: Thu, 22 Dec 2022 19:59:01 GMT  
		Size: 6.5 MB (6463110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dcb825ede09e4c615483b46aaf77e56e707f1a2e30ae7027eaf43484859483`  
		Last Modified: Thu, 22 Dec 2022 19:59:00 GMT  
		Size: 3.6 MB (3643218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f27c39d9c3fda7daacd85705c51fab24e164f5ee1e884b24c4afce7b770dc1`  
		Last Modified: Thu, 22 Dec 2022 19:59:13 GMT  
		Size: 42.4 MB (42393537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
