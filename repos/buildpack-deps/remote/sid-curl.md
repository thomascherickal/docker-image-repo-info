## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:1d1511ec584569503fdfc9a9b15b230a1928240ea5ecf388aebaeaa82ece3104
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b2be4953d60e6ae5785916f0c78c84a989753933aebd4b8ea92b09b6fd95f251
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70937819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5d70e684fb0a1ef0a8f31f474d7a78cf10b05539d35429f8d45aa079eba006b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:22:07 GMT
ADD file:b00402c4b2c5828b18b251f8a057510f9f7da733f833cd147ed1a8fcb8d574db in / 
# Wed, 12 May 2021 01:22:08 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:57:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2746b657344bbd3149c23794266413a61b32b44f53688f3619e485894c87b09`  
		Last Modified: Wed, 12 May 2021 01:28:33 GMT  
		Size: 54.9 MB (54896691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327df9aed8a8e57527a50678726f61121ed7fc1ff1b0c91e4268684ec7631ae7`  
		Last Modified: Wed, 12 May 2021 02:06:06 GMT  
		Size: 5.2 MB (5169357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b16c115b4ba04c02cb68097f3935495074622e8771a76d9f6a8c99d03331f9b`  
		Last Modified: Wed, 12 May 2021 02:06:07 GMT  
		Size: 10.9 MB (10871771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8c2df4c392a862ec6620e51ce2a5b28733fcf5cb1cebfdbf169088e0d3666c86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68084082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877d1e50a4bee2703facd7244c0553973cf4dd97904983fd09b1904a619fa513`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:57:58 GMT
ADD file:74d49eb3680e0d1e7268c77ac09aadc6a9eaca2541a1941d02c05771fce80430 in / 
# Wed, 12 May 2021 00:58:17 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:34:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:992a8499bbce77a1397237914a5f442e2a2d90912c4dcf8d75ced68fa669452a`  
		Last Modified: Wed, 12 May 2021 01:11:33 GMT  
		Size: 52.4 MB (52438763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbeeca774ae665bb974c9807245a126ddd59de992fc8b8627af4dd3cf6da38a`  
		Last Modified: Wed, 12 May 2021 02:47:42 GMT  
		Size: 5.1 MB (5074028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e28b75bd91c05df9e2403084c7a1160c21a93dce8b3591f4e77576118297aaa`  
		Last Modified: Wed, 12 May 2021 02:47:43 GMT  
		Size: 10.6 MB (10571291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:449fb7afd27d53ab79175a9100ca62434e6ac26da120f5b02e2a7900bb527d91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65236712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f72879a11d7541e9d58df33ade6be7734095e976e0014d02797a29ce8b527eb1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:01:00 GMT
ADD file:b91b8d2ef6efe2bd9fc0625108290b82f4567ba3654aeea20bd4b9e7c9fcacca in / 
# Sat, 10 Apr 2021 01:01:05 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:09:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e9c76177d1ffa0bc1a85678dee6f5c61b2264a677790342fc5bb17961fb8015`  
		Last Modified: Sat, 10 Apr 2021 01:08:52 GMT  
		Size: 50.1 MB (50083439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26176a706c2fe768e7e54369121192f2b1336a3ac2985c3b017b574b99f4164e`  
		Last Modified: Sat, 10 Apr 2021 06:21:18 GMT  
		Size: 4.9 MB (4935049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ba90a2781c4eed4854a1e54204b119cfe0e948ec34564b9e2235d443f69f1`  
		Last Modified: Sat, 10 Apr 2021 06:21:19 GMT  
		Size: 10.2 MB (10218224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:163fe5ec3721cb93cd467aa9b4b7ae9355fba3b97f21e531fc9af30d26c65eba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69609961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eae7b9054808151cbb12b203d9f7c4e85294963e871fa2d83083364957489e0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:54:16 GMT
ADD file:bffb08485a063deee6d89343a52bf604c1b25c42687e69b289d304c56a35e425 in / 
# Wed, 12 May 2021 00:54:20 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:38:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:38:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:187d6bdc2d3198067fb9a19db77a105ae346c5a0de7d9892597e87e77c9d4b2b`  
		Last Modified: Wed, 12 May 2021 01:03:04 GMT  
		Size: 53.6 MB (53579726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8afada75acd21128a315d0521b9f088d01bca2afc87f040802bf44907e04d96`  
		Last Modified: Wed, 12 May 2021 01:49:51 GMT  
		Size: 5.2 MB (5157609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bbf9f1d8a87e7d8c1e33819ddc87db8595e963b10998927f5227f657bd4e`  
		Last Modified: Wed, 12 May 2021 01:49:51 GMT  
		Size: 10.9 MB (10872626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c740d1f98c480540ab3a92c459763ad2cb26c601461fbaca5176e78c105e93d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72463925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818ec8f8eb55fd1e850795b093b60e30f9a09bf258f833b475f39de14d0a66f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:40:40 GMT
ADD file:d1e0da16153884c1e8fed94b01ed7a0d6215598889cf4b3ecda3e4e8e01a8a73 in / 
# Wed, 12 May 2021 00:40:41 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:11:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d1831ab5654d838d70f399ab69140b583b6195b99074487f0f45c8b5e2391a70`  
		Last Modified: Wed, 12 May 2021 00:47:50 GMT  
		Size: 55.9 MB (55915170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aa5558f76b4b2d18bec73cdedd5fada6bf73f54d0205204e99072673252113`  
		Last Modified: Wed, 12 May 2021 01:19:30 GMT  
		Size: 5.3 MB (5298708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46130a767ef67e909c93d812e14d36740b2d6673db70121b3239657bf7bf4467`  
		Last Modified: Wed, 12 May 2021 01:19:30 GMT  
		Size: 11.3 MB (11250047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:da0373807492bb0020dd62f73f520ecef947dfcd1b3f370c0e8595b3e01ba367
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69156990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d8d1552adc8b359cf9b29c1dcd537a68c602b125b0516f057419a247d4396c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:10:15 GMT
ADD file:dca45bb65ee8f7144352f7ac752f805807e971fc676ede954cc095be23566bf7 in / 
# Wed, 12 May 2021 01:10:16 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:02:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:02:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:02e79e4ee7225612ac3aad55b918cb4257f8e4ea2821e093d61ce58205474706`  
		Last Modified: Wed, 12 May 2021 01:17:23 GMT  
		Size: 53.2 MB (53155797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b63156a44114e717b4b43275afc2af76c4643abc5ccd5f74eb95f7154772c`  
		Last Modified: Wed, 12 May 2021 02:13:13 GMT  
		Size: 5.1 MB (5128666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b331baf926199e9584576eb92ab16ebc86d42b9f2840844dfe1a47f4a77ca98`  
		Last Modified: Wed, 12 May 2021 02:13:15 GMT  
		Size: 10.9 MB (10872527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dfe048de582cc5a1dd0f1c14efeca12c506af5d0d9b90f6ba8c0e6726003f573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75819119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337af443a6b5a399a1f993f55cf09d5a0154cceb47112574066aa40048b87442`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:27:11 GMT
ADD file:a41b62f9bc6147a0ab13a91e4ce5169739d220f716dc3752d7c872c9bf22748b in / 
# Sat, 10 Apr 2021 01:27:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:47:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:48:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:907e6a464bad63c32df38aaa0e848e3e09634237527afb1f8728bda2038576ed`  
		Last Modified: Sat, 10 Apr 2021 01:34:23 GMT  
		Size: 58.8 MB (58777775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d1d0df065cb2c84ba66e763425b139d7dc18eb050bf8cc5cb8dca7e25ac80b`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 5.4 MB (5420160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebdfc94479ccc35bbc35f2da43ced87239a8ca75ef23ce43d8dd981eab17c3a`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 11.6 MB (11621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4749a399c6319688a95603642b01662e0bace242c22e150956d2ea739f2f8074
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69097527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1668f7d17e60fdf765c72bb99f7db13f8fab3275c4750be5cf45e3e79ecd73dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:43:58 GMT
ADD file:22b27fbf0808244bac39e39b8239caa784e78a6b5682c7978c1cb4fac0813a67 in / 
# Wed, 12 May 2021 00:44:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:28:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:55e7e62594640e8831f8e39a7fe34cbb94c1ebfb345106b49c32b7d6c7e81eae`  
		Last Modified: Wed, 12 May 2021 00:48:17 GMT  
		Size: 53.2 MB (53183650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8529932d914624dabe07c03bc600a762580bed8457dbe8571680979ad85b69`  
		Last Modified: Wed, 12 May 2021 02:35:38 GMT  
		Size: 5.2 MB (5151016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a75f6cba4036a878c0379562599e814a8859cb2041c9de51c09b79bbed27a0`  
		Last Modified: Wed, 12 May 2021 02:35:39 GMT  
		Size: 10.8 MB (10762861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
