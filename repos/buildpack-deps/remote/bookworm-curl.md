## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:cd30bc2c9773e6ac6033833ca41e6a0ff30bcb92e8bef5d1052b72ab483f3da5
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:71403088a0f33dfd835bf14f208a503f61810b8aa73cb25a4d19a670b5bf89f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73659569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a42d8913ff184e1b6a7a87b900712881c87b527af4f73a847188d55c926c31`
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

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8eb76b698e7ff845f128909420a2a659462a9aec49b6436816951316d2e029af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71887126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed8220d697a41def4f4ad11313f1e5d5f384a3a2d3443301b8892c37cb8c6158`
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

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7d1e315b3f0013ef10e0cfd12e74fe08814b7576823531dabafcf8aa9d88928e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68912163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9ec3847e09e18b9082b4e0b16285daef483dfefbe8a4997befdbc6b1a54579`
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

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:38b9356fb0d0d4df55680024f67bb2fd6e44154401752db03283f1f016cdc900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73715005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6d964c5f91de2926306f3451df7d714847efa88ef8deb78b6093f1bff10836`
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

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:67c9850dd73c65da6ca63e243e4fb1eaf212b875059a257d5f8538a7a4d055b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75389329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9279b70eacdd19d1e0bce3fe84d12aa39d1c2af2d5e1ca2e60c1f163ce8e3309`
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

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e5058dddc52ad36c288407f5af719a4dc3aa74924aec66516c30dc751bdfa176
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73215183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5951df76190d6ae0ef0fa7a4d6820b112afae63e962209ec9582838531c05a6c`
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

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:16b8884c6952638e584e248afc40fd2695c060d532ceb4fc0c46c5dd45237393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.6 MB (79580130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e92435cbc761f33548636821dac68869eebeb6c4b9594b131cf7aff29b55ca1`
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

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6229d598713dfed89b90fe6f45e43b144a159e0742c6cd70d5a57284be0a2d40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71967970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995e70e1bd8e6868ba941246cd408c2f10741ec1b632fb631cb9b97393cba5ff`
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
