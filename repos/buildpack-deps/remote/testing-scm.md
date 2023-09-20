## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:352eef28e9d72e13892f627d4e16cf85cdf6bf0af957cf27463af316224bdaac
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
$ docker pull buildpack-deps@sha256:f33c8e96705c40209ee56dd09395a9ecb5b713a223dad78a41f6dc954a02c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123566268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c450fc305174f9eb7d21e13717c1d3512ed305729d8775f1410a84fdab7814`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe3001385a2b717c083b0eb81363b8210958afe6ccf0dfe6a62a78df022ec5`  
		Last Modified: Thu, 07 Sep 2023 01:49:25 GMT  
		Size: 18.6 MB (18600941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39960ddda116bc7eddff9010f7bdc11c97332a0ea990a5a7e825d0cdcc2868a`  
		Last Modified: Thu, 07 Sep 2023 01:49:43 GMT  
		Size: 60.0 MB (59954833 bytes)  
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
$ docker pull buildpack-deps@sha256:31878c48a551e60acfe2aa68406016be01f64a82e69b53d72d0ee701a6f32cbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137871241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a958d70d6528e570ffe292108ab492680225ccec8f02c354a108b0551e4342`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:44 GMT
ADD file:5d53bf28b6cbc8eac8124a07c0bb8e04ee2d0c8989a8b7219612f6ced4f064bc in / 
# Thu, 07 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e0d37cd24f690f803c53e61b67871ef6d1dd8980331679da74a8059a191a9fa`  
		Last Modified: Thu, 07 Sep 2023 00:49:00 GMT  
		Size: 50.5 MB (50534548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b76d6a16699dd100cc2549b60405a4d0d78dc30f81cc263bee0da056e922a5`  
		Last Modified: Thu, 07 Sep 2023 05:42:45 GMT  
		Size: 20.8 MB (20840661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc12640afdfa7cf01b8781ab7883502fe26134031f798e3a1391eb3c53ff9125`  
		Last Modified: Thu, 07 Sep 2023 05:43:08 GMT  
		Size: 66.5 MB (66496032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:046462eed28745d1caadd54b9dda3bc4b442d35bbd759eb1657dcacd290ea312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132549205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26e1bffc8263b56c40daf67e3080482d2c74fb716bd092b220df4286228a706`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:13:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9d654b3c49c164cc43a4683b85bf2e1374ecf02ddb2c3f7187cfd204ec3309`  
		Last Modified: Thu, 07 Sep 2023 04:30:10 GMT  
		Size: 19.6 MB (19559687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8decd0a052b38d92ca1b1753f6ddbe6c1df433473ed31f5705fe4bb91479355`  
		Last Modified: Thu, 07 Sep 2023 04:31:01 GMT  
		Size: 63.6 MB (63632011 bytes)  
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
