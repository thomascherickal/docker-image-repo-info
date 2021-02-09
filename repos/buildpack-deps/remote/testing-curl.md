## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:3d4953a5699e149a11f8ece06e14cdee47a605be5e52b20aafc15ba4f505cec4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edffa5e69b63146783401791226d5b16bff77d7bbfc637468be8f65011f9c2b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70544360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e094078a6d97373e1eb022f2e2035764ce13343885f5eac893ae7416101f8262`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:09 GMT
ADD file:695398a9e249223d1e07b12d735ae1a0ce3d645d0fd4cf1478400a985311f1cc in / 
# Tue, 09 Feb 2021 02:20:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e6f7b6573b5973ff98ec7b4368f16ac39a85fa4fa49a414c58d0a9a012d37354`  
		Last Modified: Tue, 09 Feb 2021 02:25:52 GMT  
		Size: 54.8 MB (54757786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e06a77fb30b0ab01ed40c4454b51ebc1989110fd455036a95486c37328845d`  
		Last Modified: Tue, 09 Feb 2021 04:44:39 GMT  
		Size: 5.1 MB (5143859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423fe70e1db2a70eb1116ca8f81653348710538e8027421da14d99331de5cc9b`  
		Last Modified: Tue, 09 Feb 2021 04:44:39 GMT  
		Size: 10.6 MB (10642715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ef4a78e0edd7dc58af8c0f6af9ed32782517017e87e1d22600d1bb39457d09bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67664516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328bbeac69bf98bf2f18faf052686d3d9dc2e101ce0ad3c5ccd08b33c5e0de6c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:49:05 GMT
ADD file:e692f14c1c4483cbc88d3f2b2b98df48a5589bdf417d84c2dd9dbb7388ad079b in / 
# Tue, 09 Feb 2021 02:49:07 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:da2c3be8f08cfd7ddd509966bb4655b1f7c74b4eaa31a7ab733c50e91684f29c`  
		Last Modified: Tue, 09 Feb 2021 02:58:02 GMT  
		Size: 52.3 MB (52282753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9638f6c6794cf8abb357179d6515914ce152a277d089f8baec5e2553acf260`  
		Last Modified: Tue, 09 Feb 2021 03:38:28 GMT  
		Size: 5.1 MB (5054036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9f24461ae5121b4bee6d238f5d67ac3f026a1264614cf4428418453a0cfb5a`  
		Last Modified: Tue, 09 Feb 2021 03:38:30 GMT  
		Size: 10.3 MB (10327727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9cbf49e6d0c62179c0502344f0569bdd03d61076de3132e360cbfb3187a89655
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64819326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b41df4237ed4716d161f9956e5ce224d35e3606d080b409567ca10234e0be9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:59:45 GMT
ADD file:dbec72322674e09aeb852498a932b1b1be67734644d9efa41f70930b49e956ea in / 
# Tue, 09 Feb 2021 02:59:48 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:22:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ffa24fa47fc6ecfac0851b7ffbee3dc36b7d721e5a4d08285c3577bfe04c31a1`  
		Last Modified: Tue, 09 Feb 2021 03:08:35 GMT  
		Size: 49.9 MB (49936256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95997d63d97278978549401c96f2fa498f1420591bf0a8fc3bace484b2250bb2`  
		Last Modified: Tue, 09 Feb 2021 04:38:08 GMT  
		Size: 4.9 MB (4914496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001ea97578ff6bb0c099fa0742f2ed56527bfbc1c389ff125d63e64a5aa83f`  
		Last Modified: Tue, 09 Feb 2021 04:38:09 GMT  
		Size: 10.0 MB (9968574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0837027406ed0a481ab13cf9f9c33c3f9ab441d373779dfc0ad6917b73190511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69208474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f95c309e308f725be72b2d83d8710931cfb2a36d2ad5675cb240ffd8e3cbef29`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:06 GMT
ADD file:33be07279470bfff8a3572cfc0847b56f8230b343043052761953a9c6a60acf0 in / 
# Tue, 09 Feb 2021 02:40:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:40:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:40:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4a012a5760f92ca41c31246ef8e4d918873156a81f765b0a7c5d840e0f5704b6`  
		Last Modified: Tue, 09 Feb 2021 02:46:23 GMT  
		Size: 53.4 MB (53428538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79d28ddd44a525843a64c4a38bd53e21517f7cea2429e5566c98fe63eca0100`  
		Last Modified: Tue, 09 Feb 2021 04:55:58 GMT  
		Size: 5.1 MB (5132214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b66026d3757ddaa2f953691aee45d95fad0e392e5f27c9030a7a327ff1972`  
		Last Modified: Tue, 09 Feb 2021 04:55:59 GMT  
		Size: 10.6 MB (10647722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:64ca29eb24941f11f069f64cfc3cdf81c29feb55cdbca38f56898ef361c8a67a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72033157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0eeb003ce09741c74158df693152c523161c63494edc334b1e43adb3974d1c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:01 GMT
ADD file:f81099d47b3f99bd08895e4a96fb89eec618d9d0e6c9c8b2fb34681259f340d5 in / 
# Tue, 09 Feb 2021 02:39:02 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:07:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e734eb27dd94c1f3c88a6f32899a659ba2861df7282687c7b9c90f8df744b794`  
		Last Modified: Tue, 09 Feb 2021 02:44:51 GMT  
		Size: 55.7 MB (55737065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e825922dd50d020f9bf23f62b411455511e3368cce25b3304525c231209ec605`  
		Last Modified: Tue, 09 Feb 2021 03:18:46 GMT  
		Size: 5.3 MB (5271393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c92fbb51c2a913e1648e9cfa5323f95e95123462fef6d2370963c8b8c23052`  
		Last Modified: Tue, 09 Feb 2021 03:18:47 GMT  
		Size: 11.0 MB (11024699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1400f722c1634f52dcf05ff5ac1f6d3eb6f4d62589133e799fdf9c1bc090c9be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68763233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f7076bc22cf986185f97021bcac8a45afbbb2379a4a1aa1d226eb7372828cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:08:17 GMT
ADD file:7f68924af238bc101419c6fcd9a321aa3ff88b6234d508100e66c9234756eafa in / 
# Tue, 09 Feb 2021 03:08:18 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:00:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:00:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4cf1c8f9242008a01fc5567967aa7bfb87bd9f5dfbbd4f4b296fc463a02ee18f`  
		Last Modified: Tue, 09 Feb 2021 03:13:48 GMT  
		Size: 53.0 MB (53004321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaa6f5a332631981e084265abaccebb0a60c433eb0544f48b4c9a36acd40c1`  
		Last Modified: Tue, 09 Feb 2021 04:13:19 GMT  
		Size: 5.1 MB (5107186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a371ec00a3dddda57cd21f3bf82cdceb3fcb8f04ef78924a1357172ec6fd0dc`  
		Last Modified: Tue, 09 Feb 2021 04:13:22 GMT  
		Size: 10.7 MB (10651726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:395e3354a94259806ac798908af6dc02791e1f6eb0f555f0f36e2608ead4cff2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77415262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e53a0af5f4fa4668472028f5f823c4da07c357e467f66dbe2cbaa4a04a20fb5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:23:03 GMT
ADD file:840490bff9a0b2cb1e20599d893c1160f6884327f51294479567e5d43f91b885 in / 
# Tue, 12 Jan 2021 00:23:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:39:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9d21ce86f5496c36ba2ba289acb977a3b160c6c56fb257c10e3adb8b55164a16`  
		Last Modified: Tue, 12 Jan 2021 00:32:24 GMT  
		Size: 57.6 MB (57562164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42b61558772eb59064c0ebad8029e0e7524bf865c29218b048871cd3e43fe7`  
		Last Modified: Tue, 12 Jan 2021 02:37:14 GMT  
		Size: 8.4 MB (8431230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663cfe2e2cfc28477e509f0e7aaffd4159d2f37157b32a7327bb6f43a7508ac4`  
		Last Modified: Tue, 12 Jan 2021 02:37:17 GMT  
		Size: 11.4 MB (11421868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:29a8549158e40c78622e677b7b2ce4fec56c5632ac5cc3c51a53c87f3d9fe406
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68652909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27504c4808fe1e16b056765946aef4a6cc628eac23bf38aed8228df2fff735e1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:32 GMT
ADD file:b29f05e744766860cbed836c9527b8ec4e72570959bb61a8aa0e5c363cb72484 in / 
# Tue, 09 Feb 2021 02:41:35 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:03:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:03:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6eee01c120872bf1700180eee1b04681a66f946d188f352a1a7d516d703e4a66`  
		Last Modified: Tue, 09 Feb 2021 02:44:42 GMT  
		Size: 53.0 MB (53006960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d2f6f124d0127ebcdbee7e40a00127640a914d79503aaef238ab4afe12cf36`  
		Last Modified: Tue, 09 Feb 2021 03:10:53 GMT  
		Size: 5.1 MB (5127719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3216ed6227ef8df582c34143415b588c1ed64bb3ed322108f9c67d4318a5e6b2`  
		Last Modified: Tue, 09 Feb 2021 03:10:54 GMT  
		Size: 10.5 MB (10518230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
