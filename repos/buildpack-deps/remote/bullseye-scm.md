## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:01941c0e1635d37307eb72fa6d4e99274046e69e7e16f0c71eb85f55cf08669d
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
$ docker pull buildpack-deps@sha256:40bf118ca0f938a4b7c607af043400a7e08de7d67efd7e877ed8f454288dbc4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134685019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc51c925b32448bdc6abd4035c1b4493f86368dc3a917a6499ca37ec84efe78`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:28:56 GMT
ADD file:902a353e8fdec64f149d504baaf70654faec8f23749856644d0edeaf32da0fba in / 
# Wed, 23 Jun 2021 00:29:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:08:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:09:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 02:13:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09c77b0cc13f990901884e4cf084070a3b7c2d5058b18159ca0117900336d82f`  
		Last Modified: Wed, 23 Jun 2021 00:35:48 GMT  
		Size: 58.8 MB (58810873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6c805420c238dddbe4c715e87fd16ad2e71d52a3036b1a48f06e6584d64cbf`  
		Last Modified: Wed, 23 Jun 2021 03:11:48 GMT  
		Size: 5.4 MB (5399574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e0528ffe8427919da60d21c425a0bc9149c5ab77a889114c2b164910ed13df`  
		Last Modified: Wed, 23 Jun 2021 03:11:48 GMT  
		Size: 11.6 MB (11625302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dac324cb49459105c8f24ac4140888956a65e1b86ebf62d06119935807d0cde`  
		Last Modified: Wed, 23 Jun 2021 03:12:11 GMT  
		Size: 58.8 MB (58849270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d5481a43545a50ac7d34f7d74654eea04fc0de258bcdbd8bac822a2595201ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123119157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895e70922614a7c78633d0f8755c50c9b1bcd7d7e4936a7870229df01388d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:45 GMT
ADD file:c4e658e7b0a2f1bcd1adbc3f8d4b90c39d22edd3817e41078cce53daa39778f0 in / 
# Tue, 22 Jun 2021 23:41:48 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:25:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:25:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:616c5ebef764d038df48c869a270b4c696a19212343d41c89f2f771e65bc2219`  
		Last Modified: Tue, 22 Jun 2021 23:45:00 GMT  
		Size: 53.2 MB (53183223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737c98df0314ebb29463b455192c2ddadf2fa88b14c144696f90208ba852c5dc`  
		Last Modified: Fri, 25 Jun 2021 21:39:55 GMT  
		Size: 5.1 MB (5134629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a78c11ffa8e166c5614d89fe616afdab1b7a87ea98e165bc32c45f08e210459`  
		Last Modified: Fri, 25 Jun 2021 21:40:01 GMT  
		Size: 10.8 MB (10760386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2e05502d0861f3314ebb136802cfd9a4f4cdfe298c2f89a4a0c82af42329cb`  
		Last Modified: Fri, 25 Jun 2021 21:40:17 GMT  
		Size: 54.0 MB (54040919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
