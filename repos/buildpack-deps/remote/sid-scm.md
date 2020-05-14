## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:b3106e1e7a276371963e263b5a1fe0c560396dd27571147a6776b23209584e55
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
$ docker pull buildpack-deps@sha256:1856dca6a14251166d0d563a682db7bfbdd0511413c9885996b8e10e259587c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120325618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a621801a834d707768d2048ae37ac2d61987f1040fac0c2cb24290cd368f6cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:53:19 GMT
ADD file:b96a79161ef28394a61231962b6b094cc6d55101ffa9e159bca48da52498c02f in / 
# Wed, 13 May 2020 21:53:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:44:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e01d6f3a75b2bb37376867eda5418ce8818270da85f9e637bc0f8131b3c49c32`  
		Last Modified: Wed, 13 May 2020 22:01:43 GMT  
		Size: 49.4 MB (49359537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4060fe458be3ad9bb5734b9386b2be633e551438da5fa5933a3caf2eef1d3084`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 7.5 MB (7514215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e846164403fa17ac3349dfde468323e0107f2f131933333cec4baa962c230c`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 10.2 MB (10157674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3205e486be95e4ba1ae8b2d22f6ad94505d38726a1f4f4c6cef0287bcfc053`  
		Last Modified: Wed, 13 May 2020 22:58:38 GMT  
		Size: 53.3 MB (53294192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:708fd57b28ba49df720e05984372490e051aad6a2cbe7d5bc61edf87fd974b73
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115306055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a247ebf6c6e11c4a742937b2f00208afb44fb1b080cdd0cebfa1976c90c129`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:17:11 GMT
ADD file:5c1bf8e876f6ffb8a54374fd8f26d78a98dea1fae6787eb5fc225b65db262397 in / 
# Wed, 13 May 2020 21:17:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:06:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:07:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc0a6102c512ac7a18c58c8bfeb98c10b25edd28979b9a105af510e9c56fd786`  
		Last Modified: Wed, 13 May 2020 21:27:04 GMT  
		Size: 47.2 MB (47161205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f603ac474016e66e34904c06b4aec33100f42c805573cd91e60bfa44fff303c`  
		Last Modified: Thu, 14 May 2020 00:22:44 GMT  
		Size: 7.3 MB (7257035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd00f44c97780ed4c8b26dc3d2908006e596311de54a3c167ea77feaf1dc80a`  
		Last Modified: Thu, 14 May 2020 00:22:44 GMT  
		Size: 9.8 MB (9804644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c6fe09309e5999dadb8db8393a92e735426982776fa6a2cd5ce0589eab7f89`  
		Last Modified: Thu, 14 May 2020 00:23:07 GMT  
		Size: 51.1 MB (51083171 bytes)  
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
$ docker pull buildpack-deps@sha256:5275fdcc5bde224d1116f011698e6b3bb22f1f3f07eefd9258e33ef0d8868f27
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122673287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8921834060d190fce4842264cf2d61867991f69db00d47c93833f5082db87aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:50:21 GMT
ADD file:414f2e62e00cdfce0e28fe63b849f1edf12ec34ca7cfb09a08a2b45e2a5cbccf in / 
# Wed, 13 May 2020 22:50:22 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:01:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:01:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:02:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80f0b2fda6b50bded03a482e7f73f99daa6b715b932d0253f4c3054be1410241`  
		Last Modified: Wed, 13 May 2020 22:59:52 GMT  
		Size: 50.1 MB (50132193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc04cfdc11b752ee43412d0778b055107628b6cd534fb814336f68aab3c695f4`  
		Last Modified: Thu, 14 May 2020 00:19:44 GMT  
		Size: 7.5 MB (7460878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387d9d2e6037ae9b70690a8e4c4191c3d98d50f37419a122cf4cc9084fa2b873`  
		Last Modified: Thu, 14 May 2020 00:19:45 GMT  
		Size: 10.5 MB (10484731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab2877d4e519baee4968b25241b41ad05c0e80c36ab68b8baade630800fe0a5`  
		Last Modified: Thu, 14 May 2020 00:20:40 GMT  
		Size: 54.6 MB (54595485 bytes)  
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
$ docker pull buildpack-deps@sha256:627d77fb802fa50c5e03bcff10a5732fa83965d5c509a77e6def014682041fa5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122848692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823f552524fe2196e0bbe3c6cce298774bd4c51908cc824c5eae939314e768e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:22 GMT
ADD file:e7473e4f1acf1308ed319dfcc667696c733d4173125423a8f1b2c67039e5f498 in / 
# Wed, 13 May 2020 21:43:24 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:42:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:42:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23e07cfb1ab58da76b3f9f0fdc8f5c154643a262a86037b7b6d1c26b5959a166`  
		Last Modified: Wed, 13 May 2020 21:47:43 GMT  
		Size: 50.0 MB (50002084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e62641450b73095b82a741ceaf6d58012156b7f78bf4f67b73575fb15b7a03`  
		Last Modified: Wed, 13 May 2020 22:49:18 GMT  
		Size: 7.6 MB (7600546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f55d4f91dc718f22796b06fd0faf568f26113eb77e940c765216272c8262472`  
		Last Modified: Wed, 13 May 2020 22:49:24 GMT  
		Size: 10.3 MB (10347816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4524f47c96e9e169805caad967eaff45bbd160c819137b91ec0a64201132afa`  
		Last Modified: Wed, 13 May 2020 22:49:38 GMT  
		Size: 54.9 MB (54898246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
