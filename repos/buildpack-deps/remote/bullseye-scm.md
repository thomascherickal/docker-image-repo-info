## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:c7031cfa14d861c8c363cea86252006bf67e120a6d92e13da190348351c572b2
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
$ docker pull buildpack-deps@sha256:dfff17c4317c954868c77bfbbe97680d7a0671789464e3dcf45d7fe05eb7fdd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124785647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8771905bfeb983a2f7362dda3b3f6741c1d8eec4ed4d5ebae7e3ab244a98361`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:24 GMT
ADD file:fa865518757ef9e0af03796e7abd6cbfd59e20f5ae325422e41524615051a2d1 in / 
# Tue, 17 Nov 2020 20:20:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d004aa4da82e9e47169ac4cccf33df9b52bef6dda8aa5f7b0bcb03af34078173`  
		Last Modified: Tue, 17 Nov 2020 20:26:32 GMT  
		Size: 55.6 MB (55578105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5514b41a34cf855f2908da965f01f2b0f68fc62b29b9fb67811a07e7c61d16`  
		Last Modified: Wed, 18 Nov 2020 00:47:23 GMT  
		Size: 5.1 MB (5063216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3985bf4e3bf68c52363fd7853ecc6142b55501eb8457558d27ae10a0358e8907`  
		Last Modified: Wed, 18 Nov 2020 00:47:24 GMT  
		Size: 10.6 MB (10645972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f00fbcbbd3c3783e061ff8d861834c157f06601ed495383250dabb36682027`  
		Last Modified: Wed, 18 Nov 2020 00:47:43 GMT  
		Size: 53.5 MB (53498354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b01cb55a5adc9d935895d80f079e7d419bb7e1333639e9ce9df35376c0987704
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120364930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004de1c79142aa4b3421e80d01e033bdafe4933fe2bc1f929a96ac1af4e12935`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:8b9117df3f1a986438250b725bc8ec117cf1caba2e6953cf9a870edbcda4c565 in / 
# Fri, 11 Dec 2020 02:03:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:37:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:38:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69233e69b29a579de45732361ee762ae02ccbe96b0f2a09fc2a48a802a25b265`  
		Last Modified: Fri, 11 Dec 2020 02:13:31 GMT  
		Size: 51.1 MB (51053259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d208cbc2dd055b46a0eb797352719db7e40a64bb90bab94b3d64b5b3b1c4a6bf`  
		Last Modified: Fri, 11 Dec 2020 03:04:31 GMT  
		Size: 7.4 MB (7444057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8ae15eeacf7f92e597567cdb02de06832bdbbcbbc72e66d77dba4a1854f649`  
		Last Modified: Fri, 11 Dec 2020 03:04:34 GMT  
		Size: 10.3 MB (10335286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63c9e301bf107aaab041c8ea9ccf08104e472540b7fad385a3c0c9b14a93cb1`  
		Last Modified: Fri, 11 Dec 2020 03:05:00 GMT  
		Size: 51.5 MB (51532328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3e46f6097ba1c37048ff3714d4ca548456fd9342f7b9894f210a56e3dcc5e62e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115480434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b29b5a80f549e26353988678db64a0e23df6b4c3492270e233e361c3c4a452`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:22:18 GMT
ADD file:f1ca2b90268fd790612e08e0e01b5ea1b63749dbec2ebb79b37a6168e5e82815 in / 
# Fri, 11 Dec 2020 02:22:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:18:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3354b3972c3003db2792ea643d0250983d6938232305c0bd0b2f3f8ee458c9ca`  
		Last Modified: Fri, 11 Dec 2020 02:32:03 GMT  
		Size: 48.7 MB (48731592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f0027df82d0578bcc2d43af7c68680af181d153ad76b785b97e3ffb1a53e8`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 7.2 MB (7185940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f21be10a21df5869d3131ec5a4c6715acb9e45fe541b0050baa4013a18f0`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 10.0 MB (9974110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cd80ba9b81350feb3d9ed853fd31625b9a1308882fe61f8cee95c338f871d7`  
		Last Modified: Fri, 11 Dec 2020 16:41:50 GMT  
		Size: 49.6 MB (49588792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ec8c805e804face54e02e0c706b563be8024584a92f5a8a6027dd8e38b03aacb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123642431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6f4d56db5489fc7cbba023ce812204f87aaa24b3bc731e106ade1251fe7197`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:22:08 GMT
ADD file:58908becb64a88c580fc5d9fea54a7e73507d1e537e70b5567f5d58c26ad000d in / 
# Tue, 17 Nov 2020 20:22:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df1866c47e1fa1c26619e32544732be4853c6b58bfe5ea76c192ae970daf5da7`  
		Last Modified: Tue, 17 Nov 2020 20:30:56 GMT  
		Size: 54.3 MB (54323419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71907b4dd26e793f4e9841e590a1a930f7265a02f7c07e57767ef9cbe91f8b`  
		Last Modified: Tue, 17 Nov 2020 22:33:52 GMT  
		Size: 5.1 MB (5055744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2cf86d1130240ba8633c0151d4a4a4b9e6a251bf8ec2bf14d72ce40a67727c`  
		Last Modified: Tue, 17 Nov 2020 22:33:53 GMT  
		Size: 10.6 MB (10648270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c6056c2ca2fb8c36f5f80c875444bbf38dab5bc7ebf358fd257bac133169fb`  
		Last Modified: Tue, 17 Nov 2020 22:34:20 GMT  
		Size: 53.6 MB (53614998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:112273b5796141d07de61def08f0ed046485c72266e3d2e98a0f2cc1a62f740d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127762353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da19a817a8d76b76bd6d6be3370876afac4eb49838e404ae319c22a60f7343ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:01 GMT
ADD file:df88ece8f6b35ea6811921d958952eb8431b76449597cb6d5151e88c62167964 in / 
# Tue, 17 Nov 2020 20:19:01 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:01:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:01:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:02:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9137c9a05e5bbf8d80413499157abbe788cac975a7926ded72bd9ff285f7520`  
		Last Modified: Tue, 17 Nov 2020 20:25:46 GMT  
		Size: 56.7 MB (56728874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd9994454c4b84708c2d9754f396aac9f662a7169c2322418210f8d161ac4d`  
		Last Modified: Tue, 17 Nov 2020 21:22:12 GMT  
		Size: 5.2 MB (5182817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87786a5db1b57a9ac7c14addd518c4d55f9ac878f951e8110866257d83d6d82c`  
		Last Modified: Tue, 17 Nov 2020 21:22:13 GMT  
		Size: 11.0 MB (11022570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88de8fd349f0d1c859351edc10905c5adca2e975f84e43d737a1933c7ee86944`  
		Last Modified: Tue, 17 Nov 2020 21:22:35 GMT  
		Size: 54.8 MB (54828092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0e3bc85ea4c775692bc283766353add81ea870ca87a34405d21ce36d6c4a61fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122479987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffab2120d2f5f553ba6252c116926942570e71ac5cfd80924900a920d949928`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:20 GMT
ADD file:1c9d3b0dae65df3d925c78ab44bc00642c930f3deef925694dc0c1a3213de35a in / 
# Fri, 11 Dec 2020 02:02:21 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:44:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:46:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede4ac036d71d6e9539de8a220d9f79c46f7c9cb9bf53f8498188327ec302195`  
		Last Modified: Fri, 11 Dec 2020 02:08:06 GMT  
		Size: 51.8 MB (51829610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97d6058f001d48012d3119e7be581954924dd50d584771418ffecb191be4d2`  
		Last Modified: Fri, 11 Dec 2020 02:58:53 GMT  
		Size: 7.4 MB (7410105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5e05d9ca9fe9992047f5f69faf9d8cc20423eba1ebf9226cd16e85d820255c`  
		Last Modified: Fri, 11 Dec 2020 02:58:54 GMT  
		Size: 10.7 MB (10656688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f67c25b93b905661111d2e1ac9d028619abd3d68daf06b9e2d83aae2342219`  
		Last Modified: Fri, 11 Dec 2020 02:59:45 GMT  
		Size: 52.6 MB (52583584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:282c0780784f22f8bc7a390b4815b57b16d4b1b7be55e45ff06ffd602435dfbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134297203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7471653717b8eb9ab9ad25b46e43e273d1db5d364e166f471a3c87344b1ea24`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:21:22 GMT
ADD file:2194006ac3b70de157ecb2806ad599d0c7994e239170bef461ecd9ac5f7f7528 in / 
# Tue, 17 Nov 2020 23:21:31 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:26:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:30:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc7190938049d8573412a9fa0fdcbaffd5e24ad75693e87ff89a4f37791f0907`  
		Last Modified: Tue, 17 Nov 2020 23:29:22 GMT  
		Size: 59.8 MB (59761557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4c36e5042edb900f63e80ffd0e14c80fc84b50d9d0983b6e7f46898e988fa5`  
		Last Modified: Wed, 18 Nov 2020 01:46:30 GMT  
		Size: 5.3 MB (5302380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2b5d04b45968683b84bbca4828b6ba15fe17909e3c64cfe7678a9d180f99b`  
		Last Modified: Wed, 18 Nov 2020 01:46:30 GMT  
		Size: 11.4 MB (11408115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953d5427968cc8c9a1c8ddb3e8a07c98b8fc47806f8cd1fd0f6eb9428e8fe9c`  
		Last Modified: Wed, 18 Nov 2020 01:47:45 GMT  
		Size: 57.8 MB (57825151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:daa773908a4543e14ecd9fd47e402bbc815ec6fd12b51ff8b80294b0e9fb956b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123073098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6485cea7a4c062a13671b7d834319daecb43cd9e20804d5d70f59ba241532064`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:03 GMT
ADD file:74a0f68651d74636caec45b24b97289c444300a4e20ead2e9dd4ecad9a89b149 in / 
# Fri, 11 Dec 2020 02:11:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:56:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:57:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 15:58:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c1102ca26cfeafe4e6f6b885fc1f8b1c19daafd157e556c9eb528d215f3ec2a`  
		Last Modified: Fri, 11 Dec 2020 02:16:10 GMT  
		Size: 51.7 MB (51656809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5318fd9b9f903620dcea8eebe0d1b3e4c22fbc8b859c0bf46ac13755d1a52a`  
		Last Modified: Fri, 11 Dec 2020 16:14:25 GMT  
		Size: 7.6 MB (7565720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845cbfbba3746772baf57c643c9a8edde11b111c4a69407f278d0c47ace4f158`  
		Last Modified: Fri, 11 Dec 2020 16:14:26 GMT  
		Size: 10.5 MB (10525441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739f79a56621b8c3834393733c04a12d896e7ec992d0f284d592926bb45255ae`  
		Last Modified: Fri, 11 Dec 2020 16:14:42 GMT  
		Size: 53.3 MB (53325128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
