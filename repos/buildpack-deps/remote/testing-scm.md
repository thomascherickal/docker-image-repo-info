## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:86d05e25b85c5462c3da2da049e69eac35c169939e10cc0dc3ba58dfff402b19
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
$ docker pull buildpack-deps@sha256:a6bf132e694a90e42d8ee72c8e575bdec9546b215d9edc9712df301273a8302e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121924122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d8e72148d1fbeba83470fab0d4082ee811ca7927df4496673aa05967b7ab8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:41:41 GMT
ADD file:08a45295cc01bc25ae6c0bee004d66cebbd39b1063d32645343bea01d625c89b in / 
# Tue, 13 Sep 2022 03:41:41 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:28:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:29:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 07:29:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe4907198754eba3e4eb94a429c1d51a16b13e54532966f7e63095561ccc26e`  
		Last Modified: Tue, 13 Sep 2022 03:48:21 GMT  
		Size: 49.9 MB (49856149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420b0f20e1d35af12f3b13f66466ccec491acd8d5c853b2d7331caa002fb0125`  
		Last Modified: Tue, 13 Sep 2022 07:42:25 GMT  
		Size: 8.4 MB (8398145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0295625fc185d3c6591c7521c564281b97938cdb7817a5ae7b697913362ba95d`  
		Last Modified: Tue, 13 Sep 2022 07:42:25 GMT  
		Size: 10.7 MB (10657869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6940b5d6436d3113432c89a2db04bb405f6a7cae9aed3fbf3cfb8e86884f693`  
		Last Modified: Tue, 13 Sep 2022 07:42:52 GMT  
		Size: 53.0 MB (53011959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5e3d2fb310cd869f939e6e3e338bc1beb8f4bf815aca372ea02f74ac9e274948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130847214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413c921456d7315b2f0c9bcb38a3cc9776c91ee9faa56ee990571e8e7db0ab53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:16 GMT
ADD file:eeca8a92b00b852cd39f0abd34d39f9d03f4559200a531fc30b095517809ccae in / 
# Tue, 13 Sep 2022 02:10:18 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:59:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:59:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:00:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe69ceee3eeb1b19bdce7ce202b8955dd4b3a0d59f4585e141d537a96e025cca`  
		Last Modified: Tue, 13 Sep 2022 02:15:09 GMT  
		Size: 53.4 MB (53445867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ed3abbadeabe42e467532bcafb9ad0fb312c6dccece83b3e2ff8343432133`  
		Last Modified: Tue, 13 Sep 2022 05:08:46 GMT  
		Size: 9.1 MB (9129907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81a15d4669e4683135ddc0a6911fb0c15c76d889aff660d85d3a412360b555d`  
		Last Modified: Tue, 13 Sep 2022 05:08:46 GMT  
		Size: 11.1 MB (11139231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f008c65966ee18456e65669028da042a442b77aedab02e65670ff717e319e62b`  
		Last Modified: Tue, 13 Sep 2022 05:09:06 GMT  
		Size: 57.1 MB (57132209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3bcf7ca0ae2995d1ff61c4eb71f884da390aa7de7a7532b13e5b4f2674712661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134084280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:debca53c28246a5576117107b090b589ae39307018f6e5cc076514e79e51d959`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:02 GMT
ADD file:017ab146b2bdfc1a02848a9c381369cfc30fdf39ab4fe2050ddecd000ae22219 in / 
# Tue, 13 Sep 2022 01:39:03 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:46:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 04:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4789d73ea79dddf7755bc7b1a512d5c038ace080bd9396a1ad89a757d1273fc`  
		Last Modified: Tue, 13 Sep 2022 01:44:11 GMT  
		Size: 54.3 MB (54341895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589fa07f5181d9bb6862b768db886dc41de845bdf26acc03a8e336471d90af10`  
		Last Modified: Tue, 13 Sep 2022 04:55:57 GMT  
		Size: 9.5 MB (9470035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0fdcf500442071f4c4377f7962edbf18a092afbbfd1a99b1dff583a9b1d32c`  
		Last Modified: Tue, 13 Sep 2022 04:55:57 GMT  
		Size: 11.6 MB (11577399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c918566c81a3c66d99097dc59988895b0174d4d0a9ca49531a124abb1758b8f3`  
		Last Modified: Tue, 13 Sep 2022 04:56:16 GMT  
		Size: 58.7 MB (58694951 bytes)  
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
$ docker pull buildpack-deps@sha256:4388cb7d2975da7f14f52aba83ab7b94510316b03ba2fa57438568f079109229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141497947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd6469f57a72f01dabfb0eb08465ff8b5c7585e715d259850bd6f5a751e50ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:06:57 GMT
ADD file:953c3e24c2166fd8c69fa244bfdab95a8235a25af714160bc89f208a156d37a4 in / 
# Tue, 13 Sep 2022 02:06:59 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:09:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:09:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7c4a0b69d3e0c34047cf77031a6316bf181afd76639e65cfc6f654271ea6f10`  
		Last Modified: Tue, 13 Sep 2022 02:12:09 GMT  
		Size: 57.5 MB (57545876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9081d6899be61711c2e7f05f971158a99d2676a4b17f6942b1849533b6b35d84`  
		Last Modified: Tue, 13 Sep 2022 05:23:10 GMT  
		Size: 9.9 MB (9884781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4922896dd184bdb8d8bee44fb92422394a7bcf8242c2597f07517d01f08eae6`  
		Last Modified: Tue, 13 Sep 2022 05:23:10 GMT  
		Size: 12.1 MB (12149473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1be9db6160aeeb6176c78ff5a69bfdb313ffb29a797480c041d3c97dd0a13`  
		Last Modified: Tue, 13 Sep 2022 05:23:39 GMT  
		Size: 61.9 MB (61917817 bytes)  
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
