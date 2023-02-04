## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:55239bc48d86eebf8f44e70d5f3ccdb967b1d79da7b374fc1cb765536ccc731c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:70321b363637dbc4320f3bb51ac905e65e36dd96c31e41e20f0f6411ca1d63e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133838711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45b37b7d9279dd0cfbd276ce03eac95f0376c737373aebbefd6c40e81b32936`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:42 GMT
ADD file:a2e9c6618e31202c1b929d106d9d8f2e98a0d6a45ae13b56e9149536eee01769 in / 
# Sat, 04 Feb 2023 06:52:43 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9338402809c6c0e98dbcb30453239ee887fa0b3378ee26565d576b66c08dfdea`  
		Last Modified: Sat, 04 Feb 2023 06:57:50 GMT  
		Size: 49.0 MB (49039305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4000be28de3a086efcb096b84ff6947c42412ed2bc4e11f3ac254f7bd261ad9e`  
		Last Modified: Sat, 04 Feb 2023 07:31:34 GMT  
		Size: 9.0 MB (9033091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e133244bdf5da6e4b9014a53c5852a95e3d23591adc288ee97761ce0ae33b538`  
		Last Modified: Sat, 04 Feb 2023 07:31:34 GMT  
		Size: 11.4 MB (11354725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955bb19a4ed9a2c958bdbec5ad4f471b29d89c40ac19c0051083c5be93aef6c8`  
		Last Modified: Sat, 04 Feb 2023 07:31:52 GMT  
		Size: 64.4 MB (64411590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3af92d823beeb7f575953a76ccf83038aa5c955b3bdabd8fd8456b0639e77924
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129428472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:893af253446822b8d2371a7480f77b8de01b286a0c72053305c59c62887c0f3d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:53 GMT
ADD file:12eddccc39577b9f5e10835b6a2c5edd0b1a49ad547e20f5e2640f434b8d2a42 in / 
# Sat, 04 Feb 2023 02:46:54 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:18:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:19:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 03:19:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9756a18a5cc1d83f45eef500c448fdd88a17d9e9c99f86f02056851b6b5ac543`  
		Last Modified: Sat, 04 Feb 2023 02:52:12 GMT  
		Size: 48.0 MB (47996437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fe962304c3c3ba0027d920911fc9ab41a7242d7642f72fee189ed95174159`  
		Last Modified: Sat, 04 Feb 2023 03:24:35 GMT  
		Size: 8.5 MB (8481338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a388c264e9b4ce6fddf6a155cc927db77f824e38f9f65a6e0faa5dfb07c3e5`  
		Last Modified: Sat, 04 Feb 2023 03:24:35 GMT  
		Size: 11.0 MB (11002018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b439fe54160791a810e4bfd8992bb49028ed2ee80a4517801f46e4a7c279572`  
		Last Modified: Sat, 04 Feb 2023 03:24:59 GMT  
		Size: 61.9 MB (61948679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e379623d9248c267f168ff58be4b585f2a8f94c013ed47d4dbaaac65dcfdd31f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124149025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042415745dbe484a780b29df12cbde5d836933be264bb35a461fffd7d2a4f783`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:00:50 GMT
ADD file:3ef0e7784a31367bd6b8f62d72fd921e841a63c5f468870ca51cb13d32a10c98 in / 
# Sat, 04 Feb 2023 10:00:51 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 10:53:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ade7fb7e5df21b5001435afddae5270817c5e2a665e698f2b89244410fe9cf7`  
		Last Modified: Sat, 04 Feb 2023 10:08:21 GMT  
		Size: 45.8 MB (45796020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bceada3f9ea60690de207a1e9c70a03da888ace132ddf883dae8d5fca62d92`  
		Last Modified: Sat, 04 Feb 2023 11:01:34 GMT  
		Size: 8.1 MB (8124737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50080361018a99fea8d092caa292a14416ca537e3bd79c9f67230d9a7c08a73d`  
		Last Modified: Sat, 04 Feb 2023 11:01:34 GMT  
		Size: 10.6 MB (10635882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1ac5fa03f848c3a3f0164bddfc45d3737e41903e2bc94ce67d041a44b8f5b1`  
		Last Modified: Sat, 04 Feb 2023 11:01:56 GMT  
		Size: 59.6 MB (59592386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:17a5b66399180c169e6a670f9a5b75c224ff94f87c6615f7c130ff5ec13fd5aa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133555020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d21d87c759ea079ebd140b191777fe2e990f630c4bdc466017ffc9cfaf96c93`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:48:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:48:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 06:48:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6930bf2e2eda29b99cfe171c0422db365474b36931b359c0da6fff3dad52f8f6`  
		Last Modified: Sat, 04 Feb 2023 06:53:51 GMT  
		Size: 8.9 MB (8865606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d13ff72c8703f7d53521adcfd3a671f43824fbccadf8fa55bb396a67218577f`  
		Last Modified: Sat, 04 Feb 2023 06:53:52 GMT  
		Size: 11.3 MB (11319779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc660b3f704253e5469e3bda6b9ab48c6df752e652bcb111f62126d45a5249`  
		Last Modified: Sat, 04 Feb 2023 06:54:08 GMT  
		Size: 64.3 MB (64304684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:72d28bcc3ccd7168fb6d764ad86d33bfc419cff11ba2c38bde5ad4c815681109
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137157297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f68ba1267a8f99ef399c02daf1c7d0b1cf119ae2f650383968d562d0b2707`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:50:25 GMT
ADD file:e52d2501a6498b9d4b4b7c45345d2dd2f2fbfa7df2849d1f794768270c0971a5 in / 
# Sat, 04 Feb 2023 07:50:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:23:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 08:23:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc17d0499e93f237d6be86c3138e9cea4fd1d950920edfec3d640e8d8b6e6230`  
		Last Modified: Sat, 04 Feb 2023 07:56:51 GMT  
		Size: 50.1 MB (50095432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710c92d5b146f60cc687aee2f6d6a8c5c0a878fe515dedd23c774c10eb2ae049`  
		Last Modified: Sat, 04 Feb 2023 08:29:19 GMT  
		Size: 9.2 MB (9211457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1259464f51bb3a359b44d45da125dab6d573ba39303370fdb924ff37d221981`  
		Last Modified: Sat, 04 Feb 2023 08:29:19 GMT  
		Size: 11.6 MB (11557549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463be9d4d4182876e4e437db7d948625fe02b899c747e76701da314ad3014d41`  
		Last Modified: Sat, 04 Feb 2023 08:29:38 GMT  
		Size: 66.3 MB (66292859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89288224523428d3a56b2052f17f83f1f8330ecd9ca7b1cdacc0e31c815f821d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134118351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2741ff507ffc348b66d112b33b8423018178423789adcc18c631b5e02f4e5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:35:05 GMT
ADD file:a772415cec37230670450044a3962179f53657814c9c0e8bc6ef502ab4fff614 in / 
# Wed, 11 Jan 2023 16:35:12 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:30:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:31:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 17:33:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8fe537e863349284188081cc926e1cbc3d1d09a758c86969580374a79f6a9a0`  
		Last Modified: Wed, 11 Jan 2023 16:44:00 GMT  
		Size: 49.0 MB (49043063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48d22c89d2231b986e2d8e07b29039b4077a44f2ed6aac30212a0adc292871a`  
		Last Modified: Wed, 11 Jan 2023 17:46:11 GMT  
		Size: 8.4 MB (8400802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bf98ffebf3705900ffc4ce2bc2ee4d9f6f919564fdc57406d4df67e95f4b87`  
		Last Modified: Wed, 11 Jan 2023 17:46:12 GMT  
		Size: 11.1 MB (11104051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10eb2bd84dd13d143069e2a30d3ef34051906e3536c1f3ffba3448d9277fcc9`  
		Last Modified: Wed, 11 Jan 2023 17:47:06 GMT  
		Size: 65.6 MB (65570435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1215c360b72e8f812ef67fb7d38611a69da26d964d5e27477c84e4eb785fd9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.3 MB (147293439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5163d6265809108ec00b68c96e70ca3eacc70e2ff3d3c97731eb16405489076`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:50 GMT
ADD file:a8a466b916dd8b82163da9263cfb32eb757c2a0eb173228a5ac8ef05bdc55653 in / 
# Wed, 11 Jan 2023 03:49:53 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:17:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 07:18:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35c8c29d2bf600cd3a311b3649ac4076a0670c35cc296f1f28d2622bb6dd54d4`  
		Last Modified: Wed, 11 Jan 2023 03:56:03 GMT  
		Size: 53.1 MB (53077709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab0d63135d44be3ecac38d5206687b79632de571e5c05f58c0a49d13d4dd332`  
		Last Modified: Wed, 11 Jan 2023 07:27:41 GMT  
		Size: 9.6 MB (9615481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b2df2d7c9512f9de0ee08a692413dcbdbf53d56bc49fda25fae6cba32ce022`  
		Last Modified: Wed, 11 Jan 2023 07:27:41 GMT  
		Size: 12.1 MB (12115501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f811c7b48263d45bec77d7173793763f8b118007064bd7f81a3184c8353898`  
		Last Modified: Wed, 11 Jan 2023 07:28:11 GMT  
		Size: 72.5 MB (72484748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:80fe5d929462fbcb8fb502564ba1c94f3a1fb305aff0e201341b695be50f3fd5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122015209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3095c5914c0792da561d083de7026417fc5bec6e01a866d86b2f8f8d796eac27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:39:40 GMT
ADD file:cff1e1a432929527e9bb64bde53e2b614c941bd4631b7bd3634fdda8a7240455 in / 
# Wed, 05 Oct 2022 00:39:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:26:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cc6da93595cf4d9d589de999765cc4f1efa5e0d8e23ca6dd8b73b18afdc8189`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 48.9 MB (48857821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce58712f86101a4716baede25ee43c9c1fc550b39fb4b3e5fa1622fd3b00b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 8.4 MB (8388012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd132871253f925889ef836099addcf830644843a64a1529bddc510390846a9b`  
		Last Modified: Wed, 05 Oct 2022 03:30:22 GMT  
		Size: 10.8 MB (10750715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfc76b3f6f1ba447e697e6e2190cf70e757458cce81446b79426ae4cccdb03`  
		Last Modified: Wed, 05 Oct 2022 03:33:00 GMT  
		Size: 54.0 MB (54018661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:93e6874f52ee0b8b7145a5c3a0d471c4d3a990756cdacde674c0d71bb193fb50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130675897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e005d19f91a92824db317cf6042dc9cfc1c5aeaa2e9b232887747c6c25a8e73`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:27 GMT
ADD file:93877457106ba25112f38787099a736e27572cac3ea286b62bb0cea369e7334a in / 
# Sat, 04 Feb 2023 04:06:29 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 04:34:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eed18e15556323b9c6a0c2e3bb53a6d5526fb5398a405780091330bc1da9c2c`  
		Last Modified: Sat, 04 Feb 2023 04:10:42 GMT  
		Size: 47.4 MB (47408087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6536f8239e347252e1f3cdc22fe9df56c0b9215fefb3e2510b174579df58afed`  
		Last Modified: Sat, 04 Feb 2023 04:40:31 GMT  
		Size: 8.7 MB (8666333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade48b27fe2a94e7c854679e6f337da7e24a6cd38e0413e30ce13ff2eae0232`  
		Last Modified: Sat, 04 Feb 2023 04:40:31 GMT  
		Size: 11.2 MB (11218213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abf37075e0ca75d856b6855371078b6e53bd22bed4876382c2ecca1b0eb0f60`  
		Last Modified: Sat, 04 Feb 2023 04:40:47 GMT  
		Size: 63.4 MB (63383264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
