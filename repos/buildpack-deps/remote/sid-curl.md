## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:1295a8df722d58dadc69830726b740852f57f05d3d56e2ae874e6bf66951608c
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
$ docker pull buildpack-deps@sha256:3cfa993030b52daf43693f58d86f736c278c8006a98cd4905ecd6b57f9724fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72002001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59b642e6983819d8705b9d653eadb5064f959d152236963fad4a8e9b810346c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:58 GMT
ADD file:69369feb027cb9fcd22f8a4b51431458f4e51eca8bb0c398edde4cc47c3d74e0 in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:48c02bc8c594d3500557aad8d76d43fb3cd9632de373f64648f0523fd33f3197`  
		Last Modified: Wed, 26 Jan 2022 01:49:14 GMT  
		Size: 55.8 MB (55811672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05b5335d4dea27f0ba29bd1ce5c5b9d3b0ab8f87964be3312ecadc0f34e96`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 5.3 MB (5274876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dacb71892995084387b6a8a0a9ac7eae9ee1b597031f8e25ee46a18d91140f6`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 10.9 MB (10915453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2291bb994819fb70d76f692a5ff2496d0e9b8d8455e677cee5d8988ab210436a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69013656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0eb84f2bb26185744faf0604f34dc40993b35cea34a640472ee7e0798c1a58`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:b2ee7e73ad4207feb437f92888b1a73e57515c82fc8325c4604d21a39771e52f in / 
# Wed, 26 Jan 2022 01:45:21 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:39:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:39:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:248f9d803d87b1b0a005a24c98133b989ced8e0b664be38cb600b683c4593899`  
		Last Modified: Wed, 26 Jan 2022 02:02:42 GMT  
		Size: 53.3 MB (53255788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc4178c3c07ea158cad18d885ec03af227796d71c4a004c8f15b307cc4de474`  
		Last Modified: Wed, 26 Jan 2022 03:01:01 GMT  
		Size: 5.2 MB (5174902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0983cc859431bb8e8296bbc443587cef8bf5f35a9b346102ec3018f68c610`  
		Last Modified: Wed, 26 Jan 2022 03:01:03 GMT  
		Size: 10.6 MB (10582966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c27e54623d1ceaf876b344efaf32c0e1d11af7acd73de4bc1b11d502faa2d74d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66174637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e815eee1044a1c832ed17ec74d46afdb88b3c4b452c76d6345d40921ff3cc68`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:42 GMT
ADD file:25bd7c90ec9cba9155b5f5e4b8ba10eee0a84413efe182bfd8e270eec1783ca2 in / 
# Wed, 26 Jan 2022 01:45:43 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:45:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8beb160c955a6211ac47cc7f90ad3b37999d7da6c9b2f0d32e82d6ac9bb4e6a3`  
		Last Modified: Wed, 26 Jan 2022 02:02:50 GMT  
		Size: 50.9 MB (50897789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5033ef8051fa00849de7e1029124d977fce14e2255ef3ea2e9a0aa226e20a793`  
		Last Modified: Wed, 26 Jan 2022 17:09:44 GMT  
		Size: 5.0 MB (5035338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2221dacf46091a2f23a799af18530570a3c4d219f9d87d052eb48e5982c95d9`  
		Last Modified: Wed, 26 Jan 2022 17:09:46 GMT  
		Size: 10.2 MB (10241510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9474eac30331a00765795d70f73fbaaf0c3ceb81fb1a3a50134d17d4f7cfd536
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70716713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fbf124c34229cecdc4111e9875cf8ced630c47e19ceadb8b5ccf8032ca9861`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:52 GMT
ADD file:b374f2870285b974edf3ed21e9bcab7b86f3d5f58f504052e4ef7507affd730e in / 
# Wed, 26 Jan 2022 01:43:54 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c162c40f334c8be5b3a873f3af9fdbb3e46d36b02232496f08adc78fd0d1197`  
		Last Modified: Wed, 26 Jan 2022 01:51:38 GMT  
		Size: 54.8 MB (54776771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5527738d1213690712a506bdfb6a4e4e53f00abc3a857f27e46783342a012`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 5.3 MB (5263075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb344bcecb1f1e4eb7e0b7d7ceb695b290ff4e82c3967bc1c646a8c98de6d21`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 10.7 MB (10676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:59b414bf8ec2e34ae396a90db93d18a7814b17066160e5539b4eb3470f806e45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73567661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d47cabcd75412e84dfe9962bfd264512d108f80665e8483c10c390d304711`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:da0be8aacf1ce5f6b8eac72cc37cf866a1f42436b73a7491a048fc296e2aec59 in / 
# Wed, 26 Jan 2022 01:41:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:19:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:19:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9befaf96f69d02ac54d26fdd6569c9b6bb607e4566ebcdba828f8df0ed688997`  
		Last Modified: Wed, 26 Jan 2022 01:52:27 GMT  
		Size: 56.9 MB (56852445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1205a9ac4da466a85715ecf930f05eece9a89e5b6f512222898eefe087f5697`  
		Last Modified: Wed, 26 Jan 2022 02:31:45 GMT  
		Size: 5.4 MB (5407567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59261fa94d22670274f83195f55b41969e923771145bb95d95eee75fd629f932`  
		Last Modified: Wed, 26 Jan 2022 02:31:46 GMT  
		Size: 11.3 MB (11307649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c1ac39f70af83e4195419409a22ebc4844cb8bb34a6e787d3e8098e17c833f4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70594033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959514de54c0a0f8aebd17c7910762ae51dff70eae90ec14ef983405880599b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:58 GMT
ADD file:ff5cb17f112000b0283048e51a31c66fa6d3b7b5c73ebbb9e407d66773bd71dd in / 
# Wed, 26 Jan 2022 01:44:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:30:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:780a90a74dc946c86fcaf8ad99094385c527418934e8729eb8e19bd129202058`  
		Last Modified: Wed, 26 Jan 2022 01:54:46 GMT  
		Size: 54.5 MB (54487249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28747c788a9fd6c864f18d440188468cf9eadd01d3170b173b0dcabaffd1dc0c`  
		Last Modified: Wed, 26 Jan 2022 02:44:18 GMT  
		Size: 5.2 MB (5231642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e77450002c767308f9f932c83fde37fdf6742b761b14caad928f47ea3c8735f`  
		Last Modified: Wed, 26 Jan 2022 02:44:21 GMT  
		Size: 10.9 MB (10875142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a29dbeb76b087143d00dab6d056bcb902b9b014ee11d2577bfac2027e7309446
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77431058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6a7dcad2485aadf3a29ddf8c28458ef0f507050ad59bbeaa99c7c53c7e135c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:50 GMT
ADD file:00619ac2b9b09af1ef0989fac7a97e811d92f85cef55887a843850c6edd6397d in / 
# Wed, 26 Jan 2022 01:48:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:59:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:207334870a9e08012db59a768343c68c9297e1123cfd3f49c878d325443196c9`  
		Last Modified: Wed, 26 Jan 2022 02:01:42 GMT  
		Size: 60.2 MB (60197594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44ef395f05a799994decb77ffb1782c89a4c0282be793f404418d1a7f1d81a`  
		Last Modified: Wed, 26 Jan 2022 03:25:17 GMT  
		Size: 5.5 MB (5540064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f233b52a0118c53ec4e4fcbf2d80e0f1a054746b47ff133ba2e3c92eb1246992`  
		Last Modified: Wed, 26 Jan 2022 03:25:16 GMT  
		Size: 11.7 MB (11693400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5aaa3a274ab894b0e6b0107f0c834d8ad96ca0a7a52cd78d8633c39ec9e695b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66935242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfa2b401e1a5d1cc43c83166f0556dcbf070f14693faa5bf1600b9342ec43d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:38 GMT
ADD file:a60c98877072aff885ac29b30770d767360f732a9ca188e3b7832a90fd81e724 in / 
# Wed, 26 Jan 2022 01:47:41 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:31:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cdc7b3e2f290f0098d8226cf770b0357385cf234ac7fa2076ac921525985e05c`  
		Last Modified: Wed, 26 Jan 2022 02:03:53 GMT  
		Size: 51.5 MB (51527715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db22b43c730abfb99368b4808036748143ac4a5666da043b17aa922d81cf8c25`  
		Last Modified: Wed, 26 Jan 2022 03:05:51 GMT  
		Size: 5.1 MB (5089854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8880ef8492c671ac8a4ad50074157fd88c5e5e566f686156dd6ef6918591bde`  
		Last Modified: Wed, 26 Jan 2022 03:05:54 GMT  
		Size: 10.3 MB (10317673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:475f15bcd9985ede793720e1d07b5e958cec3647b86d2c1e9b49c89167cd3077
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70152207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b6a90ee0e25551e062bedddb3693ecbcf929f3faed83224140ea2ccf166437`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:22 GMT
ADD file:3bad388a0bccdbe60c35b9f2f185f24531da6894d5fbaaef83c17aaaf447084d in / 
# Wed, 26 Jan 2022 01:42:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:018136a50defba2fd8fcf9a0ff234cc3971c8e2e29eaaea1a3db05b950df25a2`  
		Last Modified: Wed, 26 Jan 2022 01:48:18 GMT  
		Size: 54.1 MB (54089891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b646642536852c2c78a0d07f56fe415018ecf441c1ff4bb1f3672347e0a16d0`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 5.3 MB (5254889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716bdea6cf2de7b0ea754b38c3e71201e96482b618ecfe5cdd22d50c44f2853`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 10.8 MB (10807427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
