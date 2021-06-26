## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:a1ad7ec6b2b7b7ed9c5e16a2c0a5e6e4f596d7955e05b5efa4d06490ab4162da
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:afb029322d4178a02dc3b018ea6be5b78ddc3a646d84f9afcd215ccc38516283
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126205019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4fac7dc096ecd81fb205f24a2fcd62f82f2c576603b605696122d3efd67b6fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:14 GMT
ADD file:5745436941906af011c9450820c7baff61a091235f04da258ba218ca450622a5 in / 
# Wed, 23 Jun 2021 00:21:15 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:54:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bbd4da8ff6e19a9b86585f9b55dede690ca6dca9f96d946fa1fb6456182931cd`  
		Last Modified: Wed, 23 Jun 2021 00:26:45 GMT  
		Size: 54.9 MB (54902493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0246214aa0ecb6ede7631e54d50bebe607ad610e577d4fbf6857d6b158e7dbf`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 5.2 MB (5170501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35d77eb31156f1996620962d6772ae81841ad63c839af8f4841118c8410fade`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 10.9 MB (10872573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c94a6468c400151537722b4a6b82a7e4fe16655ef49643f3ef4c591fa91fe`  
		Last Modified: Wed, 23 Jun 2021 01:03:34 GMT  
		Size: 55.3 MB (55259452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:59b5d43114e8e6ba1c0fe689fe79676ef4a8977b7d049acf65639c84c970b359
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121054119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719f2b3d5c8f5cfc48e8aa1a7d5ab3527883f2be8a359531881adce7a7702fab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:21 GMT
ADD file:6f138ddb818c5f09c669ab36feab96f8445d36fb1cf1263f9c3fa7ed334d14a9 in / 
# Tue, 22 Jun 2021 23:51:23 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:43:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:43:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4336d4df3d0160b4c6137b83e3c61fb0dcc6d38a51f2eccbe2cb96b75500f65`  
		Last Modified: Wed, 23 Jun 2021 00:03:50 GMT  
		Size: 52.4 MB (52440085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da427d5f1beeee9b5703b32a33e4b43db3a9512ed77d21591733d938dd07a245`  
		Last Modified: Wed, 23 Jun 2021 06:00:34 GMT  
		Size: 5.1 MB (5075069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f214b11d05abfca12f1b6f7c7ea433c7a204d7f6b4113383a0600cbba119e`  
		Last Modified: Wed, 23 Jun 2021 06:00:36 GMT  
		Size: 10.6 MB (10571940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54e2fc2ec25ce2da62055fb0589733c080b3749628cabcc0bb9f2f1880f89de`  
		Last Modified: Wed, 23 Jun 2021 06:01:28 GMT  
		Size: 53.0 MB (52967025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a68fa52ae8cda39b73133eb8dc829fcf8961ce695cf909e307654bb293e18c78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116185018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46748faf632f438417f0350c76207bfabcae013001982b4bfeedad36777d70ec`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:40 GMT
ADD file:10ae021b5b2998c7ee0904a6d9b6a3697ef580d3a6b0a0980c2f209a6ad2bb29 in / 
# Wed, 23 Jun 2021 00:21:42 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:49:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bb9348ee5f2e424d70e44ac1d1e0b029bb37d72f6050453f93408edc2af9176`  
		Last Modified: Wed, 23 Jun 2021 00:33:47 GMT  
		Size: 50.1 MB (50105618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10d3401b65a0651a08c5c29f2e1207dc4ca1027e80abc9b35cf15c88d96958`  
		Last Modified: Wed, 23 Jun 2021 06:21:43 GMT  
		Size: 4.9 MB (4936190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5dd2865193f1b761bf000f90190639fb8bfea0ce5033bf2de30ad2d9738789`  
		Last Modified: Wed, 23 Jun 2021 06:21:45 GMT  
		Size: 10.2 MB (10217331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f157f0331915f121358a516bb24081ca7d6310badb3e864d7a50a1e81882`  
		Last Modified: Wed, 23 Jun 2021 06:22:33 GMT  
		Size: 50.9 MB (50925879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f1acc49c42f6372c4266b5486c5aaaab1a043f193c5cbff5455ecbe0709bb68f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125024342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308e7757bedbe74ba23302ac1ed059d5c862cf8c8bd25f632fc9a920885adf62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:14 GMT
ADD file:339319b02d36af7daf322a0b1295cc9416a58c021a5f5ba7a504f28717588cea in / 
# Tue, 22 Jun 2021 23:50:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:26:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:26:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:26:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e1aa4e0221ceafc83fb2f0929a4a51d5784e6bd00ecdfc3672853b28868fdf17`  
		Last Modified: Tue, 22 Jun 2021 23:56:31 GMT  
		Size: 53.6 MB (53586541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7626ab4adf6f17b187ebd4dddff8961986d7954ecf61d62b69eaa7ced1a128a9`  
		Last Modified: Wed, 23 Jun 2021 00:34:41 GMT  
		Size: 5.2 MB (5158799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f68a62ea25befd0307cf6cab1bf22ed625727daa8fcc5c452219a0bea940c1`  
		Last Modified: Wed, 23 Jun 2021 00:34:42 GMT  
		Size: 10.9 MB (10873185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6612ca213cc17f4e7c8e850bbd08e3342a7fb58ff637b59bc667f3bfb4792eb2`  
		Last Modified: Wed, 23 Jun 2021 00:35:03 GMT  
		Size: 55.4 MB (55405817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6659db0ec76e1ce8c3435017e4d243fd35cd99bb22d5bbf6e4d7e37c199ad13c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129131440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab03a0a89a12e2955c80614f29f214b564bb762e4c6374843bf1290af24ee3d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:40:18 GMT
ADD file:20378fd7bc859874d8620bd807402968cbe571a1ca281d0f344392ed5d8af55b in / 
# Tue, 22 Jun 2021 23:40:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff9feaae647f307940e0b5cfdb30f3d3a877220cd3394859c1af4b3d653b2e97`  
		Last Modified: Tue, 22 Jun 2021 23:47:46 GMT  
		Size: 55.9 MB (55914853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5310b9c9dfb8fd34f5ff4cccb1d7af5e1baf20620d64357dc51a0e69717717e`  
		Last Modified: Wed, 23 Jun 2021 00:19:34 GMT  
		Size: 5.3 MB (5299879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab8c3b07912881a8d38f2ca51a04fef6fa1d22c0163da069cd226eec7362a07`  
		Last Modified: Wed, 23 Jun 2021 00:19:35 GMT  
		Size: 11.3 MB (11250598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66c7b3456d19d1557f96e2c7bf74716f3187c850af8e39dbbccf8890f4c354e`  
		Last Modified: Wed, 23 Jun 2021 00:20:00 GMT  
		Size: 56.7 MB (56666110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:96773b4f02300d6e483feafe2afa795ee4bb758038c1dc708a651bd41841cf3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123221813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d20a999706ac9c6584d98907547ac8b0c92a5a65e4fc7c59c630a0aa5199437`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:56 GMT
ADD file:723b0881c85ba05a782aae0c0dfbbca4283e1a595a167af6a9a9b23b34916226 in / 
# Wed, 23 Jun 2021 00:09:57 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:46:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f938924a38054ec92bd31be4d18e4f654308796e5e915428065faea9385c73d`  
		Last Modified: Wed, 23 Jun 2021 00:16:36 GMT  
		Size: 53.2 MB (53157176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df9715e9403d707b9879b1f23718b1730cb5cf3feb4f483c137a321c7a2dbab`  
		Last Modified: Wed, 23 Jun 2021 00:57:10 GMT  
		Size: 5.1 MB (5129996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6704ed06dc069325a9235d3c57db6d14a34623f005bd10aaacc4acb2b42585`  
		Last Modified: Wed, 23 Jun 2021 00:57:12 GMT  
		Size: 10.9 MB (10873312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdace0ce09b260021353f35b35cc0d8e2dc930fe2d1cfb3cbf0cdc51c6f5c681`  
		Last Modified: Wed, 23 Jun 2021 00:58:02 GMT  
		Size: 54.1 MB (54061329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:04d0ce34de5495cfced7668a1b4be9bae5afd3221cc60ca8d4fc38142713ba98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135526426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd1f4c07da144dc407f2750eb066b6c0608494062453c25e7fdc0cf121ab7979`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:59 GMT
ADD file:9d5a0ba0a24f9a37f3d9812637e4beef52ef27fa65d76c97dffa3f4933633701 in / 
# Wed, 23 Jun 2021 00:31:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:53:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:54:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 02:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28a36a9b0ca23da4474256976c303c139c5800da883d61fb1e52bc74123ba134`  
		Last Modified: Wed, 23 Jun 2021 00:37:34 GMT  
		Size: 58.8 MB (58812906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ce3e2f4d09b0f4d35d601239d717711e3f893fb78190eaa180b1adc8dd92d`  
		Last Modified: Wed, 23 Jun 2021 03:14:37 GMT  
		Size: 5.4 MB (5421248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbe87f0a03412b2b5a32d8785f613157b9523c1f863846b35bcc432d61fdf5`  
		Last Modified: Wed, 23 Jun 2021 03:14:38 GMT  
		Size: 11.6 MB (11626445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aaf9f7c5ff36a26cf0399471711dcb660cdf03278f69c6b3514de580cb110a`  
		Last Modified: Wed, 23 Jun 2021 03:15:00 GMT  
		Size: 59.7 MB (59665827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d991aef5f8fdff78d9ab52be37aef235b6b01147f2baddcde8bb7e35a49f9d66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123814228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27711bbd88a7a6d778bab922057d0d6629da9fa56428c726c4beeb4d7a389828`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:38 GMT
ADD file:b2361f35b2807ada58f66b4f4f160b2133140a85db4ecd56889a15f080793790 in / 
# Tue, 22 Jun 2021 23:42:40 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:29:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:29:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:29:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:247ed76d4285ef2f620cc0d1ec3492f8a6d1b0cc613aadf4e236db73dc508cca`  
		Last Modified: Tue, 22 Jun 2021 23:45:59 GMT  
		Size: 53.2 MB (53184006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38beaef678629ec960494a9226e20ded66d424e512e2f8d97b09696ae369ba9d`  
		Last Modified: Fri, 25 Jun 2021 21:41:53 GMT  
		Size: 5.2 MB (5152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c768f7d61191fae5d7b88323c8a65d317729f892fd66add7fb09f14947f0dd2`  
		Last Modified: Fri, 25 Jun 2021 21:41:53 GMT  
		Size: 10.8 MB (10763666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b24f017823384ca0156ad13648b596fd62658a1be4e80f8732a82b181f00f`  
		Last Modified: Fri, 25 Jun 2021 21:42:09 GMT  
		Size: 54.7 MB (54714391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
