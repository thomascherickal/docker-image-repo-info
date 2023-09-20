## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:102c9990201297db9743231999e602892a619db801e99364effff77cea932d73
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
$ docker pull buildpack-deps@sha256:9a8dc5fb0de072162e4982b81be18e4a99362490bc9c98f73c555dcf73df7526
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134405925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117234419216a3681e04989309f0040e891a89fb4f7df17d851ec6be0c779d71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:58:17 GMT
ADD file:cd33732baf7a8215a9cb532ae6f2fe0be64d030adb1f3e0085e461cf4f22ec4d in / 
# Wed, 20 Sep 2023 04:58:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:27:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3954180d94025620e480192adbba35d582d59582f662e17f992f954d83539feb`  
		Last Modified: Wed, 20 Sep 2023 05:04:48 GMT  
		Size: 49.5 MB (49467670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e565cc2b6bbf1308bd8312f40ad760a99d8567113763dec2537af6652bb673`  
		Last Modified: Wed, 20 Sep 2023 09:34:11 GMT  
		Size: 20.3 MB (20269130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10974eceaa5affd1244428fad92105303c6661b8d09326a7a85b3f11de3125`  
		Last Modified: Wed, 20 Sep 2023 09:34:28 GMT  
		Size: 64.7 MB (64669125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f99ac269e199347fb1b7a43f0af61e63beff877a6a4229c6f8dd6f1e0575f732
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128788593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dcd9ae9b973a889c32892023e3a566f71825952a198c125d85b3673b639c2ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:52:20 GMT
ADD file:c6e1ebf545b4fe8a3d6b8e0eccf515df1d8291411d23a0e5002f40428db8b992 in / 
# Wed, 20 Sep 2023 00:52:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:02:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:03:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7cf8ed3fa4a717011b456890e76475bcc7f559140833924436b7fe1266ee31f`  
		Last Modified: Wed, 20 Sep 2023 00:58:49 GMT  
		Size: 47.2 MB (47170081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2095ec2ed427a717bbeb48fd093ccb5d091ef08c9a25fade3d48178836b9f874`  
		Last Modified: Wed, 20 Sep 2023 10:08:49 GMT  
		Size: 19.3 MB (19346047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb293bf1cbd7cb52e62601f49f2c2be990e63ec593b249e5cbe527fee70844d0`  
		Last Modified: Wed, 20 Sep 2023 10:09:08 GMT  
		Size: 62.3 MB (62272465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:acc1ac9ccab26e28edb954d8e260875e34f182a69fbd41f4c808e6dbbcf9a925
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123464789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e25c02dfee843291189105d29a2af30aca75f3577ae0f728e0f731b908c7bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:59:32 GMT
ADD file:48b3882ac99c385930d3ac71ac20fda8a1b071b08088814bf1a41054078ecd14 in / 
# Wed, 20 Sep 2023 04:59:32 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:219658aab374640dcbab3bd1cbe574955f68e4305522bfc19564d1ce15fed88d`  
		Last Modified: Wed, 20 Sep 2023 05:05:38 GMT  
		Size: 45.0 MB (44955127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e0f2039e0f302927a38df2eb35fc70587db403fbc14273b4fe098c21cb0969`  
		Last Modified: Wed, 20 Sep 2023 15:39:33 GMT  
		Size: 18.6 MB (18617697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba45c0e5519ac44055eac6898a4c8abe790e1be149095e9a8db5eaf719de3e2`  
		Last Modified: Wed, 20 Sep 2023 15:39:51 GMT  
		Size: 59.9 MB (59891965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:62cdd36e486fbfba31d2a255c213764972eb26e99f08194f4b844c196f51f9ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134112117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1690bd93425160bc1ebb8c7c2d8cb0487c2e9f140265b491a348e86040ad69ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:58 GMT
ADD file:dc9be3a1e3e1904a1eb81053b568b583a58307e861fc56fb1b7ce9349d2faa18 in / 
# Wed, 20 Sep 2023 02:45:59 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:30:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:30:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d433462e04ded836d58eebb0fee68803768bcf3c9f92338a2cdda77bf7bef8d`  
		Last Modified: Wed, 20 Sep 2023 02:51:30 GMT  
		Size: 49.4 MB (49404499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f21fb48a05deec994e76626b5ba27bca3dceb8c7026037ba821d1ea929fbf5`  
		Last Modified: Wed, 20 Sep 2023 09:35:50 GMT  
		Size: 20.1 MB (20054013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb2f4db47f9fa43103b397742352887aade94ad72694c0f3eb40923c90c10f5`  
		Last Modified: Wed, 20 Sep 2023 09:36:05 GMT  
		Size: 64.7 MB (64653605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b2f8e0b1cb619c1ba31c7ce085545c95d7775d0172284ac333e372bbb2afa83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137824119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92558f5a493cac7344e3474a66d997568d18dc6b7af721aa59818d80c08faff8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:44:37 GMT
ADD file:9e992ca17751b113240a189433e8f77647c4ebe62d129da1b528a8d6a3702972 in / 
# Wed, 20 Sep 2023 00:44:38 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:34:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd505a05e9a1d549793b6c0278e192920932cc3051d24604cbaee75803a68342`  
		Last Modified: Wed, 20 Sep 2023 00:51:58 GMT  
		Size: 50.5 MB (50484788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cc9ae28e9bda901dc51164cf94a986ae909c659e90d0c25cd8875aa954d2de`  
		Last Modified: Wed, 20 Sep 2023 11:42:34 GMT  
		Size: 20.9 MB (20853303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918107427c2cb228f04a420f2253a41cf0b3eb4b65b3ba84caf3838923d4cd15`  
		Last Modified: Wed, 20 Sep 2023 11:42:57 GMT  
		Size: 66.5 MB (66486028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:727e9fe1f77c1588185b66afb3f2b80418419f6129f90f0789a088ff2f8bd22e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132468867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2282b32b790ecf43c4a34a9a80a2be5ae8755940d0b68ab3693a0b8d911d8154`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:16:43 GMT
ADD file:feafc03e82af46c6c55a0a73cf1d1107968b6694a898de04dbd04b90bd98508d in / 
# Wed, 20 Sep 2023 03:16:48 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:12:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c3624a744ac0024156b087e27ec700730d5abd850c903edaefd0cd35bb20d02`  
		Last Modified: Wed, 20 Sep 2023 03:28:01 GMT  
		Size: 49.3 MB (49302317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee833587bbee7c28ebb44ce27cbd72e6bb33739d9203cf1e4464b7ae564d8c1`  
		Last Modified: Wed, 20 Sep 2023 22:30:41 GMT  
		Size: 19.6 MB (19560312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8fb39bb7824bc4241044104821fb808dc3b6465ce10625a02aee85775a106d`  
		Last Modified: Wed, 20 Sep 2023 22:31:30 GMT  
		Size: 63.6 MB (63606238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:72156954a9b099c40a23a0a3d8d0304f1d0138aff7df3283798ca1af79f5ccd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145145534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b15dc951807aea9f1b2f0ef4d0996a84eab120881da236326efab433a6fd5f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 08:47:34 GMT
ADD file:67c6bc6190a4808adcfff4395e6c56581b3752c48d672a8e0f2219a636f2a300 in / 
# Wed, 20 Sep 2023 08:47:36 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:10:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:11:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9a74cf8b7ffbe83932cf1e965d34b5885f2faaf418add2de59cab2819786fdd`  
		Last Modified: Wed, 20 Sep 2023 08:54:05 GMT  
		Size: 53.4 MB (53395271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c71db45c4ad54904bb2bce74d8d742f2d8dbdd2d22c4dfa8a8f5fc93560b7`  
		Last Modified: Wed, 20 Sep 2023 10:25:35 GMT  
		Size: 21.6 MB (21603073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7335db3fce1eb0b4617264ad0d31360a888034f9609729b7030179a1f1377309`  
		Last Modified: Wed, 20 Sep 2023 10:26:02 GMT  
		Size: 70.1 MB (70147190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:674bb59204439f695e8d2ecb8cfa4d7d8eb3805b156a68d603366044937a4fd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133052627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3fda32daff1d5d2e7775f8c7ca9457ef232955d4dfbc336765f0d759e9437a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:57:24 GMT
ADD file:77b51e0abb2ed786e762b44ab5463930ac60fc37a4a4404ee62cf4653a99e1fa in / 
# Wed, 20 Sep 2023 02:57:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:54:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:55:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dcfbcf60cde4d1764ae5735832195c5a57365459959cebb93c0e57bd40fd54a4`  
		Last Modified: Wed, 20 Sep 2023 03:02:19 GMT  
		Size: 48.8 MB (48760791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b239420005ab6c651870ef013ed3c379e88028e2ae4355642040198cb4a863c6`  
		Last Modified: Wed, 20 Sep 2023 10:01:14 GMT  
		Size: 20.0 MB (20005597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724dc0240d930e9ebf4eb3a0070c3eb553d06a44798e05283cc1cd48b73a5b82`  
		Last Modified: Wed, 20 Sep 2023 10:01:29 GMT  
		Size: 64.3 MB (64286239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
