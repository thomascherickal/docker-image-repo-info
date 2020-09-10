## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:ff961ad052b609449756f2152ccb118b836b458742a8462dfa0ad6ec33d24d3f
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

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9f4c4ac33747c175f99969041063659fe55db6438dec2c47fdc8921a46eb589
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120033733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651fcceed5842b6b8de05882d67ce13cc1c2a7ddf0274a9781944d1fb277d5b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c1bdc28b78815a8b40f6b687ed6b080dbebe5019ad76960a8bac51adfacf6e13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114729432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac928c7e543c81c1d6e8d4a4d21d66566f06c23f5eac33d20568223484d5d3c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:11:38 GMT
ADD file:e1152998db9c9a59e88100fa415cb22c317d906c5143042e7e36fa6911264f66 in / 
# Tue, 04 Aug 2020 03:11:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:13:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:13:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 06:14:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e007f43c47fbc3bc147d3d82021dc9a400b509f9c30dc687c1a3ed5fd23065`  
		Last Modified: Tue, 04 Aug 2020 03:33:39 GMT  
		Size: 48.1 MB (48108803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0270eaf99061a6aa3af6cdd0f5e0ae94bf697d7565783759c971252b202c37dd`  
		Last Modified: Tue, 04 Aug 2020 06:36:56 GMT  
		Size: 7.4 MB (7360991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e527b7990670f219ff9d29ac8963fbdc4756e6c6190434bba9c0482626f4ca`  
		Last Modified: Tue, 04 Aug 2020 06:36:57 GMT  
		Size: 9.7 MB (9687011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556ab5cdb159eebd1404529d56d69ebe7cdffa65e8113e5d41a2e11fee7a734e`  
		Last Modified: Tue, 04 Aug 2020 06:37:26 GMT  
		Size: 49.6 MB (49572627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6ce46ef63064b37020ce6fe10ced25586c6e35754d754622a1d20df089a667ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109666263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0bb260567cac81a26d6b2e92dc66e2d77f5e656ebb7c9c2d0e00a57937c3ae4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:302516a3d6e3c3fcc03d6eee297189f5c96379c5addd85344665541efaba0252
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119005173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11e88189bb0c1cafcd952aec5c8877c547dadd4403b7b10ab2e2d93bb9f6fcb5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:21 GMT
ADD file:c8c11e622b1b8a1e31f32e2457ff4d1314d5cd4a7ad22b3991ab9d0542db23fd in / 
# Wed, 09 Sep 2020 23:50:22 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:28:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:29:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3a32671b6316bd11f4bf18cb034394ac94d2bb3bc6d09de388b19b06fb94b91`  
		Last Modified: Wed, 09 Sep 2020 23:58:45 GMT  
		Size: 49.2 MB (49175549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1202c4ddac582c7164a6b65b13a2442759bc04660da9ca7d62fabf75225482`  
		Last Modified: Thu, 10 Sep 2020 00:42:35 GMT  
		Size: 7.7 MB (7681394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f110d64c20212ec5e7a7f0622d610346edbd6e508fde94679db44e0f2827b2f9`  
		Last Modified: Thu, 10 Sep 2020 00:42:34 GMT  
		Size: 10.0 MB (9983858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c41999aa9f871546022553f35d4fbbd39cd2bfe8e1a03cce7b1bd78d2a5b0`  
		Last Modified: Thu, 10 Sep 2020 00:43:02 GMT  
		Size: 52.2 MB (52164372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3955845c72fa280b6c891f9b811539bdcf2a7ac219a4dd8e3d3bd4662658c5c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122911849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0e8d52556e0840ec86df56739323434539fb27c9924596fd7dfcb2dea08fe8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ed766f5b5aed902fac08bebe9008529da19538d5cd52003c49d506449d259230
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117106740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0e53a53f72a3288653778e17c9a25f9bf26152d2d276af00326b80bb923270`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:01 GMT
ADD file:b98dee5937df5f9781b3c514a8c53f6f42fa8016979e581d1252ae689da15ebc in / 
# Tue, 04 Aug 2020 06:42:01 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:39:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91cc9e0aa8bcda5d45dd8780d9369f22c649c4d8fcd354183a1d0d6a7102744e`  
		Last Modified: Tue, 04 Aug 2020 06:47:56 GMT  
		Size: 49.0 MB (49017231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1447a30fea55273b0a628cb142daba1f5482171d155f458d47b5cadd49079d9`  
		Last Modified: Tue, 04 Aug 2020 10:50:50 GMT  
		Size: 7.2 MB (7231573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2846bcb2ba044284b6ee8c358e6d443ac48b4e01c2e72e0f8bd252128a30a0d`  
		Last Modified: Tue, 04 Aug 2020 10:50:50 GMT  
		Size: 10.0 MB (10015826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb4e1f307e1aa9ad1acfb68478ca06e971c7136b431f8d954ac34b08301dd7a`  
		Last Modified: Tue, 04 Aug 2020 10:51:40 GMT  
		Size: 50.8 MB (50842110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8575ac9b16c0c21c43631f66eb0f42a804fb40711271455093485c783f803f38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130580403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2afc146caa4dfd0f16e55b673ff5d707dca409f185026e0a4a49ef8b719bc5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:44:59 GMT
ADD file:7cc5195cf323fbee8e0c74a76984198dca35599ab18b1ecc5639fa719326bd35 in / 
# Tue, 04 Aug 2020 04:45:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:15:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4e2d8d5901311f959f0a2271be587f91ea2826238f2a17347ffab142413f53`  
		Last Modified: Tue, 04 Aug 2020 04:52:50 GMT  
		Size: 54.1 MB (54142497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe2d012519ce68bcd2414835909fb4784fd4eb5bea2c88916fdea0c661c872e`  
		Last Modified: Tue, 04 Aug 2020 07:45:05 GMT  
		Size: 8.3 MB (8254809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f1d1f9197bf1817cda35a89da9bd2544ceb7bf0c7b92fba5977ab2b2ab9e6`  
		Last Modified: Tue, 04 Aug 2020 07:45:07 GMT  
		Size: 10.7 MB (10727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1301750ffb48db80c63d6d21adae9f88f4f4aaf4f561ab3512287683a04c04c0`  
		Last Modified: Tue, 04 Aug 2020 07:45:33 GMT  
		Size: 57.5 MB (57455994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9de3cda15fba829b061b05fac221ceb9b647c83ed7074ea557e177e3f673be29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117613682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1c4e16faa4d9586600b7f891593e7ade48e0a0da5009d58de08c78a0e3079d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:11 GMT
ADD file:67eedff26215ed3c8100b93d0201c563ec8efe2af7bdfff5c7717037f95057af in / 
# Wed, 09 Sep 2020 23:42:15 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:06:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:07:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c594945c9b37f16bdb296d1c06754e5bbcc3c28a736d7aa6091f61a081b3cfb`  
		Last Modified: Wed, 09 Sep 2020 23:46:12 GMT  
		Size: 49.0 MB (48966294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e127f29ba8a9174c7c67de6a285e78af9f06c2c36fed6521332d7854917d2782`  
		Last Modified: Thu, 10 Sep 2020 00:12:13 GMT  
		Size: 7.4 MB (7385208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e209a7f0db80455bc526e00593053bd27892e74f2f355899c7b05b2f8b74dce1`  
		Last Modified: Thu, 10 Sep 2020 00:12:13 GMT  
		Size: 9.9 MB (9882116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d094fc7b8815cbefc16bd1eb31d1052bf6fa6016dbaf460808e7a49665906c`  
		Last Modified: Thu, 10 Sep 2020 00:12:27 GMT  
		Size: 51.4 MB (51380064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
