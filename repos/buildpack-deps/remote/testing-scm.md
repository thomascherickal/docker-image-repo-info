## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:4986e5e42fbb130a1f45bfc6f985f1fd92830f4f3e385b558b62951df1779b33
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9e0a8aa83c5ef72705654241a78395b4a932531fe4ac4280f6e2f9e86399f608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127359227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc650f26de87c3ae40d7984a71993c79833d41e7aa05403fd271c593620618`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:00 GMT
ADD file:91c81aa3735ab11fcf7db3eb2dc51c94759276e7d3657f0fe81829c133f7c8dc in / 
# Tue, 04 Aug 2020 15:42:00 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:24:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:25:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7bda3d6de74128f57cc726f2172127887e010c6a291320273a9c9eb8ad29209`  
		Last Modified: Tue, 04 Aug 2020 15:48:28 GMT  
		Size: 51.8 MB (51838182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8231f0c7125cafbd1f958df6356c90a0dc3947e50ede3c176820814176b1318`  
		Last Modified: Tue, 04 Aug 2020 23:38:27 GMT  
		Size: 7.9 MB (7921995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4f23b97ad1b9a745be0f1e7dc1856f9a233a25a83f51b22fce0c16759de05`  
		Last Modified: Tue, 04 Aug 2020 23:38:27 GMT  
		Size: 10.6 MB (10580797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2bf24be332afd3092d09e178f69ceece27993e6347cf9f2b4fa4526dc9131f`  
		Last Modified: Tue, 04 Aug 2020 23:38:44 GMT  
		Size: 57.0 MB (57018253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f0f509aa2b1281b6818b79851c4359e8f57cb0b942c7413ea5c38c988f4665d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122141087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f14ae55c02d4f48fccd5aa756ec271e95494992d5ab5eef7843828070bbedb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:08:44 GMT
ADD file:2b581429c7fee51f5899cbb76a5d9c36cf7223edcbb473fbe2f8db3a53a82263 in / 
# Tue, 04 Aug 2020 03:08:52 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:07:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:07:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 06:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2a8e3d684f3a7d5eba8b8ba267ffcbcf9d2089c1f803e105113f8b34f8991e`  
		Last Modified: Tue, 04 Aug 2020 03:32:48 GMT  
		Size: 49.8 MB (49784523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa91b4ecc0f372adaedd757806f1b23aee559777f06d525ee224f6f2911c31f`  
		Last Modified: Tue, 04 Aug 2020 06:35:19 GMT  
		Size: 7.5 MB (7501685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9150d7965ec842da0721c1a458d2f16e78d852da4190dd6c46b4d82e38e27476`  
		Last Modified: Tue, 04 Aug 2020 06:35:20 GMT  
		Size: 10.3 MB (10267288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c670d1433953e1f7e99c5959030cdd629bc54e680c8aafc16116a6288cbada`  
		Last Modified: Tue, 04 Aug 2020 06:35:44 GMT  
		Size: 54.6 MB (54587591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dc0d3bb22fbdf7c2ff080f358a5ab720817dfa359fa6eceb1cd19391a3ccf26f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116987373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9c486c009ed7fdcc7c620b8af73493246d6589825b65a88178b9d402290043`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:55:34 GMT
ADD file:8d817c9168a8bfbddda5007f76443d27203cb5bf02ec609cd277ddc327736b10 in / 
# Tue, 04 Aug 2020 04:55:36 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:45:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:47:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:984ab044320fbabd5c060737e15adfea7aa109893b7f68f41abc04f445d3440f`  
		Last Modified: Tue, 04 Aug 2020 05:04:18 GMT  
		Size: 47.6 MB (47570419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93473ce552fd633dff0ed8a7eba4610e368b271c6582de1c474472a31cc7340c`  
		Last Modified: Tue, 04 Aug 2020 08:24:12 GMT  
		Size: 7.2 MB (7243678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9559bb2ff9f55098d0aae9e6210eb73fdb47f91e0b6fff535ae21fcbbfa54dea`  
		Last Modified: Tue, 04 Aug 2020 08:24:13 GMT  
		Size: 9.9 MB (9915965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ff07294173b72b0b22d817ab0dce8e848d6eee67c264eafd80f785b1c18e4`  
		Last Modified: Tue, 04 Aug 2020 08:24:40 GMT  
		Size: 52.3 MB (52257311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:456764d92d150277ff944a80bd582e02e0e3e671ffc22d375b8bfc3548d0aa9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128464883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e53f4959ed29952caab2a521652504697dcfda9ec054ec138a41c89161f26ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:49:11 GMT
ADD file:82c33a26fb9be3ddaf17956539af2b205bdb6e28fe5ff1c7304ae8f294fe9581 in / 
# Wed, 09 Sep 2020 23:49:14 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:25:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a65667356fa05b061c6733c879afab36ec44c6877341c2527e321b7206a26b2`  
		Last Modified: Wed, 09 Sep 2020 23:58:05 GMT  
		Size: 50.8 MB (50825395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730279b4ebb859065c90bbf90b3ac77059bd7d1e6cdc143106e0994dca9f4c59`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 7.7 MB (7743447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2c8b657c8d1b22dc8f6d15821f7035a315a0900f84b26ef36c86803feb02c`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 10.6 MB (10635675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c8357b95e1bce3c0d061d88bd56a0cbc03afe5af4f86cdd0057650adee23ef`  
		Last Modified: Thu, 10 Sep 2020 00:41:30 GMT  
		Size: 59.3 MB (59260366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a6c332caad95c733778a2845cd6ddf655b20f3b6f7f77a36d0d4187949b0ba8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (130979148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b997d35c79905934deea6f8b4edb2fe1bf65d5e35e198b64428770b8e0a4215`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:36:50 GMT
ADD file:e3f476fccb15ccc08c3c8c26ac23f1909e7c0f79bc060289f35fc37bb4483f80 in / 
# Tue, 04 Aug 2020 03:36:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:04:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:04:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:308ce7c38ffec8ca43e219653810c298ee87abfaaa068ff112f1e8003b108546`  
		Last Modified: Tue, 04 Aug 2020 03:41:50 GMT  
		Size: 52.9 MB (52909727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429c636a1f75410c98b200faef3ff9f568a242579e0d885a7b7c70d771f96e9a`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 8.1 MB (8099324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e845809b7e141a8bd0e85748582037ea1e08bcb9ca449097624dfc315d876d2e`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 11.0 MB (10960569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a782bddafbc0654d5b0e92f99d7ee9edffa1960018fb14017095b3dae8bfc63`  
		Last Modified: Tue, 04 Aug 2020 08:24:45 GMT  
		Size: 59.0 MB (59009528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:55d9c46fe77c5e9908caee88749ca4248f90d2047179cc76df351baf44dbfa13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124573680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a03d50c4e56edd082db5a7e00b38d6935ed82820c3ece0e87c7ae4a4d574a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:41:13 GMT
ADD file:9e3d31545fae8b44e8aa3ad24629d2336276c01e23dfbdde9885d01e61a54298 in / 
# Tue, 04 Aug 2020 06:41:14 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:33:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:34:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:35:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:249c58d6beef4ec2d380f0e2adf7ea99a80c295cddcf6f6bc3d6b463dfe44a05`  
		Last Modified: Tue, 04 Aug 2020 06:46:35 GMT  
		Size: 50.6 MB (50550783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049f809de28cc8d8e169ab9ee5721613f58fafdc670bbe6d66a1058fe998ee06`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 7.5 MB (7450522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557e2093dc94091a8f931745b728c83f35ad977f14de65f1ec5db00bedf8580`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 10.6 MB (10599039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d597a52166ec3c0e83e53c0b933c57f9230d87fbc629e0c1fb4c68970dec8`  
		Last Modified: Tue, 04 Aug 2020 10:48:22 GMT  
		Size: 56.0 MB (55973336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fe5fd3ddd6bfc9df82e2058b94be41831c042a374edc7378813cbe47d98d3add
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138014766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7d996f16962ccfd58a8911b097e03706fe5f2364f7dc0f0f43710d60edf1be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:43:52 GMT
ADD file:a1065b5d1a75daf3153a753a23c630c5a77451644b83418dd23b2c1d046c970d in / 
# Tue, 04 Aug 2020 04:44:00 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:01:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:02:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:03:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26d0cc426ef5200b8e12941b37f3b65f8de8a01be463ecfef94be00ae56f5596`  
		Last Modified: Tue, 04 Aug 2020 04:50:57 GMT  
		Size: 55.7 MB (55655910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aadce00449a8701783ecb72b8dce872a06609d7a90a69b4dfa29a8727a1bc3`  
		Last Modified: Tue, 04 Aug 2020 07:42:12 GMT  
		Size: 8.3 MB (8347825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f8213614f8c61ad803c5be08bb2ca48b08b0b8111551a50801c69e31afcf4b`  
		Last Modified: Tue, 04 Aug 2020 07:42:13 GMT  
		Size: 11.3 MB (11327020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a3017101817902f76986e15e141f0d4e7a84d78f35d8e4ddb6d03363fd29d6`  
		Last Modified: Tue, 04 Aug 2020 07:43:26 GMT  
		Size: 62.7 MB (62684011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e0ba2a654b46559d6df1bdc7c65a171b7321ede89a2e55016e846916c89c75c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126741432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d8646c50c6005345fcb6b1be73815e012477fe41713783251905305dbef4c6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:41:38 GMT
ADD file:d30705fcc57734260b517d32c4d610f1fe18e7d5faa78a22754774f5bf15eb9a in / 
# Wed, 09 Sep 2020 23:41:41 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:04:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:04:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7fac0c9089d6ff39f6a7de3af657a8d580a7b074b45118b115539fd90213654`  
		Last Modified: Wed, 09 Sep 2020 23:45:45 GMT  
		Size: 50.5 MB (50468550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e4abf36c400373c14e1dc03dc7d41c9bb01249ef118a39b67294471b0cea9d`  
		Last Modified: Thu, 10 Sep 2020 00:11:24 GMT  
		Size: 7.5 MB (7537717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c291ff634945f7dc165f540d95c5d3958483aba31d45fbae0ee30d37ef13ca7`  
		Last Modified: Thu, 10 Sep 2020 00:11:25 GMT  
		Size: 10.5 MB (10504927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6369fe3859abc7090769cdf547264b790f6a68071ae32f9e9cc6ae6002948f10`  
		Last Modified: Thu, 10 Sep 2020 00:11:39 GMT  
		Size: 58.2 MB (58230238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
