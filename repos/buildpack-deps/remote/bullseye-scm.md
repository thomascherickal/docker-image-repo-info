## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:653cd4c51d2a0e8d9e4eb377cf5cb3dfe3e6a90a579e08fee49742355a26e3ea
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
$ docker pull buildpack-deps@sha256:fd04e21a45663223207243344f0ac8b1d9c0fe01b1b8601b25d5686a0fdbaa2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125670325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ff4917fce4dadc637924ff195fcebb04273691c7152bcc869fb766c88d8e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9e7679f60e92aa82358cef8f564a6e732729b3503ca53e1b80a919f2a706c325
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120512477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bed037ffb511fba1886e0f3244960548195bab1a90822e8f61aee8e315aeb48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:56 GMT
ADD file:e5a40ed79070e00490d94152874430cb225b3b00e8ca84eed2bf5fc8c0bd8155 in / 
# Tue, 04 Oct 2022 23:48:56 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:16:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5662b6ce27f2ffe436703124b1912c3225002537510f22d7c95f9a34c5ec19bb`  
		Last Modified: Tue, 04 Oct 2022 23:53:20 GMT  
		Size: 52.5 MB (52547199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a80bb504cd29e69e6350b33a76059b83f8cfee21547380361b3f8c0a06f460`  
		Last Modified: Wed, 05 Oct 2022 00:23:40 GMT  
		Size: 5.1 MB (5070967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cab19d0fbcb73e4578935f0fad14812d8b9ab6a6dde7c7018aae6fae6b9dca`  
		Last Modified: Wed, 05 Oct 2022 00:23:40 GMT  
		Size: 10.6 MB (10573717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab0b688aeaeb9421000ccc7930823635add0db8f343233cc5dbcfe9dbdebd0e`  
		Last Modified: Wed, 05 Oct 2022 00:24:05 GMT  
		Size: 52.3 MB (52320594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50a85a985b089ddf5972b836da6a0053b066b489827aa55bac5f7bec2bf93ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115701649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f987ffe03e99e4f18811a3ed9c6b544fa00393058f4ef2abb83df5bc1d7673`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:afffe795f446d4ce92c983035a75c565bcc603854de8e5a09d4420f3a133fcb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123984044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989d35c51090cf662d136202df9df7e3a42cb4f60fd08bf918b51a818297719a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:23:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:23:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c953a37e989b49a533e8d08c80d87ce66fadee48160f9a4d8cd2dd5b0ec87`  
		Last Modified: Wed, 05 Oct 2022 00:37:21 GMT  
		Size: 4.9 MB (4944361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98802a15fc60bda24c79203236f930586f1dba6218aa2b4c121cf0dbf5627b38`  
		Last Modified: Wed, 05 Oct 2022 00:37:22 GMT  
		Size: 10.7 MB (10657400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aff223bb11e201213e82ed9838541b6a63fd9276370f73ed0dbdd6efd73e32a`  
		Last Modified: Wed, 05 Oct 2022 00:37:44 GMT  
		Size: 54.7 MB (54681658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:276c4815cc89619890b0b09bc6ae18bc3485e3dc61ab64829f331ec7db42ec52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128066279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef937282bba895e6fc33fc12098a6989a6d10ccb6588936175b58f398a0763fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15df4e6d66d7ef34631f8ac1f2f38abe91987ed6275417ef61001ed95b599de9`  
		Last Modified: Wed, 05 Oct 2022 00:21:52 GMT  
		Size: 5.1 MB (5086230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cdb6e95c7d15713b2674296dc059b3fb57437a59e6ae7f0a416810cac68192`  
		Last Modified: Wed, 05 Oct 2022 00:21:53 GMT  
		Size: 11.0 MB (11032979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee51252aba3fb7dac64a84b99f59aaea9ff1fca510ba6206d156dd0698e581f`  
		Last Modified: Wed, 05 Oct 2022 00:22:15 GMT  
		Size: 55.9 MB (55923264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a1acaa6746ce03d5ac1c9c184b9983adf517c0cc252294f448e9e9c51580b9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122150421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa73d3a5551fa701da480cd6d0b3d216e9aace1ea0d1de8201cd9fe13f05ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6df46a5d6a6c80757f20fe5f0b4177f75a338d6415069eafd4c7cf7955ff23ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134825393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93366447273bd8d73802b430118db4cb242c40c01aca13bfbd40dd2472144136`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:17:40 GMT
ADD file:74537fb4eedf6a0c9693fcdd0c9acb2797046cca66098b2e05d5c1a536a9aeda in / 
# Tue, 04 Oct 2022 23:17:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:52:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Oct 2022 23:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e05b86739fed11b3d0c5663063e627eebea0138239b30345630bc7e3f2549d5c`  
		Last Modified: Tue, 04 Oct 2022 23:23:34 GMT  
		Size: 58.9 MB (58917259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7bea042a44ccdc9501c249caf514fa6de00a3228715db35ba71c17eaf9c1fe`  
		Last Modified: Wed, 05 Oct 2022 00:04:17 GMT  
		Size: 5.4 MB (5412961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f894eeb91c899bc14a3e136246a0c07322d6c4b74067bab3f79e024985db053`  
		Last Modified: Wed, 05 Oct 2022 00:04:18 GMT  
		Size: 11.6 MB (11629009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3bfa3bf4fe3c94ca2fe03ad268cfe16d7ef5e1d219d4c86cb02ea8e8db4feb`  
		Last Modified: Wed, 05 Oct 2022 00:04:50 GMT  
		Size: 58.9 MB (58866164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c177f8af2234b7b32f37418cdcf1fb1f000cac0203c16c56fd3306b57b86e59e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123247239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f318d65cbe46ae5f8f285f69da689e86aff0f6e085b8beb68eceddba72342`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:22 GMT
ADD file:fb9c2e517bc349a0e6677548de7dd78a3c392343ca80152fc08744efe4e1e38b in / 
# Tue, 04 Oct 2022 23:42:25 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:10:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:10:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:11:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce03284d180c9b8801e9121eaf8daa52493209b61340c414b6b804b73ba5d1a4`  
		Last Modified: Tue, 04 Oct 2022 23:46:55 GMT  
		Size: 53.3 MB (53279735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25e6f765bfce349a1c11b8d41dab38a21481b1192abe8556233e2795f8aab85`  
		Last Modified: Wed, 05 Oct 2022 00:32:17 GMT  
		Size: 5.1 MB (5146912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cce1561740629c5ba38a89da20cb30d214952d490d528c360651330a776454`  
		Last Modified: Wed, 05 Oct 2022 00:32:18 GMT  
		Size: 10.8 MB (10765859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1820496135598ec73cd4a64e192caba5f100dcd08a66460a44332bbb02f26`  
		Last Modified: Wed, 05 Oct 2022 00:32:34 GMT  
		Size: 54.1 MB (54054733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
