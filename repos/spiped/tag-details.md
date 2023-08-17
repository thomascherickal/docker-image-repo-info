<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.2`](#spiped162)
-	[`spiped:1.6.2-alpine`](#spiped162-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:c42b9052f6a3081943ed261fadf5247b77cacceabc35c927eca7f7b12622d0e1
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:4f171c0f35b98776248253a67a50d37cccfd8473f07fb2695dde6d81ca2f139f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c704ab1e808854f06ff32f8281253ead1a6c81540e920fa3bb9a47349621c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:30:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 15:30:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:30:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 15:30:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 15:30:41 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 15:30:41 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 15:30:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 15:30:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f551bec805deb5c52468d55f52862d6fdac1441548dfe3b2dd6231bb13e35a9`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b935b31ab4b7796d274c3e3a3eb993798d9569355480bae3f11670c689b753d`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 2.6 MB (2586465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0425e3de531ea482e5effd29e0133c17f5d6210b2156d74dfb9c6d6a4e07864`  
		Last Modified: Wed, 16 Aug 2023 15:30:58 GMT  
		Size: 6.5 MB (6469487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802cd71544c6e0f12906f839800e76cbc6b05c24338da8b071db43a1d7ab7128`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c19c22c6f39515988c166c9dd995a108858c6d349fb731487be774bfffbfd`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3c7289266dfbfbfaab5924d86a6921ba5649eb1fbb89a61b70a374e4e4207130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd889b8582c22d497551a1ddbb7e3f468870196acda21ae9b4ccf81381905ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:32 GMT
ADD file:661e14e9730f2608fba590f84fbb357838a3068db018f1e0569c79035783c86d in / 
# Tue, 15 Aug 2023 23:48:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:32:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:32:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:32:40 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:32:40 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:32:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:32:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:32:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:46d4cdda07fa660f92a3251737b0b22ad71ebafb783af374930d636935a2d8eb`  
		Last Modified: Tue, 15 Aug 2023 23:51:34 GMT  
		Size: 27.0 MB (26983543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076403abf1d4e6fa2aabacbba757d8d2ac102ce57a1be34150e84ed466a1a60`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0d0f8f84a3e50c749376a9eb2403d724afc7be278a0138a504ee3be9f5ed38`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 2.2 MB (2184076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12251ef379190d727f05a79edfe62dc54784cba94545aa3bd6908f640b86391a`  
		Last Modified: Wed, 16 Aug 2023 00:32:53 GMT  
		Size: 5.1 MB (5136554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3b5689db6eca5fcdd32a4c46476d4d3e38ee1b6dfeed21e802e84bd344b130`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47adae998e8dc4db3b09a4235d7adb64c346db5d1fc2444d80b594d2a30a5`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5e8f0c26a16c4df76b2dc3fc6e710f79f928bc84e4ba1738ffb16a38d097769f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce26cf5793431ba1477cc81a099f7b8fec63f842df5a4d2ef708cfba02b37b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:12 GMT
ADD file:45cc27bd11f601d2fef5d7494a1a6253287e6d22e108e39c0884761c7533cd9c in / 
# Wed, 16 Aug 2023 00:17:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:25:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 05:25:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:25:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 05:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:25:51 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 05:25:51 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 05:25:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 05:25:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a44aa9565b062e4216f7b39ce6c67dcc5376e10f76caec55bd3acd1cc8b76b75`  
		Last Modified: Wed, 16 Aug 2023 00:21:27 GMT  
		Size: 24.8 MB (24805419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9c11d18979b89d7fa32eabe7f88a8cd64e01b4b8fa271fc334fb7d2b699b2`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b903a5c832d6f2fe4b495269a61fdf5cb49b36db7bea0569860fa6d84d00e`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 2.0 MB (2043310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f485e2da8130574c637c09ae0956f61e314214b2723b60575c9716e0f89ec`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 4.9 MB (4878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff0fe969b7330d3d7bb0cf4092f32ed845104416d60805fd202948a8404909`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25331bf9ce347281c7ed517293d861fd29f7d86535538cc031c9e9f3cfccbd97`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:64514be16b61c506ed4f38b7d901c8e2b309b08d76553ce403b891fce1180d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa77f5aed6d0831a3cc71c19adea277f0ccd481222fea6ba883c7f4865da198a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:20:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 10:20:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 10:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 10:20:30 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 10:20:30 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 10:20:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 10:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 10:20:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba019cbc445fbc18bd6dc20c125c8b39acf864a2824f00790582fa3560857391`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70188df993927106fe5ebbfd4c58f0d56ac94454c68dd496f6a7a61b5821602`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 2.4 MB (2429874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6b33daf23ff234e23662d0a02c051ef0e6151253ecaccf61b86ac6e8ea24f1`  
		Last Modified: Wed, 16 Aug 2023 10:20:46 GMT  
		Size: 5.5 MB (5478844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6b29684139d7512fa4b7ec02dbfd76c71952b4c482be6e6c368e4537d8af2c`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512d64842146daa84b8e6e4a582f3ec628fd10741650957d5aa95d22d9b874a`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c1269ae34205a7105e15e21afb748acf092303d42802e691703c620acdfe126e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9dccc0b103ac44995ceb2445bec61936130bb9cfa4d0b782e16ad93ff12327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 20:40:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 20:40:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 20:40:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 20:41:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 20:41:03 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 20:41:03 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 20:41:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 20:41:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 20:41:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03457c876b07f1c91adaf8fb6937472beeda4a93329a4ea034beddb49371b3a0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a2251fa8712a87ba72cf1b7210863ff8ffb1714aea584978ffb9257568d78`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 2.6 MB (2583561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea65716bab4c92cfb7167bcec8537472d71948f927537f09b9ba7430fe8177ec`  
		Last Modified: Wed, 16 Aug 2023 20:41:23 GMT  
		Size: 5.9 MB (5940186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7fe253882086312121ecd6331d5e7ccda72ef6ff2245bff10b4760a2211b6`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe62b93bfa24ccf2d27d2385608f70dcaed03bb85755b5e0d5b8967c58417b0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:9b4dbeeeabafa3af4b5285d65a9ee1b4666256018167363e939c2bbb17d24aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d6ea40c73469c69646f5a574fa790101c1a2efe663c9ab48893271c1d0b6468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:08:43 GMT
ADD file:6122efd66f4e010b48e48eeb243d900439ef783f5a10df76043546a288d35d38 in / 
# Wed, 16 Aug 2023 00:08:47 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 03:26:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 17 Aug 2023 03:26:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 03:26:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 17 Aug 2023 03:28:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Aug 2023 03:28:38 GMT
VOLUME [/spiped]
# Thu, 17 Aug 2023 03:28:40 GMT
WORKDIR /spiped
# Thu, 17 Aug 2023 03:28:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Aug 2023 03:28:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 03:28:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52390931db742e6fb36945aff79b92fea76dcfe0964f8a5cf7e5b5faaa40b80f`  
		Last Modified: Wed, 16 Aug 2023 00:19:34 GMT  
		Size: 29.1 MB (29121481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d455b5a855378e6a6a616a046e1fa07cfb625a604fd20ca1d37d52fda22174`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1badeb5ed503d07963318ac71660ae002cc2315591c20057b3c2c18811e128ba`  
		Last Modified: Thu, 17 Aug 2023 03:29:02 GMT  
		Size: 1.8 MB (1831704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acdbe213b6cb697af754286c587896d18df39349e4b4f26cb3eaaf0db9b0844`  
		Last Modified: Thu, 17 Aug 2023 03:29:06 GMT  
		Size: 5.8 MB (5801896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c09cc60cf7ce55c7cd74c75045171c3cd7a5cac4c3505dfee318d5cce1e9cd4`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee1deae900a5f4fdb29cdff7c2a89c3326fe9869b248c6a3943008517f9bfd8`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:cda509b294751f959f7764d1e1af011f4ce61c61e34eefbd25203a9ca0b28aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc441e69e8db9c2db390a467a61c87ec2e35d7a2a63c359e0e788615281064e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 15:42:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 15:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:43:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 15:44:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 15:44:05 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 15:44:05 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 15:44:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 15:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 15:44:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a39a8f321e61913bcebc5b10f2f4388ad008aed3aa0b7108c1c98aa672b8`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8637b8770fbcc45d233bc8c0685a004f863248524d9589bb8133462ad2ef98`  
		Last Modified: Fri, 28 Jul 2023 15:44:25 GMT  
		Size: 2.8 MB (2764991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e47b32eeb162a453e0f56b17945b85e59188dea37e5050beeb9fe549df43b6`  
		Last Modified: Fri, 28 Jul 2023 15:44:26 GMT  
		Size: 6.4 MB (6420314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6ad0fc910585043bd75c1f9f637776962532c3318497e750adf297becfa27a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe513cc6e981f0bcc9b41c0abcbebb0c975a964bdfc186524bcefd2f32b1496a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:84cf3b032ac9c98b0694f112d6543074edec69387196326c626d5110782d0ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5d933bb3ed3f1d38a0072fffbea977a9fe1a57bd15a21111ae268333636fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:31 GMT
ADD file:53543c10022986b61ebedef43821a8984443468fb85c225a6fa19c8d6c76f642 in / 
# Tue, 15 Aug 2023 23:42:34 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:45:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:45:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:46:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:46:04 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:46:04 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:46:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:46:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e165c0f9e8f698888061cd00c559fc4e4751505fa2e647bfbf5b2ff0dadafbd2`  
		Last Modified: Tue, 15 Aug 2023 23:47:53 GMT  
		Size: 27.5 MB (27489761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50f6cb6aee208293ff4de3faa6f922cf494871a4a2ae5ebc8039c13654c91e1`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed3495d001827fc24354a561db0b089a3283e04251e6535cc584a8702f4226`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 2.3 MB (2257969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc14100c7e65bef730a13ebbcb8ef00d75512dc4ec87b42522271b05f9bf366`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 5.4 MB (5383391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8459fd8ee0a7b197fc673352f85d0bf6e064636852130e18170b42e410c47d0b`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b957665d1c4ddc4ea206ff316da27c25d911ed700608ac92f22de1db04bac1f`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:9e0a090f395df640e73bdda9b2387d3fbadf14c6cb5d789c43f1da21368acb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:49da7ccf4fd259700f2ac1db19a287d31a9ecf3a44e405470bf84179e4a151db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0439a8b1da8e9de36492d0a058f2acbdbfba92eb2bb87d48f767e0a31237098`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:03:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:03:24 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:03:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:03:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:03:34 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:03:34 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:03:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:03:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158fd3e69013bf879861985939c5aac2cbc46278db264aeae05ee1344222b07`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfba2e005bb6d82f820494ca9e65f63ae7042f6d1e2b54a8c6784c76b725a9d`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118bcda9b744a84a9c764eadd2a58bd39cba589942a2f8f7c6489d77a0f2d9a`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 221.3 KB (221274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76e498c240a7f12cb65ca8ed5d392aa245b449c370b5f77cc48781b7b0fe2e0`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd21f5dcda92cc1313530a1f07e075d96091d58e595b5ab77b810ff6b80125`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:92c72514aab4032a46bd337535d95862b853d6c7e90cb1e86e689409cc93616f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4589191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3dd418f5fe3e7be9bbb2632a3fd0fbbedad7f67e01d907d0d41c06bb6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:07 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:36:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:36:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:36:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:36:17 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:36:17 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:36:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ffd38f9a9109fd6f2d98e59fac671a21acbcbd826d953a190916b8e28c4d7c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafe31ddd32f93d6462563149d47e652289246cae76c3d69e2ae22c7f2dc157`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.2 MB (1236777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711c8b1ac9af3a0357e5e2ae10175a62c27bdea58e2e79fb7d413e2fa3a10138`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2f76630a196bedcec1d4f1f0542336e3189757e62aa7c83bd7f7e8f58680c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f674889b446c00cdd7da82689ee81ea78c84e02c462ad671bf3f9afd926afb1`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6b4ce7a3a962f7016da46f810228189be1cd6de1de0409f784505adca9fee42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4264646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f8b18499e87820bcff1593b1ccee12dbf54a9a32e6f7412af5d5c00268ce73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:51:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 21:51:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 21:51:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 21:51:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 21:51:52 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 21:51:52 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 21:51:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 21:51:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd254e37c3835d8a90d159f62497146fa2c0a51539455baafa4b5f3ad94073a`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87a0e27917b2f49aabe18b41a38f10f52561eaed9cd75ecbf9bb54dd5ad657`  
		Last Modified: Tue, 08 Aug 2023 21:52:10 GMT  
		Size: 1.2 MB (1163899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3f71f875284eede5e8bb82a4d0706d42594a0fec380b98dd516f0f75ed88`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 199.5 KB (199532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0eec6ac7d1270176b9ec72709b3186f9c9af79d5c747bdd03ac4818437e4b9`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da618866e96da51da8e7f96815a2d1e87198583082d2e819eaea328e7698149`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dfe860acf255915c9dcaae09dee878429e2b4c60798c048d82792352553d097d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4910891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9eb2d7445a05df9d201e84087d63696ade07ba940606d9e9deff249fd99f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:24:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:24:56 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:24:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:25:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:25:03 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:25:03 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:25:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa528de18ca9d8d7a81ae0d2ae78e694dca22d0e57c1adfd51230a5e72d602e`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4370e4fd5a67983765277bfaecb212d7f59e20db8264e69a6addca35b95526`  
		Last Modified: Wed, 09 Aug 2023 04:25:16 GMT  
		Size: 1.4 MB (1362701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605f0c15e8832deb396dd75011d9b8192e38e7b774733cea490c48a6c601da8`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 215.7 KB (215688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261765f25ad95a25543e0e6a6027cde75c58f6d3ceff188b0603ddcac15e32dd`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777264984131985e8771b4c25137123bf218b95e4de8ca97a58fe188f07340e6`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:3b9156620133e8bd472e78fcdc63367c0bd8ce4728e9b37100cecab16f9ba20b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4822397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ba2e93561dabc36ed836ecddc93cde747f6c0533764e243a1059c63a1ea4f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:25:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 22:25:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 22:25:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 22:25:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 22:25:30 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 22:25:30 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 22:25:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:25:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c31dcd775c39ea60679a161fbb3ec0114ed4a665986290232a4978c9b6a4e`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d724475632ebc1a22d1c3ca248315c7f4e6f7c5296f4eae98f587b0b3d246cb8`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.4 MB (1353881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a4abf10ff23af34214cad41a3ae8c5d722d0e578c719b02dcc3b303fa33ba`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 231.6 KB (231630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efbd75e8157b70348066566d4008a9c0bada288c04ada82ba412b78dc02e0c`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b78bd941b6d435a0daeb98222178fc6fdbd36c9b3cf1c59533e4bb87eb77b`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:b970c43232a9d83311742cddc2169c379db8304ab7409d9da95ff993ac82fbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4929752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45510f2b3a9a17d1bb74f84ca2abab8ed1061dff0e55839a3e8754e2c3290639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:49:46 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:50:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:50:03 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:50:04 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc475aa02ec0250350b4a331524b0a1e029de0aa51afc8d13cde5114f9a38f3`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64752c695a009aa97f4b6b21ee3618c0e6a15c1ccff9682ad7b50a01c411c09a`  
		Last Modified: Tue, 08 Aug 2023 23:50:27 GMT  
		Size: 1.4 MB (1361737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6958824bc296d0ee662dc09b65827f4c19cf6d08b0bc88c29c0aac7daef4b`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 220.0 KB (220022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbe94a7a7ea3e66fec66bafea8a8825cb0e1e4d4e13a6dd126caa55abc4368d`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d36cfcde9b1ab7cc6cd3e055bd3be46da17fbb42fd44094957dc575cb2aef`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7a35ce80545ef01185c3169716056ca5ee9520f1581c67074f5bd685d4f12ef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4646060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6af800db14443eb1061db4d4abf6affd33538028addd00c5cd1c46f9cbb00c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:16:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:16:02 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:16:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:16:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:16:08 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:16:08 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:16:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c947b711155cc9344e62be76da2fecb7e905aca9dad8fc53f2cb638fe84aa6`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705178608b8d1386cffd5a0ae5a7f41f2e6f580e6fb623ad053b6f8210fef7b1`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.2 MB (1221485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daaf6c162e1789b8a3c771759f74ad7c9ef9d19c7b7b614f9bea92f6f181874`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 208.6 KB (208644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9625b69d1551e16c0e8f95bc6eb00c95fbff0b0343391700336a2adb0752`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c787e2ceba069513a1f75d40922510e58442a2924c5668f7cefd24fff1c7`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:c42b9052f6a3081943ed261fadf5247b77cacceabc35c927eca7f7b12622d0e1
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:4f171c0f35b98776248253a67a50d37cccfd8473f07fb2695dde6d81ca2f139f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c704ab1e808854f06ff32f8281253ead1a6c81540e920fa3bb9a47349621c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:30:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 15:30:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:30:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 15:30:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 15:30:41 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 15:30:41 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 15:30:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 15:30:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f551bec805deb5c52468d55f52862d6fdac1441548dfe3b2dd6231bb13e35a9`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b935b31ab4b7796d274c3e3a3eb993798d9569355480bae3f11670c689b753d`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 2.6 MB (2586465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0425e3de531ea482e5effd29e0133c17f5d6210b2156d74dfb9c6d6a4e07864`  
		Last Modified: Wed, 16 Aug 2023 15:30:58 GMT  
		Size: 6.5 MB (6469487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802cd71544c6e0f12906f839800e76cbc6b05c24338da8b071db43a1d7ab7128`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c19c22c6f39515988c166c9dd995a108858c6d349fb731487be774bfffbfd`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3c7289266dfbfbfaab5924d86a6921ba5649eb1fbb89a61b70a374e4e4207130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd889b8582c22d497551a1ddbb7e3f468870196acda21ae9b4ccf81381905ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:32 GMT
ADD file:661e14e9730f2608fba590f84fbb357838a3068db018f1e0569c79035783c86d in / 
# Tue, 15 Aug 2023 23:48:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:32:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:32:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:32:40 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:32:40 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:32:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:32:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:32:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:46d4cdda07fa660f92a3251737b0b22ad71ebafb783af374930d636935a2d8eb`  
		Last Modified: Tue, 15 Aug 2023 23:51:34 GMT  
		Size: 27.0 MB (26983543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076403abf1d4e6fa2aabacbba757d8d2ac102ce57a1be34150e84ed466a1a60`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0d0f8f84a3e50c749376a9eb2403d724afc7be278a0138a504ee3be9f5ed38`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 2.2 MB (2184076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12251ef379190d727f05a79edfe62dc54784cba94545aa3bd6908f640b86391a`  
		Last Modified: Wed, 16 Aug 2023 00:32:53 GMT  
		Size: 5.1 MB (5136554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3b5689db6eca5fcdd32a4c46476d4d3e38ee1b6dfeed21e802e84bd344b130`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47adae998e8dc4db3b09a4235d7adb64c346db5d1fc2444d80b594d2a30a5`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5e8f0c26a16c4df76b2dc3fc6e710f79f928bc84e4ba1738ffb16a38d097769f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce26cf5793431ba1477cc81a099f7b8fec63f842df5a4d2ef708cfba02b37b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:12 GMT
ADD file:45cc27bd11f601d2fef5d7494a1a6253287e6d22e108e39c0884761c7533cd9c in / 
# Wed, 16 Aug 2023 00:17:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:25:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 05:25:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:25:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 05:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:25:51 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 05:25:51 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 05:25:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 05:25:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a44aa9565b062e4216f7b39ce6c67dcc5376e10f76caec55bd3acd1cc8b76b75`  
		Last Modified: Wed, 16 Aug 2023 00:21:27 GMT  
		Size: 24.8 MB (24805419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9c11d18979b89d7fa32eabe7f88a8cd64e01b4b8fa271fc334fb7d2b699b2`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b903a5c832d6f2fe4b495269a61fdf5cb49b36db7bea0569860fa6d84d00e`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 2.0 MB (2043310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f485e2da8130574c637c09ae0956f61e314214b2723b60575c9716e0f89ec`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 4.9 MB (4878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff0fe969b7330d3d7bb0cf4092f32ed845104416d60805fd202948a8404909`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25331bf9ce347281c7ed517293d861fd29f7d86535538cc031c9e9f3cfccbd97`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:64514be16b61c506ed4f38b7d901c8e2b309b08d76553ce403b891fce1180d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa77f5aed6d0831a3cc71c19adea277f0ccd481222fea6ba883c7f4865da198a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:20:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 10:20:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 10:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 10:20:30 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 10:20:30 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 10:20:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 10:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 10:20:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba019cbc445fbc18bd6dc20c125c8b39acf864a2824f00790582fa3560857391`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70188df993927106fe5ebbfd4c58f0d56ac94454c68dd496f6a7a61b5821602`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 2.4 MB (2429874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6b33daf23ff234e23662d0a02c051ef0e6151253ecaccf61b86ac6e8ea24f1`  
		Last Modified: Wed, 16 Aug 2023 10:20:46 GMT  
		Size: 5.5 MB (5478844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6b29684139d7512fa4b7ec02dbfd76c71952b4c482be6e6c368e4537d8af2c`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512d64842146daa84b8e6e4a582f3ec628fd10741650957d5aa95d22d9b874a`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c1269ae34205a7105e15e21afb748acf092303d42802e691703c620acdfe126e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9dccc0b103ac44995ceb2445bec61936130bb9cfa4d0b782e16ad93ff12327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 20:40:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 20:40:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 20:40:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 20:41:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 20:41:03 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 20:41:03 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 20:41:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 20:41:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 20:41:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03457c876b07f1c91adaf8fb6937472beeda4a93329a4ea034beddb49371b3a0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a2251fa8712a87ba72cf1b7210863ff8ffb1714aea584978ffb9257568d78`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 2.6 MB (2583561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea65716bab4c92cfb7167bcec8537472d71948f927537f09b9ba7430fe8177ec`  
		Last Modified: Wed, 16 Aug 2023 20:41:23 GMT  
		Size: 5.9 MB (5940186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7fe253882086312121ecd6331d5e7ccda72ef6ff2245bff10b4760a2211b6`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe62b93bfa24ccf2d27d2385608f70dcaed03bb85755b5e0d5b8967c58417b0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:9b4dbeeeabafa3af4b5285d65a9ee1b4666256018167363e939c2bbb17d24aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d6ea40c73469c69646f5a574fa790101c1a2efe663c9ab48893271c1d0b6468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:08:43 GMT
ADD file:6122efd66f4e010b48e48eeb243d900439ef783f5a10df76043546a288d35d38 in / 
# Wed, 16 Aug 2023 00:08:47 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 03:26:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 17 Aug 2023 03:26:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 03:26:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 17 Aug 2023 03:28:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Aug 2023 03:28:38 GMT
VOLUME [/spiped]
# Thu, 17 Aug 2023 03:28:40 GMT
WORKDIR /spiped
# Thu, 17 Aug 2023 03:28:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Aug 2023 03:28:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 03:28:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52390931db742e6fb36945aff79b92fea76dcfe0964f8a5cf7e5b5faaa40b80f`  
		Last Modified: Wed, 16 Aug 2023 00:19:34 GMT  
		Size: 29.1 MB (29121481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d455b5a855378e6a6a616a046e1fa07cfb625a604fd20ca1d37d52fda22174`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1badeb5ed503d07963318ac71660ae002cc2315591c20057b3c2c18811e128ba`  
		Last Modified: Thu, 17 Aug 2023 03:29:02 GMT  
		Size: 1.8 MB (1831704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acdbe213b6cb697af754286c587896d18df39349e4b4f26cb3eaaf0db9b0844`  
		Last Modified: Thu, 17 Aug 2023 03:29:06 GMT  
		Size: 5.8 MB (5801896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c09cc60cf7ce55c7cd74c75045171c3cd7a5cac4c3505dfee318d5cce1e9cd4`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee1deae900a5f4fdb29cdff7c2a89c3326fe9869b248c6a3943008517f9bfd8`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:cda509b294751f959f7764d1e1af011f4ce61c61e34eefbd25203a9ca0b28aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc441e69e8db9c2db390a467a61c87ec2e35d7a2a63c359e0e788615281064e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 15:42:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 15:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:43:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 15:44:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 15:44:05 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 15:44:05 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 15:44:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 15:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 15:44:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a39a8f321e61913bcebc5b10f2f4388ad008aed3aa0b7108c1c98aa672b8`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8637b8770fbcc45d233bc8c0685a004f863248524d9589bb8133462ad2ef98`  
		Last Modified: Fri, 28 Jul 2023 15:44:25 GMT  
		Size: 2.8 MB (2764991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e47b32eeb162a453e0f56b17945b85e59188dea37e5050beeb9fe549df43b6`  
		Last Modified: Fri, 28 Jul 2023 15:44:26 GMT  
		Size: 6.4 MB (6420314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6ad0fc910585043bd75c1f9f637776962532c3318497e750adf297becfa27a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe513cc6e981f0bcc9b41c0abcbebb0c975a964bdfc186524bcefd2f32b1496a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:84cf3b032ac9c98b0694f112d6543074edec69387196326c626d5110782d0ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5d933bb3ed3f1d38a0072fffbea977a9fe1a57bd15a21111ae268333636fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:31 GMT
ADD file:53543c10022986b61ebedef43821a8984443468fb85c225a6fa19c8d6c76f642 in / 
# Tue, 15 Aug 2023 23:42:34 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:45:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:45:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:46:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:46:04 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:46:04 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:46:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:46:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e165c0f9e8f698888061cd00c559fc4e4751505fa2e647bfbf5b2ff0dadafbd2`  
		Last Modified: Tue, 15 Aug 2023 23:47:53 GMT  
		Size: 27.5 MB (27489761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50f6cb6aee208293ff4de3faa6f922cf494871a4a2ae5ebc8039c13654c91e1`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed3495d001827fc24354a561db0b089a3283e04251e6535cc584a8702f4226`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 2.3 MB (2257969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc14100c7e65bef730a13ebbcb8ef00d75512dc4ec87b42522271b05f9bf366`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 5.4 MB (5383391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8459fd8ee0a7b197fc673352f85d0bf6e064636852130e18170b42e410c47d0b`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b957665d1c4ddc4ea206ff316da27c25d911ed700608ac92f22de1db04bac1f`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:9e0a090f395df640e73bdda9b2387d3fbadf14c6cb5d789c43f1da21368acb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:49da7ccf4fd259700f2ac1db19a287d31a9ecf3a44e405470bf84179e4a151db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0439a8b1da8e9de36492d0a058f2acbdbfba92eb2bb87d48f767e0a31237098`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:03:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:03:24 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:03:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:03:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:03:34 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:03:34 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:03:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:03:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158fd3e69013bf879861985939c5aac2cbc46278db264aeae05ee1344222b07`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfba2e005bb6d82f820494ca9e65f63ae7042f6d1e2b54a8c6784c76b725a9d`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118bcda9b744a84a9c764eadd2a58bd39cba589942a2f8f7c6489d77a0f2d9a`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 221.3 KB (221274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76e498c240a7f12cb65ca8ed5d392aa245b449c370b5f77cc48781b7b0fe2e0`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd21f5dcda92cc1313530a1f07e075d96091d58e595b5ab77b810ff6b80125`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:92c72514aab4032a46bd337535d95862b853d6c7e90cb1e86e689409cc93616f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4589191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3dd418f5fe3e7be9bbb2632a3fd0fbbedad7f67e01d907d0d41c06bb6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:07 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:36:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:36:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:36:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:36:17 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:36:17 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:36:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ffd38f9a9109fd6f2d98e59fac671a21acbcbd826d953a190916b8e28c4d7c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafe31ddd32f93d6462563149d47e652289246cae76c3d69e2ae22c7f2dc157`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.2 MB (1236777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711c8b1ac9af3a0357e5e2ae10175a62c27bdea58e2e79fb7d413e2fa3a10138`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2f76630a196bedcec1d4f1f0542336e3189757e62aa7c83bd7f7e8f58680c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f674889b446c00cdd7da82689ee81ea78c84e02c462ad671bf3f9afd926afb1`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6b4ce7a3a962f7016da46f810228189be1cd6de1de0409f784505adca9fee42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4264646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f8b18499e87820bcff1593b1ccee12dbf54a9a32e6f7412af5d5c00268ce73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:51:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 21:51:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 21:51:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 21:51:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 21:51:52 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 21:51:52 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 21:51:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 21:51:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd254e37c3835d8a90d159f62497146fa2c0a51539455baafa4b5f3ad94073a`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87a0e27917b2f49aabe18b41a38f10f52561eaed9cd75ecbf9bb54dd5ad657`  
		Last Modified: Tue, 08 Aug 2023 21:52:10 GMT  
		Size: 1.2 MB (1163899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3f71f875284eede5e8bb82a4d0706d42594a0fec380b98dd516f0f75ed88`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 199.5 KB (199532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0eec6ac7d1270176b9ec72709b3186f9c9af79d5c747bdd03ac4818437e4b9`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da618866e96da51da8e7f96815a2d1e87198583082d2e819eaea328e7698149`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dfe860acf255915c9dcaae09dee878429e2b4c60798c048d82792352553d097d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4910891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9eb2d7445a05df9d201e84087d63696ade07ba940606d9e9deff249fd99f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:24:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:24:56 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:24:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:25:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:25:03 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:25:03 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:25:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa528de18ca9d8d7a81ae0d2ae78e694dca22d0e57c1adfd51230a5e72d602e`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4370e4fd5a67983765277bfaecb212d7f59e20db8264e69a6addca35b95526`  
		Last Modified: Wed, 09 Aug 2023 04:25:16 GMT  
		Size: 1.4 MB (1362701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605f0c15e8832deb396dd75011d9b8192e38e7b774733cea490c48a6c601da8`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 215.7 KB (215688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261765f25ad95a25543e0e6a6027cde75c58f6d3ceff188b0603ddcac15e32dd`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777264984131985e8771b4c25137123bf218b95e4de8ca97a58fe188f07340e6`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:3b9156620133e8bd472e78fcdc63367c0bd8ce4728e9b37100cecab16f9ba20b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4822397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ba2e93561dabc36ed836ecddc93cde747f6c0533764e243a1059c63a1ea4f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:25:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 22:25:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 22:25:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 22:25:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 22:25:30 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 22:25:30 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 22:25:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:25:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c31dcd775c39ea60679a161fbb3ec0114ed4a665986290232a4978c9b6a4e`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d724475632ebc1a22d1c3ca248315c7f4e6f7c5296f4eae98f587b0b3d246cb8`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.4 MB (1353881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a4abf10ff23af34214cad41a3ae8c5d722d0e578c719b02dcc3b303fa33ba`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 231.6 KB (231630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efbd75e8157b70348066566d4008a9c0bada288c04ada82ba412b78dc02e0c`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b78bd941b6d435a0daeb98222178fc6fdbd36c9b3cf1c59533e4bb87eb77b`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:b970c43232a9d83311742cddc2169c379db8304ab7409d9da95ff993ac82fbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4929752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45510f2b3a9a17d1bb74f84ca2abab8ed1061dff0e55839a3e8754e2c3290639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:49:46 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:50:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:50:03 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:50:04 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc475aa02ec0250350b4a331524b0a1e029de0aa51afc8d13cde5114f9a38f3`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64752c695a009aa97f4b6b21ee3618c0e6a15c1ccff9682ad7b50a01c411c09a`  
		Last Modified: Tue, 08 Aug 2023 23:50:27 GMT  
		Size: 1.4 MB (1361737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6958824bc296d0ee662dc09b65827f4c19cf6d08b0bc88c29c0aac7daef4b`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 220.0 KB (220022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbe94a7a7ea3e66fec66bafea8a8825cb0e1e4d4e13a6dd126caa55abc4368d`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d36cfcde9b1ab7cc6cd3e055bd3be46da17fbb42fd44094957dc575cb2aef`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7a35ce80545ef01185c3169716056ca5ee9520f1581c67074f5bd685d4f12ef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4646060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6af800db14443eb1061db4d4abf6affd33538028addd00c5cd1c46f9cbb00c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:16:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:16:02 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:16:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:16:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:16:08 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:16:08 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:16:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c947b711155cc9344e62be76da2fecb7e905aca9dad8fc53f2cb638fe84aa6`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705178608b8d1386cffd5a0ae5a7f41f2e6f580e6fb623ad053b6f8210fef7b1`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.2 MB (1221485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daaf6c162e1789b8a3c771759f74ad7c9ef9d19c7b7b614f9bea92f6f181874`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 208.6 KB (208644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9625b69d1551e16c0e8f95bc6eb00c95fbff0b0343391700336a2adb0752`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c787e2ceba069513a1f75d40922510e58442a2924c5668f7cefd24fff1c7`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:c42b9052f6a3081943ed261fadf5247b77cacceabc35c927eca7f7b12622d0e1
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

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:4f171c0f35b98776248253a67a50d37cccfd8473f07fb2695dde6d81ca2f139f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c704ab1e808854f06ff32f8281253ead1a6c81540e920fa3bb9a47349621c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:30:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 15:30:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:30:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 15:30:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 15:30:41 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 15:30:41 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 15:30:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 15:30:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f551bec805deb5c52468d55f52862d6fdac1441548dfe3b2dd6231bb13e35a9`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b935b31ab4b7796d274c3e3a3eb993798d9569355480bae3f11670c689b753d`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 2.6 MB (2586465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0425e3de531ea482e5effd29e0133c17f5d6210b2156d74dfb9c6d6a4e07864`  
		Last Modified: Wed, 16 Aug 2023 15:30:58 GMT  
		Size: 6.5 MB (6469487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802cd71544c6e0f12906f839800e76cbc6b05c24338da8b071db43a1d7ab7128`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c19c22c6f39515988c166c9dd995a108858c6d349fb731487be774bfffbfd`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3c7289266dfbfbfaab5924d86a6921ba5649eb1fbb89a61b70a374e4e4207130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd889b8582c22d497551a1ddbb7e3f468870196acda21ae9b4ccf81381905ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:32 GMT
ADD file:661e14e9730f2608fba590f84fbb357838a3068db018f1e0569c79035783c86d in / 
# Tue, 15 Aug 2023 23:48:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:32:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:32:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:32:40 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:32:40 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:32:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:32:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:32:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:46d4cdda07fa660f92a3251737b0b22ad71ebafb783af374930d636935a2d8eb`  
		Last Modified: Tue, 15 Aug 2023 23:51:34 GMT  
		Size: 27.0 MB (26983543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076403abf1d4e6fa2aabacbba757d8d2ac102ce57a1be34150e84ed466a1a60`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0d0f8f84a3e50c749376a9eb2403d724afc7be278a0138a504ee3be9f5ed38`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 2.2 MB (2184076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12251ef379190d727f05a79edfe62dc54784cba94545aa3bd6908f640b86391a`  
		Last Modified: Wed, 16 Aug 2023 00:32:53 GMT  
		Size: 5.1 MB (5136554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3b5689db6eca5fcdd32a4c46476d4d3e38ee1b6dfeed21e802e84bd344b130`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47adae998e8dc4db3b09a4235d7adb64c346db5d1fc2444d80b594d2a30a5`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5e8f0c26a16c4df76b2dc3fc6e710f79f928bc84e4ba1738ffb16a38d097769f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce26cf5793431ba1477cc81a099f7b8fec63f842df5a4d2ef708cfba02b37b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:12 GMT
ADD file:45cc27bd11f601d2fef5d7494a1a6253287e6d22e108e39c0884761c7533cd9c in / 
# Wed, 16 Aug 2023 00:17:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:25:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 05:25:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:25:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 05:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:25:51 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 05:25:51 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 05:25:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 05:25:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a44aa9565b062e4216f7b39ce6c67dcc5376e10f76caec55bd3acd1cc8b76b75`  
		Last Modified: Wed, 16 Aug 2023 00:21:27 GMT  
		Size: 24.8 MB (24805419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9c11d18979b89d7fa32eabe7f88a8cd64e01b4b8fa271fc334fb7d2b699b2`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b903a5c832d6f2fe4b495269a61fdf5cb49b36db7bea0569860fa6d84d00e`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 2.0 MB (2043310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f485e2da8130574c637c09ae0956f61e314214b2723b60575c9716e0f89ec`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 4.9 MB (4878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff0fe969b7330d3d7bb0cf4092f32ed845104416d60805fd202948a8404909`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25331bf9ce347281c7ed517293d861fd29f7d86535538cc031c9e9f3cfccbd97`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:64514be16b61c506ed4f38b7d901c8e2b309b08d76553ce403b891fce1180d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa77f5aed6d0831a3cc71c19adea277f0ccd481222fea6ba883c7f4865da198a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:20:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 10:20:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 10:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 10:20:30 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 10:20:30 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 10:20:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 10:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 10:20:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba019cbc445fbc18bd6dc20c125c8b39acf864a2824f00790582fa3560857391`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70188df993927106fe5ebbfd4c58f0d56ac94454c68dd496f6a7a61b5821602`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 2.4 MB (2429874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6b33daf23ff234e23662d0a02c051ef0e6151253ecaccf61b86ac6e8ea24f1`  
		Last Modified: Wed, 16 Aug 2023 10:20:46 GMT  
		Size: 5.5 MB (5478844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6b29684139d7512fa4b7ec02dbfd76c71952b4c482be6e6c368e4537d8af2c`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512d64842146daa84b8e6e4a582f3ec628fd10741650957d5aa95d22d9b874a`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:c1269ae34205a7105e15e21afb748acf092303d42802e691703c620acdfe126e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9dccc0b103ac44995ceb2445bec61936130bb9cfa4d0b782e16ad93ff12327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 20:40:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 20:40:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 20:40:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 20:41:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 20:41:03 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 20:41:03 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 20:41:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 20:41:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 20:41:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03457c876b07f1c91adaf8fb6937472beeda4a93329a4ea034beddb49371b3a0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a2251fa8712a87ba72cf1b7210863ff8ffb1714aea584978ffb9257568d78`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 2.6 MB (2583561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea65716bab4c92cfb7167bcec8537472d71948f927537f09b9ba7430fe8177ec`  
		Last Modified: Wed, 16 Aug 2023 20:41:23 GMT  
		Size: 5.9 MB (5940186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7fe253882086312121ecd6331d5e7ccda72ef6ff2245bff10b4760a2211b6`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe62b93bfa24ccf2d27d2385608f70dcaed03bb85755b5e0d5b8967c58417b0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:9b4dbeeeabafa3af4b5285d65a9ee1b4666256018167363e939c2bbb17d24aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d6ea40c73469c69646f5a574fa790101c1a2efe663c9ab48893271c1d0b6468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:08:43 GMT
ADD file:6122efd66f4e010b48e48eeb243d900439ef783f5a10df76043546a288d35d38 in / 
# Wed, 16 Aug 2023 00:08:47 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 03:26:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 17 Aug 2023 03:26:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 03:26:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 17 Aug 2023 03:28:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Aug 2023 03:28:38 GMT
VOLUME [/spiped]
# Thu, 17 Aug 2023 03:28:40 GMT
WORKDIR /spiped
# Thu, 17 Aug 2023 03:28:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Aug 2023 03:28:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 03:28:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52390931db742e6fb36945aff79b92fea76dcfe0964f8a5cf7e5b5faaa40b80f`  
		Last Modified: Wed, 16 Aug 2023 00:19:34 GMT  
		Size: 29.1 MB (29121481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d455b5a855378e6a6a616a046e1fa07cfb625a604fd20ca1d37d52fda22174`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1badeb5ed503d07963318ac71660ae002cc2315591c20057b3c2c18811e128ba`  
		Last Modified: Thu, 17 Aug 2023 03:29:02 GMT  
		Size: 1.8 MB (1831704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acdbe213b6cb697af754286c587896d18df39349e4b4f26cb3eaaf0db9b0844`  
		Last Modified: Thu, 17 Aug 2023 03:29:06 GMT  
		Size: 5.8 MB (5801896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c09cc60cf7ce55c7cd74c75045171c3cd7a5cac4c3505dfee318d5cce1e9cd4`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee1deae900a5f4fdb29cdff7c2a89c3326fe9869b248c6a3943008517f9bfd8`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:cda509b294751f959f7764d1e1af011f4ce61c61e34eefbd25203a9ca0b28aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc441e69e8db9c2db390a467a61c87ec2e35d7a2a63c359e0e788615281064e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 15:42:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 15:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:43:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 15:44:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 15:44:05 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 15:44:05 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 15:44:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 15:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 15:44:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a39a8f321e61913bcebc5b10f2f4388ad008aed3aa0b7108c1c98aa672b8`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8637b8770fbcc45d233bc8c0685a004f863248524d9589bb8133462ad2ef98`  
		Last Modified: Fri, 28 Jul 2023 15:44:25 GMT  
		Size: 2.8 MB (2764991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e47b32eeb162a453e0f56b17945b85e59188dea37e5050beeb9fe549df43b6`  
		Last Modified: Fri, 28 Jul 2023 15:44:26 GMT  
		Size: 6.4 MB (6420314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6ad0fc910585043bd75c1f9f637776962532c3318497e750adf297becfa27a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe513cc6e981f0bcc9b41c0abcbebb0c975a964bdfc186524bcefd2f32b1496a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:84cf3b032ac9c98b0694f112d6543074edec69387196326c626d5110782d0ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5d933bb3ed3f1d38a0072fffbea977a9fe1a57bd15a21111ae268333636fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:31 GMT
ADD file:53543c10022986b61ebedef43821a8984443468fb85c225a6fa19c8d6c76f642 in / 
# Tue, 15 Aug 2023 23:42:34 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:45:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:45:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:46:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:46:04 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:46:04 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:46:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:46:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e165c0f9e8f698888061cd00c559fc4e4751505fa2e647bfbf5b2ff0dadafbd2`  
		Last Modified: Tue, 15 Aug 2023 23:47:53 GMT  
		Size: 27.5 MB (27489761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50f6cb6aee208293ff4de3faa6f922cf494871a4a2ae5ebc8039c13654c91e1`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed3495d001827fc24354a561db0b089a3283e04251e6535cc584a8702f4226`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 2.3 MB (2257969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc14100c7e65bef730a13ebbcb8ef00d75512dc4ec87b42522271b05f9bf366`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 5.4 MB (5383391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8459fd8ee0a7b197fc673352f85d0bf6e064636852130e18170b42e410c47d0b`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b957665d1c4ddc4ea206ff316da27c25d911ed700608ac92f22de1db04bac1f`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:9e0a090f395df640e73bdda9b2387d3fbadf14c6cb5d789c43f1da21368acb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:49da7ccf4fd259700f2ac1db19a287d31a9ecf3a44e405470bf84179e4a151db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0439a8b1da8e9de36492d0a058f2acbdbfba92eb2bb87d48f767e0a31237098`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:03:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:03:24 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:03:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:03:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:03:34 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:03:34 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:03:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:03:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158fd3e69013bf879861985939c5aac2cbc46278db264aeae05ee1344222b07`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfba2e005bb6d82f820494ca9e65f63ae7042f6d1e2b54a8c6784c76b725a9d`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118bcda9b744a84a9c764eadd2a58bd39cba589942a2f8f7c6489d77a0f2d9a`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 221.3 KB (221274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76e498c240a7f12cb65ca8ed5d392aa245b449c370b5f77cc48781b7b0fe2e0`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd21f5dcda92cc1313530a1f07e075d96091d58e595b5ab77b810ff6b80125`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:92c72514aab4032a46bd337535d95862b853d6c7e90cb1e86e689409cc93616f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4589191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3dd418f5fe3e7be9bbb2632a3fd0fbbedad7f67e01d907d0d41c06bb6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:07 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:36:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:36:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:36:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:36:17 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:36:17 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:36:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ffd38f9a9109fd6f2d98e59fac671a21acbcbd826d953a190916b8e28c4d7c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafe31ddd32f93d6462563149d47e652289246cae76c3d69e2ae22c7f2dc157`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.2 MB (1236777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711c8b1ac9af3a0357e5e2ae10175a62c27bdea58e2e79fb7d413e2fa3a10138`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2f76630a196bedcec1d4f1f0542336e3189757e62aa7c83bd7f7e8f58680c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f674889b446c00cdd7da82689ee81ea78c84e02c462ad671bf3f9afd926afb1`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6b4ce7a3a962f7016da46f810228189be1cd6de1de0409f784505adca9fee42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4264646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f8b18499e87820bcff1593b1ccee12dbf54a9a32e6f7412af5d5c00268ce73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:51:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 21:51:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 21:51:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 21:51:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 21:51:52 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 21:51:52 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 21:51:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 21:51:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd254e37c3835d8a90d159f62497146fa2c0a51539455baafa4b5f3ad94073a`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87a0e27917b2f49aabe18b41a38f10f52561eaed9cd75ecbf9bb54dd5ad657`  
		Last Modified: Tue, 08 Aug 2023 21:52:10 GMT  
		Size: 1.2 MB (1163899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3f71f875284eede5e8bb82a4d0706d42594a0fec380b98dd516f0f75ed88`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 199.5 KB (199532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0eec6ac7d1270176b9ec72709b3186f9c9af79d5c747bdd03ac4818437e4b9`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da618866e96da51da8e7f96815a2d1e87198583082d2e819eaea328e7698149`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dfe860acf255915c9dcaae09dee878429e2b4c60798c048d82792352553d097d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4910891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9eb2d7445a05df9d201e84087d63696ade07ba940606d9e9deff249fd99f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:24:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:24:56 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:24:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:25:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:25:03 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:25:03 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:25:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa528de18ca9d8d7a81ae0d2ae78e694dca22d0e57c1adfd51230a5e72d602e`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4370e4fd5a67983765277bfaecb212d7f59e20db8264e69a6addca35b95526`  
		Last Modified: Wed, 09 Aug 2023 04:25:16 GMT  
		Size: 1.4 MB (1362701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605f0c15e8832deb396dd75011d9b8192e38e7b774733cea490c48a6c601da8`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 215.7 KB (215688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261765f25ad95a25543e0e6a6027cde75c58f6d3ceff188b0603ddcac15e32dd`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777264984131985e8771b4c25137123bf218b95e4de8ca97a58fe188f07340e6`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:3b9156620133e8bd472e78fcdc63367c0bd8ce4728e9b37100cecab16f9ba20b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4822397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ba2e93561dabc36ed836ecddc93cde747f6c0533764e243a1059c63a1ea4f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:25:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 22:25:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 22:25:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 22:25:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 22:25:30 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 22:25:30 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 22:25:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:25:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c31dcd775c39ea60679a161fbb3ec0114ed4a665986290232a4978c9b6a4e`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d724475632ebc1a22d1c3ca248315c7f4e6f7c5296f4eae98f587b0b3d246cb8`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.4 MB (1353881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a4abf10ff23af34214cad41a3ae8c5d722d0e578c719b02dcc3b303fa33ba`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 231.6 KB (231630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efbd75e8157b70348066566d4008a9c0bada288c04ada82ba412b78dc02e0c`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b78bd941b6d435a0daeb98222178fc6fdbd36c9b3cf1c59533e4bb87eb77b`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:b970c43232a9d83311742cddc2169c379db8304ab7409d9da95ff993ac82fbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4929752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45510f2b3a9a17d1bb74f84ca2abab8ed1061dff0e55839a3e8754e2c3290639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:49:46 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:50:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:50:03 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:50:04 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc475aa02ec0250350b4a331524b0a1e029de0aa51afc8d13cde5114f9a38f3`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64752c695a009aa97f4b6b21ee3618c0e6a15c1ccff9682ad7b50a01c411c09a`  
		Last Modified: Tue, 08 Aug 2023 23:50:27 GMT  
		Size: 1.4 MB (1361737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6958824bc296d0ee662dc09b65827f4c19cf6d08b0bc88c29c0aac7daef4b`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 220.0 KB (220022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbe94a7a7ea3e66fec66bafea8a8825cb0e1e4d4e13a6dd126caa55abc4368d`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d36cfcde9b1ab7cc6cd3e055bd3be46da17fbb42fd44094957dc575cb2aef`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7a35ce80545ef01185c3169716056ca5ee9520f1581c67074f5bd685d4f12ef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4646060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6af800db14443eb1061db4d4abf6affd33538028addd00c5cd1c46f9cbb00c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:16:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:16:02 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:16:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:16:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:16:08 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:16:08 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:16:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c947b711155cc9344e62be76da2fecb7e905aca9dad8fc53f2cb638fe84aa6`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705178608b8d1386cffd5a0ae5a7f41f2e6f580e6fb623ad053b6f8210fef7b1`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.2 MB (1221485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daaf6c162e1789b8a3c771759f74ad7c9ef9d19c7b7b614f9bea92f6f181874`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 208.6 KB (208644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9625b69d1551e16c0e8f95bc6eb00c95fbff0b0343391700336a2adb0752`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c787e2ceba069513a1f75d40922510e58442a2924c5668f7cefd24fff1c7`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:9e0a090f395df640e73bdda9b2387d3fbadf14c6cb5d789c43f1da21368acb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:49da7ccf4fd259700f2ac1db19a287d31a9ecf3a44e405470bf84179e4a151db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0439a8b1da8e9de36492d0a058f2acbdbfba92eb2bb87d48f767e0a31237098`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:03:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:03:24 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:03:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:03:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:03:34 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:03:34 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:03:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:03:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158fd3e69013bf879861985939c5aac2cbc46278db264aeae05ee1344222b07`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfba2e005bb6d82f820494ca9e65f63ae7042f6d1e2b54a8c6784c76b725a9d`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118bcda9b744a84a9c764eadd2a58bd39cba589942a2f8f7c6489d77a0f2d9a`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 221.3 KB (221274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76e498c240a7f12cb65ca8ed5d392aa245b449c370b5f77cc48781b7b0fe2e0`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd21f5dcda92cc1313530a1f07e075d96091d58e595b5ab77b810ff6b80125`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:92c72514aab4032a46bd337535d95862b853d6c7e90cb1e86e689409cc93616f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4589191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3dd418f5fe3e7be9bbb2632a3fd0fbbedad7f67e01d907d0d41c06bb6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:07 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:36:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:36:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:36:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:36:17 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:36:17 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:36:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ffd38f9a9109fd6f2d98e59fac671a21acbcbd826d953a190916b8e28c4d7c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafe31ddd32f93d6462563149d47e652289246cae76c3d69e2ae22c7f2dc157`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.2 MB (1236777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711c8b1ac9af3a0357e5e2ae10175a62c27bdea58e2e79fb7d413e2fa3a10138`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2f76630a196bedcec1d4f1f0542336e3189757e62aa7c83bd7f7e8f58680c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f674889b446c00cdd7da82689ee81ea78c84e02c462ad671bf3f9afd926afb1`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6b4ce7a3a962f7016da46f810228189be1cd6de1de0409f784505adca9fee42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4264646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f8b18499e87820bcff1593b1ccee12dbf54a9a32e6f7412af5d5c00268ce73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:51:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 21:51:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 21:51:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 21:51:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 21:51:52 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 21:51:52 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 21:51:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 21:51:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd254e37c3835d8a90d159f62497146fa2c0a51539455baafa4b5f3ad94073a`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87a0e27917b2f49aabe18b41a38f10f52561eaed9cd75ecbf9bb54dd5ad657`  
		Last Modified: Tue, 08 Aug 2023 21:52:10 GMT  
		Size: 1.2 MB (1163899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3f71f875284eede5e8bb82a4d0706d42594a0fec380b98dd516f0f75ed88`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 199.5 KB (199532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0eec6ac7d1270176b9ec72709b3186f9c9af79d5c747bdd03ac4818437e4b9`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da618866e96da51da8e7f96815a2d1e87198583082d2e819eaea328e7698149`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dfe860acf255915c9dcaae09dee878429e2b4c60798c048d82792352553d097d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4910891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9eb2d7445a05df9d201e84087d63696ade07ba940606d9e9deff249fd99f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:24:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:24:56 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:24:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:25:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:25:03 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:25:03 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:25:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa528de18ca9d8d7a81ae0d2ae78e694dca22d0e57c1adfd51230a5e72d602e`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4370e4fd5a67983765277bfaecb212d7f59e20db8264e69a6addca35b95526`  
		Last Modified: Wed, 09 Aug 2023 04:25:16 GMT  
		Size: 1.4 MB (1362701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605f0c15e8832deb396dd75011d9b8192e38e7b774733cea490c48a6c601da8`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 215.7 KB (215688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261765f25ad95a25543e0e6a6027cde75c58f6d3ceff188b0603ddcac15e32dd`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777264984131985e8771b4c25137123bf218b95e4de8ca97a58fe188f07340e6`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:3b9156620133e8bd472e78fcdc63367c0bd8ce4728e9b37100cecab16f9ba20b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4822397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ba2e93561dabc36ed836ecddc93cde747f6c0533764e243a1059c63a1ea4f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:25:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 22:25:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 22:25:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 22:25:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 22:25:30 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 22:25:30 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 22:25:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:25:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c31dcd775c39ea60679a161fbb3ec0114ed4a665986290232a4978c9b6a4e`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d724475632ebc1a22d1c3ca248315c7f4e6f7c5296f4eae98f587b0b3d246cb8`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.4 MB (1353881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a4abf10ff23af34214cad41a3ae8c5d722d0e578c719b02dcc3b303fa33ba`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 231.6 KB (231630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efbd75e8157b70348066566d4008a9c0bada288c04ada82ba412b78dc02e0c`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b78bd941b6d435a0daeb98222178fc6fdbd36c9b3cf1c59533e4bb87eb77b`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:b970c43232a9d83311742cddc2169c379db8304ab7409d9da95ff993ac82fbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4929752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45510f2b3a9a17d1bb74f84ca2abab8ed1061dff0e55839a3e8754e2c3290639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:49:46 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:50:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:50:03 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:50:04 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc475aa02ec0250350b4a331524b0a1e029de0aa51afc8d13cde5114f9a38f3`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64752c695a009aa97f4b6b21ee3618c0e6a15c1ccff9682ad7b50a01c411c09a`  
		Last Modified: Tue, 08 Aug 2023 23:50:27 GMT  
		Size: 1.4 MB (1361737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6958824bc296d0ee662dc09b65827f4c19cf6d08b0bc88c29c0aac7daef4b`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 220.0 KB (220022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbe94a7a7ea3e66fec66bafea8a8825cb0e1e4d4e13a6dd126caa55abc4368d`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d36cfcde9b1ab7cc6cd3e055bd3be46da17fbb42fd44094957dc575cb2aef`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7a35ce80545ef01185c3169716056ca5ee9520f1581c67074f5bd685d4f12ef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4646060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6af800db14443eb1061db4d4abf6affd33538028addd00c5cd1c46f9cbb00c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:16:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:16:02 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:16:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:16:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:16:08 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:16:08 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:16:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c947b711155cc9344e62be76da2fecb7e905aca9dad8fc53f2cb638fe84aa6`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705178608b8d1386cffd5a0ae5a7f41f2e6f580e6fb623ad053b6f8210fef7b1`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.2 MB (1221485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daaf6c162e1789b8a3c771759f74ad7c9ef9d19c7b7b614f9bea92f6f181874`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 208.6 KB (208644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9625b69d1551e16c0e8f95bc6eb00c95fbff0b0343391700336a2adb0752`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c787e2ceba069513a1f75d40922510e58442a2924c5668f7cefd24fff1c7`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:c42b9052f6a3081943ed261fadf5247b77cacceabc35c927eca7f7b12622d0e1
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

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:4f171c0f35b98776248253a67a50d37cccfd8473f07fb2695dde6d81ca2f139f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c704ab1e808854f06ff32f8281253ead1a6c81540e920fa3bb9a47349621c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:30:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 15:30:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:30:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 15:30:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 15:30:41 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 15:30:41 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 15:30:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 15:30:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f551bec805deb5c52468d55f52862d6fdac1441548dfe3b2dd6231bb13e35a9`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b935b31ab4b7796d274c3e3a3eb993798d9569355480bae3f11670c689b753d`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 2.6 MB (2586465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0425e3de531ea482e5effd29e0133c17f5d6210b2156d74dfb9c6d6a4e07864`  
		Last Modified: Wed, 16 Aug 2023 15:30:58 GMT  
		Size: 6.5 MB (6469487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802cd71544c6e0f12906f839800e76cbc6b05c24338da8b071db43a1d7ab7128`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c19c22c6f39515988c166c9dd995a108858c6d349fb731487be774bfffbfd`  
		Last Modified: Wed, 16 Aug 2023 15:30:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3c7289266dfbfbfaab5924d86a6921ba5649eb1fbb89a61b70a374e4e4207130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd889b8582c22d497551a1ddbb7e3f468870196acda21ae9b4ccf81381905ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:32 GMT
ADD file:661e14e9730f2608fba590f84fbb357838a3068db018f1e0569c79035783c86d in / 
# Tue, 15 Aug 2023 23:48:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:32:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:32:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:32:40 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:32:40 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:32:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:32:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:32:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:46d4cdda07fa660f92a3251737b0b22ad71ebafb783af374930d636935a2d8eb`  
		Last Modified: Tue, 15 Aug 2023 23:51:34 GMT  
		Size: 27.0 MB (26983543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076403abf1d4e6fa2aabacbba757d8d2ac102ce57a1be34150e84ed466a1a60`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0d0f8f84a3e50c749376a9eb2403d724afc7be278a0138a504ee3be9f5ed38`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 2.2 MB (2184076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12251ef379190d727f05a79edfe62dc54784cba94545aa3bd6908f640b86391a`  
		Last Modified: Wed, 16 Aug 2023 00:32:53 GMT  
		Size: 5.1 MB (5136554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3b5689db6eca5fcdd32a4c46476d4d3e38ee1b6dfeed21e802e84bd344b130`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47adae998e8dc4db3b09a4235d7adb64c346db5d1fc2444d80b594d2a30a5`  
		Last Modified: Wed, 16 Aug 2023 00:32:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5e8f0c26a16c4df76b2dc3fc6e710f79f928bc84e4ba1738ffb16a38d097769f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce26cf5793431ba1477cc81a099f7b8fec63f842df5a4d2ef708cfba02b37b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:12 GMT
ADD file:45cc27bd11f601d2fef5d7494a1a6253287e6d22e108e39c0884761c7533cd9c in / 
# Wed, 16 Aug 2023 00:17:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:25:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 05:25:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:25:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 05:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:25:51 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 05:25:51 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 05:25:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 05:25:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a44aa9565b062e4216f7b39ce6c67dcc5376e10f76caec55bd3acd1cc8b76b75`  
		Last Modified: Wed, 16 Aug 2023 00:21:27 GMT  
		Size: 24.8 MB (24805419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9c11d18979b89d7fa32eabe7f88a8cd64e01b4b8fa271fc334fb7d2b699b2`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b903a5c832d6f2fe4b495269a61fdf5cb49b36db7bea0569860fa6d84d00e`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 2.0 MB (2043310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f485e2da8130574c637c09ae0956f61e314214b2723b60575c9716e0f89ec`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 4.9 MB (4878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff0fe969b7330d3d7bb0cf4092f32ed845104416d60805fd202948a8404909`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25331bf9ce347281c7ed517293d861fd29f7d86535538cc031c9e9f3cfccbd97`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:64514be16b61c506ed4f38b7d901c8e2b309b08d76553ce403b891fce1180d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa77f5aed6d0831a3cc71c19adea277f0ccd481222fea6ba883c7f4865da198a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:20:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 10:20:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 10:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 10:20:30 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 10:20:30 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 10:20:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 10:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 10:20:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba019cbc445fbc18bd6dc20c125c8b39acf864a2824f00790582fa3560857391`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70188df993927106fe5ebbfd4c58f0d56ac94454c68dd496f6a7a61b5821602`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 2.4 MB (2429874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6b33daf23ff234e23662d0a02c051ef0e6151253ecaccf61b86ac6e8ea24f1`  
		Last Modified: Wed, 16 Aug 2023 10:20:46 GMT  
		Size: 5.5 MB (5478844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6b29684139d7512fa4b7ec02dbfd76c71952b4c482be6e6c368e4537d8af2c`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512d64842146daa84b8e6e4a582f3ec628fd10741650957d5aa95d22d9b874a`  
		Last Modified: Wed, 16 Aug 2023 10:20:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c1269ae34205a7105e15e21afb748acf092303d42802e691703c620acdfe126e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9dccc0b103ac44995ceb2445bec61936130bb9cfa4d0b782e16ad93ff12327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 20:40:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 20:40:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 20:40:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 20:41:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 20:41:03 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 20:41:03 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 20:41:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 20:41:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 20:41:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03457c876b07f1c91adaf8fb6937472beeda4a93329a4ea034beddb49371b3a0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a2251fa8712a87ba72cf1b7210863ff8ffb1714aea584978ffb9257568d78`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 2.6 MB (2583561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea65716bab4c92cfb7167bcec8537472d71948f927537f09b9ba7430fe8177ec`  
		Last Modified: Wed, 16 Aug 2023 20:41:23 GMT  
		Size: 5.9 MB (5940186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7fe253882086312121ecd6331d5e7ccda72ef6ff2245bff10b4760a2211b6`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe62b93bfa24ccf2d27d2385608f70dcaed03bb85755b5e0d5b8967c58417b0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:9b4dbeeeabafa3af4b5285d65a9ee1b4666256018167363e939c2bbb17d24aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d6ea40c73469c69646f5a574fa790101c1a2efe663c9ab48893271c1d0b6468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:08:43 GMT
ADD file:6122efd66f4e010b48e48eeb243d900439ef783f5a10df76043546a288d35d38 in / 
# Wed, 16 Aug 2023 00:08:47 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 03:26:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 17 Aug 2023 03:26:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 03:26:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 17 Aug 2023 03:28:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Aug 2023 03:28:38 GMT
VOLUME [/spiped]
# Thu, 17 Aug 2023 03:28:40 GMT
WORKDIR /spiped
# Thu, 17 Aug 2023 03:28:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Aug 2023 03:28:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 03:28:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52390931db742e6fb36945aff79b92fea76dcfe0964f8a5cf7e5b5faaa40b80f`  
		Last Modified: Wed, 16 Aug 2023 00:19:34 GMT  
		Size: 29.1 MB (29121481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d455b5a855378e6a6a616a046e1fa07cfb625a604fd20ca1d37d52fda22174`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1badeb5ed503d07963318ac71660ae002cc2315591c20057b3c2c18811e128ba`  
		Last Modified: Thu, 17 Aug 2023 03:29:02 GMT  
		Size: 1.8 MB (1831704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acdbe213b6cb697af754286c587896d18df39349e4b4f26cb3eaaf0db9b0844`  
		Last Modified: Thu, 17 Aug 2023 03:29:06 GMT  
		Size: 5.8 MB (5801896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c09cc60cf7ce55c7cd74c75045171c3cd7a5cac4c3505dfee318d5cce1e9cd4`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee1deae900a5f4fdb29cdff7c2a89c3326fe9869b248c6a3943008517f9bfd8`  
		Last Modified: Thu, 17 Aug 2023 03:29:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:cda509b294751f959f7764d1e1af011f4ce61c61e34eefbd25203a9ca0b28aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc441e69e8db9c2db390a467a61c87ec2e35d7a2a63c359e0e788615281064e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 15:42:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 15:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:43:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 15:44:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 15:44:05 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 15:44:05 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 15:44:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 15:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 15:44:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0834a39a8f321e61913bcebc5b10f2f4388ad008aed3aa0b7108c1c98aa672b8`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8637b8770fbcc45d233bc8c0685a004f863248524d9589bb8133462ad2ef98`  
		Last Modified: Fri, 28 Jul 2023 15:44:25 GMT  
		Size: 2.8 MB (2764991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e47b32eeb162a453e0f56b17945b85e59188dea37e5050beeb9fe549df43b6`  
		Last Modified: Fri, 28 Jul 2023 15:44:26 GMT  
		Size: 6.4 MB (6420314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6ad0fc910585043bd75c1f9f637776962532c3318497e750adf297becfa27a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe513cc6e981f0bcc9b41c0abcbebb0c975a964bdfc186524bcefd2f32b1496a`  
		Last Modified: Fri, 28 Jul 2023 15:44:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:84cf3b032ac9c98b0694f112d6543074edec69387196326c626d5110782d0ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5d933bb3ed3f1d38a0072fffbea977a9fe1a57bd15a21111ae268333636fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:31 GMT
ADD file:53543c10022986b61ebedef43821a8984443468fb85c225a6fa19c8d6c76f642 in / 
# Tue, 15 Aug 2023 23:42:34 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:45:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 00:45:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 00:46:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:46:04 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 00:46:04 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 00:46:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:46:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e165c0f9e8f698888061cd00c559fc4e4751505fa2e647bfbf5b2ff0dadafbd2`  
		Last Modified: Tue, 15 Aug 2023 23:47:53 GMT  
		Size: 27.5 MB (27489761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50f6cb6aee208293ff4de3faa6f922cf494871a4a2ae5ebc8039c13654c91e1`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed3495d001827fc24354a561db0b089a3283e04251e6535cc584a8702f4226`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 2.3 MB (2257969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc14100c7e65bef730a13ebbcb8ef00d75512dc4ec87b42522271b05f9bf366`  
		Last Modified: Wed, 16 Aug 2023 00:46:30 GMT  
		Size: 5.4 MB (5383391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8459fd8ee0a7b197fc673352f85d0bf6e064636852130e18170b42e410c47d0b`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b957665d1c4ddc4ea206ff316da27c25d911ed700608ac92f22de1db04bac1f`  
		Last Modified: Wed, 16 Aug 2023 00:46:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
