## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:3fb49365cba4d74083cb480597e51047a6f356345efc6538476b62d078215bfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03c440ab93f47f6f25a8234febc88184480f28020791200b902ad758cc4fc7fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84470558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823cef2ec1834c9343ac135b8763c224793328b28dd2afae1dad1a2da3016cac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6fcc5afd47847c2e97114df73dfbdb7cb98b3dba59c9d5e0460f5353e0ab2cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dc9111323484a0279e67f569d4cb21203c02f93aa3dcaa657dcc5ac889e26f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0e40d34528ab940355ef0e5c6e5a4331f9bb512e5e3104310ea9db74dc73d59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82728192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca32f751faa503b8fea9beef96876f4dbec6142b5dce0a0f3112fd89eb7c213c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f27c67b36f263760a8087131c54011ace3bd5d7db22c6529665d6abadf899e03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97492523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8b571049a41e25671a9c46d043cc1d74fe7567e153df521e45039f369392ac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:92d46888b25701d05c84398baa31995dd2f2f9cece8d00a6d36ae0b98b41ed12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75595398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a3029ed135684d6a7d55a4aa6663061bf0bddaaac730e68a265ebb4392da89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:946ba36daa4e4c0d9d38cda5253c2dfd87343e5523921f9a8f70978f0698ae7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89878914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e2cfd6247f86f57d874973213ecadf290768b88929aad3faf6c98c3ffda491`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
