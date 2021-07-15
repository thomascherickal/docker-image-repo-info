## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:ece9dbafa8d4a7e4fa55ee46f22f3e63d41786c0321b5ea2e5c6d50acb8096a4
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:af76b549bfdad564d7fd0296d7a55bdaf48debd22264c81548712c15a047990e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125488416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eff4738961cc8bb982cd12f3ca821618803e889f408a1846d8c3c67c75da7b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:59 GMT
ADD file:eebf6f761892ad2407885aa93a2abf7647cf0367e3590f3cc7971594ff47193c in / 
# Wed, 23 Jun 2021 00:19:59 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:51:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:51:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:51:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d28ba3bddf26336a2dff9ce3319ecd166971168469860f171fa659f62cb3ff6d`  
		Last Modified: Wed, 23 Jun 2021 00:24:24 GMT  
		Size: 54.9 MB (54898218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf411e1e4e47abd58ba697cdc3f8f769d452520d81804d6260ac2edb014fd41d`  
		Last Modified: Wed, 23 Jun 2021 01:00:26 GMT  
		Size: 5.2 MB (5151216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab85705b51fb188c0567dca75cc18291fe81258917cbae6ed4d271ae1e1e1d`  
		Last Modified: Wed, 23 Jun 2021 01:00:26 GMT  
		Size: 10.9 MB (10871097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d458df13ef560766d7247fad9531a5df62c87a39c070e22fc435608be267e463`  
		Last Modified: Wed, 23 Jun 2021 01:00:47 GMT  
		Size: 54.6 MB (54567885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:798f8536127d4ccc9b402920056b6ee1cf83db5ed369ec34a18da82b5dcca7bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120388158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbc1102d5d542ea617049322b4d835ed12cb02ac67a432e38db009b3b4c1251`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:48:50 GMT
ADD file:b1ab65bd906b52c44584b6aa35e2e9a14d5fccf907ac8b12a8bd3ab106368f8d in / 
# Tue, 22 Jun 2021 23:48:52 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:34:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:35:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:935ccf98b4128795cbb17daf7b631ae49bbffbf371e91db72950c1cc501fec30`  
		Last Modified: Tue, 22 Jun 2021 23:59:35 GMT  
		Size: 52.4 MB (52438388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6b5ddf0e080d4cbe3848dc082adebdfb2edceef0085a3fea40d17f5855037`  
		Last Modified: Wed, 23 Jun 2021 05:54:02 GMT  
		Size: 5.1 MB (5061948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79d8c8405f06e8f06e3d613e24bd2abc13798270d01649f5b4bca6f0ecfb97f`  
		Last Modified: Wed, 23 Jun 2021 05:54:04 GMT  
		Size: 10.6 MB (10570340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc95d3484be6753e43f5f052db8364ae5ff3b38fa20fb4e5ffa73561d1eab9a0`  
		Last Modified: Wed, 23 Jun 2021 05:54:56 GMT  
		Size: 52.3 MB (52317482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0f87b8f6836a61abd369a33cfffad09f39c9d3faf4e550e6c6bbcd8393b5eeee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115564669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d248abf130815a0f0e0de2b0c4c07081420664b44ea103b00e331e6f18d2d6d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:11 GMT
ADD file:ad79d7d1e72695a6bc5bc7faf963aa10b7640e18d61799368c033154d25f4074 in / 
# Wed, 23 Jun 2021 00:19:13 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:41:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0d841baf75fbfb347b67a1e92382bad913e5ece75d2865565bd39c673601fca0`  
		Last Modified: Wed, 23 Jun 2021 00:29:49 GMT  
		Size: 50.1 MB (50099210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a9693512c3e7bc760e8b1622077fa47c2596a70a48e0f089a6ec190c88b2df`  
		Last Modified: Wed, 23 Jun 2021 06:15:42 GMT  
		Size: 4.9 MB (4921106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0617c8a98b65b4803ec110b1e886a4e1c0c0ea78f2c46198421d90dd1c7cb314`  
		Last Modified: Wed, 23 Jun 2021 06:15:43 GMT  
		Size: 10.2 MB (10216086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba86a9cbee8cbbf64ce4737774401c28436ab21e02fdd8cd12e40a25ab43061`  
		Last Modified: Wed, 23 Jun 2021 06:16:31 GMT  
		Size: 50.3 MB (50328267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0678716bba0944f516bdd5c4f7bdb5d7246f8476f761faa6ab6daecd36040cf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124261685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05e8a046787818ef5cf8a8ba842768398c4b002bc1f58c65d53a249a36932d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:00 GMT
ADD file:4a6460733f3542d1957e24a1b1640ad7a76b0e4d8aee727e7d2ad9ecb8baa5be in / 
# Tue, 22 Jun 2021 23:49:01 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:23:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:23:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:764e5bfd58ff2b8baf2ec95af0b179082665955a271e28d9b50d4ff1917c2c0b`  
		Last Modified: Tue, 22 Jun 2021 23:54:07 GMT  
		Size: 53.6 MB (53582009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ea5376efdee8b03645276110ca156d0bbdd3889e467593830f7e683fedabe`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 5.1 MB (5140889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba64b692b9483da8feea34bf3f3f5f6650d0883ba74afc0083588f0a5e6219a7`  
		Last Modified: Wed, 23 Jun 2021 00:32:01 GMT  
		Size: 10.9 MB (10872087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815da70bf68dcc179be2dac2056857794591f8179b9388f924ed26023bcfcd91`  
		Last Modified: Wed, 23 Jun 2021 00:32:23 GMT  
		Size: 54.7 MB (54666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0f9dd6b71319f6d04de641f763da7df3d029504e558e6dff7fe90940c119d27f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128357731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:938a68a47badc6480cb99a14b83181ba37084d480d03b16541b830cfae76222f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:38:49 GMT
ADD file:ed43ceae72cd0b1a1ee0ecf4319bf0a9ff0d8cc4542a983609d4df18ccb3133e in / 
# Tue, 22 Jun 2021 23:38:50 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a1a10c368f246da8fdeabb7eecba4e66e58cdc28feb3b3f7714896e4f52dd56`  
		Last Modified: Tue, 22 Jun 2021 23:44:57 GMT  
		Size: 55.9 MB (55914378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8155b7693984d8cf280e3297045a2d6e4381a5942504ce0cd264fc90f9d3adb`  
		Last Modified: Wed, 23 Jun 2021 00:16:25 GMT  
		Size: 5.3 MB (5280678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8daea17889b2d1f7c6b1d266c5f433c93d238bf490f3cf4f26ffccc30ee4600`  
		Last Modified: Wed, 23 Jun 2021 00:16:25 GMT  
		Size: 11.3 MB (11250163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eed415b97421c9054a680b99d565726e14e9be2842282558742d42542bf12b5`  
		Last Modified: Wed, 23 Jun 2021 00:16:50 GMT  
		Size: 55.9 MB (55912512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:23416f572d33667a0b532fd56fb6449d33cd3e18fccefa66d3650a1c38a51865
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122436622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4c54261a504ad02773c10a555723993ffde1a5c5cd9e77b1184907afb38b00`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:08:19 GMT
ADD file:c35f12783d634fefd92f2d45605502f97a497b66a15f60dfccb4b2a2d4a293cd in / 
# Wed, 23 Jun 2021 00:08:20 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:37:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:37:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:38:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ebc6252e914164fc2a31f5418122631ab0e70c83ecb8f8b24f7e1ca5f4f2fa1`  
		Last Modified: Wed, 23 Jun 2021 00:13:48 GMT  
		Size: 53.2 MB (53152965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fcef1ce2b6c14e25f573bcaef690fda6b4e405c35a7b1b8952b7b62c3c8024`  
		Last Modified: Wed, 23 Jun 2021 00:50:30 GMT  
		Size: 5.1 MB (5113563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec06bd468c211fbc95164b859ed15795c4a88ea59bad6a4f3e2ea99c8f83804`  
		Last Modified: Wed, 23 Jun 2021 00:50:32 GMT  
		Size: 10.9 MB (10872897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9ac5966eaecb31300f2e111a48e6b68689426faeb9cd62c328ab8c289bfb8e`  
		Last Modified: Wed, 23 Jun 2021 00:51:28 GMT  
		Size: 53.3 MB (53297197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:04e86cc1a316cccb457c183f6f37f367bbc0b532784b8e1debaffc77ff525c9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134685753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4252fa6dff1e6d1ffb77aee6f5b9ab042b950696bc179aecf47d6a25694b709`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 15:56:25 GMT
ADD file:902a353e8fdec64f149d504baaf70654faec8f23749856644d0edeaf32da0fba in / 
# Fri, 09 Jul 2021 15:56:29 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 06:07:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 06:08:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Jul 2021 06:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09c77b0cc13f990901884e4cf084070a3b7c2d5058b18159ca0117900336d82f`  
		Last Modified: Wed, 23 Jun 2021 00:35:48 GMT  
		Size: 58.8 MB (58810873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421b0d6d9b6902a218e70de32058d29eb3078735e0c5952457b9c374d3fabf`  
		Last Modified: Sat, 10 Jul 2021 07:04:16 GMT  
		Size: 5.4 MB (5400638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06931f6d94bfc8b50c98dbdd3744053f9cafab50a00461e1990c3af3f5d8158e`  
		Last Modified: Sat, 10 Jul 2021 07:04:21 GMT  
		Size: 11.6 MB (11625404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad2b91ac3e7f764cf135b13868ee0508f6f6429f1da7c0ba00aee2fcbcc6469`  
		Last Modified: Sat, 10 Jul 2021 07:05:08 GMT  
		Size: 58.8 MB (58848838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a00da5060f007dff4794ff118651542221708518bac6b0671e6c98bb9947ac57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123120080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aff73d9dc8b1919d585a078c4d02574e4f0b2de89b05ce9727f65a1f8f99e5e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:49:41 GMT
ADD file:c4e658e7b0a2f1bcd1adbc3f8d4b90c39d22edd3817e41078cce53daa39778f0 in / 
# Fri, 09 Jul 2021 02:49:42 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:40:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Jul 2021 03:41:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:616c5ebef764d038df48c869a270b4c696a19212343d41c89f2f771e65bc2219`  
		Last Modified: Tue, 22 Jun 2021 23:45:00 GMT  
		Size: 53.2 MB (53183223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefd3f7b2b655822c9aba7a1b29d50eff7e7a7e082ac0a358bd57248f688e055`  
		Last Modified: Fri, 09 Jul 2021 03:50:33 GMT  
		Size: 5.1 MB (5135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8047c349992a015d306c9d6bc3fe69efbb81bd7d913eb1eb1fbf8969713996d8`  
		Last Modified: Fri, 09 Jul 2021 03:50:33 GMT  
		Size: 10.8 MB (10760401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e62a5341198668b99735c6293fff68d376b8a99d83d329165321b14926fd5c`  
		Last Modified: Fri, 09 Jul 2021 03:50:49 GMT  
		Size: 54.0 MB (54040709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
