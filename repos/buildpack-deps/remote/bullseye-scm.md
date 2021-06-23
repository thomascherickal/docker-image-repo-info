## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:e600bb79f6fe087030272fb0d1d722280d2e5ba98120f917842b6d464361cbeb
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
$ docker pull buildpack-deps@sha256:a968fbcfa1e91d4aad45753346252e4c6943be1cde332574ebfebde05d9bcd9f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120387955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd65c0cdd29a6d788d729f3117f19fe26f4a84d5544887d365d062af94b945e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:53:46 GMT
ADD file:776704b0dea7e9c9856d53c5db99eb2cac12414a59e66258c549cd32602f5f15 in / 
# Wed, 12 May 2021 00:53:53 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:49:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:49:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4470c8b9361b9718aac07fcf9a711d40000613ef3e0f694e3da9f5ae091dd9ff`  
		Last Modified: Wed, 12 May 2021 01:08:50 GMT  
		Size: 52.4 MB (52439186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763873e8e180836bcde25dbc607672fb53b7253594d501513fb643acf8f441a6`  
		Last Modified: Thu, 27 May 2021 20:03:02 GMT  
		Size: 5.1 MB (5061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a6f9785a03eed88540490a717438ff240f3a58e51af2ded1a200398a169ca`  
		Last Modified: Thu, 27 May 2021 20:03:03 GMT  
		Size: 10.6 MB (10570295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f059205b72a60f4cd8c4b1023ef8242980677b1dc3efe35bbfb3e43b8b015a`  
		Last Modified: Thu, 27 May 2021 20:03:36 GMT  
		Size: 52.3 MB (52316555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f429c96be7e11ea8f1c4195a1e769c8a0b7168d0ce24ba6493e3cbdc2e6cad09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115567499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703eb101f6bbdbe592de58286bb868712736b5d82ba97c6121256f9ad926244e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:00:23 GMT
ADD file:8ed6f13e7955c981e57f2e063b7bfca16927ded9fed3cbd231923f2fc092555d in / 
# Wed, 12 May 2021 01:00:25 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:37:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:37:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50de689ded7920797496a1e9f831f07c907224f7c629bb02a03a96ae30d367de`  
		Last Modified: Wed, 12 May 2021 01:18:10 GMT  
		Size: 50.1 MB (50101718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eadd03179b184db82df36753465390a99da5b2ae95dc934fcd05fb8fd8a676b`  
		Last Modified: Thu, 27 May 2021 01:01:22 GMT  
		Size: 4.9 MB (4921246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10155d4071aabcf375a96f3b69b17f5e9cb5e2f69cc8fea2cb2d87c0db3fa24b`  
		Last Modified: Thu, 27 May 2021 01:01:23 GMT  
		Size: 10.2 MB (10216154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727eafc84335571443c073433335986852106036b472e391f32ef466b7771cf6`  
		Last Modified: Thu, 27 May 2021 01:01:51 GMT  
		Size: 50.3 MB (50328381 bytes)  
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
$ docker pull buildpack-deps@sha256:8982d06da7891d47e78c4c4546b389f2213e13cf365bed4671fb7f3e0c14ebc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134668498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e0af692b2336b78406e7bec812aba505c9af12e0c544a7c55d37b5781af056`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:32:59 GMT
ADD file:dd3e802ee39ef6460fa54303399ebc1f08919c4011f872a9ea00cdee78e2e6eb in / 
# Wed, 12 May 2021 01:33:04 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:14:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:15:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 03:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79c001f710a199bddecf6231e4c1152e873413174cb20e083729089e3d15e400`  
		Last Modified: Wed, 12 May 2021 01:41:18 GMT  
		Size: 58.8 MB (58795251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772a696fa0c3a04186486f51e28b635be426e19d28f70066ae4451f4cdffb8e`  
		Last Modified: Wed, 12 May 2021 04:15:48 GMT  
		Size: 5.4 MB (5399466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b13560e5ca42c500abdc25b1eaba62e4eecf6c07847e8a5ada379658a0a0b10`  
		Last Modified: Wed, 12 May 2021 04:15:51 GMT  
		Size: 11.6 MB (11625194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117e253db3fe4dab977e1e87362629ddef48d98ecbb831fafb78e822287d9cd8`  
		Last Modified: Wed, 12 May 2021 04:16:57 GMT  
		Size: 58.8 MB (58848587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cfe29d9512b6aae119a95c23c42ff5ea1efaae1f3ec8b79b0ce0a4ec34c3cc1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123117017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2806793ee2d5f4871969d5644f9f2e8e3214e82edbc75b10b8505fb65f267879`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:45 GMT
ADD file:c4e658e7b0a2f1bcd1adbc3f8d4b90c39d22edd3817e41078cce53daa39778f0 in / 
# Tue, 22 Jun 2021 23:41:48 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:03:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:03:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:03:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:616c5ebef764d038df48c869a270b4c696a19212343d41c89f2f771e65bc2219`  
		Last Modified: Tue, 22 Jun 2021 23:45:00 GMT  
		Size: 53.2 MB (53183223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ba372b2a518f01bf5ef5547922449c0f61a5b6b5ce8af4f7f223a0acd13e3f`  
		Last Modified: Wed, 23 Jun 2021 00:11:16 GMT  
		Size: 5.1 MB (5134548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2b0dcb7538f1dea99896f8ad049a4690dc6d85a83e22119c18db98c8ec6b78`  
		Last Modified: Wed, 23 Jun 2021 00:11:17 GMT  
		Size: 10.8 MB (10760098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64e9bb1f1f4b5f50fae1eaf2cf21ba4a1a204b5b674d8c783140add7a2925a8`  
		Last Modified: Wed, 23 Jun 2021 00:11:33 GMT  
		Size: 54.0 MB (54039148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
