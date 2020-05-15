## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:fb9920f54caf7fe8d6d032e17abc2cd8cc831539db34da48ee4d327612a6e56f
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c09d42a4140e52df1a8de0c321fcad4e86ec0224f76f4fbdba09ad65e997fbc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125443464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c72cc1ef3b4dd3f150fbe712a73467b66fd2f6c9e58e7d1ad8bc7c557b67716b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:22:30 GMT
ADD file:1b99a100214a4a86a413bf6a826c70d07fee06a8c4e6d1f3ed1550fb08f9818e in / 
# Wed, 13 May 2020 21:22:30 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:37:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:268c82fb25093fc20c25872a9f96ca2bef121a19a81a91079b62afb96b725135`  
		Last Modified: Wed, 13 May 2020 21:28:35 GMT  
		Size: 51.4 MB (51390987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a426d8c659d27b64d66f82bd62c2bb3dccd6560447f354396111cb0c27bc0e8f`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 7.9 MB (7934296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac7ef969a4b66cfe2e8dae9867620b1821ab5b3d64e9e37b0a3ca56f574a44`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 10.5 MB (10463093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137f68410074c0abacbce781d17f5b40e894982fa38e5f1cf1edb52c3274181`  
		Last Modified: Wed, 13 May 2020 22:47:51 GMT  
		Size: 55.7 MB (55655088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e70916e9c42e3c9948e60f624b44e1e2b0827146e347c28453e102bfcbefc828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120339032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:281edccf5d5244a5265f648b9cccc3be0acee17456d47d963761cfe12a3cf606`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:40:47 GMT
ADD file:c2ef493946404baae91412a79e2336f831835f471608b615f053cc8cc1c1cb62 in / 
# Thu, 14 May 2020 22:40:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:53:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 03:53:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d6200ebef6b4ed212e54012a0718d6122f96033e0dbe7fd95e64d7739c61b3f`  
		Last Modified: Thu, 14 May 2020 22:49:25 GMT  
		Size: 49.4 MB (49372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e62f5ec2c655eec6bc82424f1d1705ab9a002004800db4b3d6d52fd101c1f6`  
		Last Modified: Fri, 15 May 2020 04:04:43 GMT  
		Size: 7.5 MB (7514186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282c779adbdc0e96ca8947af087a331e91a4c580e8c0092a57044a79a102cebd`  
		Last Modified: Fri, 15 May 2020 04:04:43 GMT  
		Size: 10.2 MB (10157673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f3bdc712282b5930840ac3a7ac356ab96426c57f00967b0206ef981809fa22`  
		Last Modified: Fri, 15 May 2020 04:05:11 GMT  
		Size: 53.3 MB (53294225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dfffe679649e73c83a8aae178eaa4668d613715c895e407ef21f6906a33c0198
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115323548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8641a82edfc03910bd0d127b3b9392043d5d7d3e7091b7a4ea2d316ede2e318d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:04:08 GMT
ADD file:7bc7b5e94debaef8aabee3128de6e535c9867794ed42649aadb9ba63a66a547b in / 
# Fri, 15 May 2020 01:04:11 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:44:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:45:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:921baaddbf45818850d057b247e93c5fa875838ac2dbf11e2913f526f5ac4d94`  
		Last Modified: Fri, 15 May 2020 01:13:34 GMT  
		Size: 47.2 MB (47179178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b833ddc7c9debd21799cd19fb7e5459feeaae463d767cea9ca2c02209d4e68`  
		Last Modified: Fri, 15 May 2020 10:59:56 GMT  
		Size: 7.3 MB (7257028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dd78efb72e462bafeddbe0df6aa29d83c9f987bcd797c2d1cb8c813c1bc59`  
		Last Modified: Fri, 15 May 2020 10:59:57 GMT  
		Size: 9.8 MB (9804694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ae802f2861549b9a8f8f8971dbe9e7155dc358caa0271ea51893756a3893e6`  
		Last Modified: Fri, 15 May 2020 11:00:21 GMT  
		Size: 51.1 MB (51082648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e3ba12e2235d011e4f880e849a32e67a1afde170328f47a247878a10b1bb5267
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124399187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee784a6fb5c1a9b7355bbbca5e59aad03af09ffb015da1b89212b1595b0e0eb2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:45:26 GMT
ADD file:22517e10f0b5d2760fafa2367b5a187d7ecef96291f15a746c24bfa50f756219 in / 
# Wed, 13 May 2020 21:45:29 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:27:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:28:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad0025dc69d6f0241b2f5b614e96cef6e1fd54c9ef07b726338235b4766714ea`  
		Last Modified: Wed, 13 May 2020 21:54:40 GMT  
		Size: 50.3 MB (50328664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de8e099b34fe681d2134dc5800a33dcf2d66893cc852ada1704e600b8e46fac`  
		Last Modified: Wed, 13 May 2020 22:41:03 GMT  
		Size: 7.8 MB (7809465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2735cc8b188a094edcf282e931946b14d50022e973d985f72d13b23f3a1a810`  
		Last Modified: Wed, 13 May 2020 22:41:04 GMT  
		Size: 10.5 MB (10459849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c718f2ae452283da0b15ae79d609faee60fe428710fa0ad565afc8198c9f8a`  
		Last Modified: Wed, 13 May 2020 22:41:27 GMT  
		Size: 55.8 MB (55801209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8093fc719f2ed5b0713fc5bce8d700d979b836f51a9143bcee9c20704f92ab1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128954305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c36d0e0f04f5823cf29df0dbfe71a7d17bb676c653eaf99d582ee4ac672477`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:18 GMT
ADD file:bbf57f6406dcdfbee8d207ada2ed9150a3e775fa2cb6e0784c3e35e1c3216d25 in / 
# Wed, 13 May 2020 21:41:18 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:54:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:54:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:430f489239f0254d72f3974fb8f614ac80ef76f642ab0bddcc4f20a8d4a3c68e`  
		Last Modified: Wed, 13 May 2020 21:48:41 GMT  
		Size: 52.5 MB (52481574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65cdd6becdc738c09b87ead3f88dbd9e0a0028929d1d7f9698c406b2edfafa`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 8.1 MB (8112129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2540c9f9f0836e2023dc2dff06e7a2a5186841f2f2f6bc12a2a1a2e05d7fa7a`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 10.8 MB (10841254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e950621bf55f9c03a0f91ce71347a56174670ad12c9a44c1674da2b52bfd8`  
		Last Modified: Thu, 14 May 2020 00:05:17 GMT  
		Size: 57.5 MB (57519348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:975b0a381b4dedd67a1cbbbe2ad1dc46258fc2e1fc624bee853861f57347a0cd
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122690436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb2a05ef7e12d078be5b8c888785c8dcf63ca751747e8adb3e7d44958c35126`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:49:44 GMT
ADD file:2c7c92015da849bc75eb25960609c90178c9ac455dab05aa4ef031806d26ad64 in / 
# Fri, 15 May 2020 04:49:45 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:41:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:41:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 14:42:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:567e61b8ab78e586542d5b9fab62c3880de99927de482a73e9e8b5b304f5284c`  
		Last Modified: Fri, 15 May 2020 04:59:15 GMT  
		Size: 50.1 MB (50149003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171157d3bf1886098a7c08bef7ab08c3c7a0d9b292111e8a5b8f39eecf07c2eb`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 7.5 MB (7460868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093eefc9c96bf46513b1575ab2e19b673a8a64043aca4e9ae4db05a4c7f3e803`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 10.5 MB (10484688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3ef87812e2dc9082a70deacd7c235df6ca129a598c7068a9e9847c0caf1ed`  
		Last Modified: Fri, 15 May 2020 14:55:49 GMT  
		Size: 54.6 MB (54595877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6603856837ae8bd32c4057b2ec5f209657dba52bbbd60ae56480bc34a1f36a51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135695157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dfc3b04a4138a6676612237e27482b41d159220cc62b24b536c0ddbef8c9e1e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:28:26 GMT
ADD file:7e16c349b13e97e4784ee396bb36ab2d3a069714388b0803f18ceb8d526be36a in / 
# Wed, 13 May 2020 22:28:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:55:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2aad5ee0ac7c9bdb0530f0a2f94bcadce58437453bcbdc7a2f20b5366c22799`  
		Last Modified: Wed, 13 May 2020 22:59:47 GMT  
		Size: 55.1 MB (55111830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb4a67eb9efabb0bee7a8a6ff0c8c5d8b09a6992b8574669e941eb06ffe22d`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 8.4 MB (8356775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba850bd6d1e4314d0d2953223c98e2452ff03935b42d421bbd2d54ca027da5f4`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 11.2 MB (11176751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc99aced2c3410b9c7fc622fe0d8acdcfb87cde0748b3dcf4eb683bbaabc75`  
		Last Modified: Thu, 14 May 2020 00:34:44 GMT  
		Size: 61.0 MB (61049801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8bf8a42687d1604bc5a72db85decba188c0b648ea1a7ac2b02b8b0cb6f22746a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122855450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ab3ebad11732cd4f9fe3e927ab9d5d2b3270a1ebdd3e429ac2aa866208e75`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:07:25 GMT
ADD file:e200f47e248587a66670fcf47316228d04373cff77498412eb3cc5d6a1ec50a5 in / 
# Thu, 14 May 2020 23:07:27 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:02:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 05:03:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11b5223327afa0d65cbb885c5383c894bdfd11269c346392cfb8a39f81aabaeb`  
		Last Modified: Thu, 14 May 2020 23:12:06 GMT  
		Size: 50.0 MB (50008939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcaa68d7c0d7853692ccebd673ff13ab4103a32fa894d7f1519715d3fb63578`  
		Last Modified: Fri, 15 May 2020 05:09:57 GMT  
		Size: 7.6 MB (7600688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112c6cf752bfa2d00b26e941e53dbde668d81bd2884edd4dd74954197be2a175`  
		Last Modified: Fri, 15 May 2020 05:10:04 GMT  
		Size: 10.3 MB (10347738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd846cd41672826db4f01851145be1859f34d6301450d3dc1dfd7266d159d2d`  
		Last Modified: Fri, 15 May 2020 05:10:19 GMT  
		Size: 54.9 MB (54898085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
