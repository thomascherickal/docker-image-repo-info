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
$ docker pull spiped@sha256:d92aed1ecd2051baf2fe4710dba156db5cf91c988114578f8864e1dd2f51eb20
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
$ docker pull spiped@sha256:6581a63ceb222a36c5a066bd9fd25d1089f56f572db6f1de0e4e300086046ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37420421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6ca3f0433ef4d8b38ba7574f6d2b66c9d1ab7b2c3a3488615fbd7e84a837b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 11:50:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 11:50:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 11:50:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 11:51:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 11:51:15 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 11:51:16 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 11:51:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 11:51:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 11:51:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cc092bee51fe89014f3c86fa11250aac6a790fb2db732775e807cda6118b74`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa13df5b7ee9e66563a5595b9d504a159a89ff918027e6e9e2429f1abf47aa`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65647ffa5253661353974d53cc8c42a7e872a9a0eb746ed6429c4bee1320447`  
		Last Modified: Wed, 05 Oct 2022 11:51:34 GMT  
		Size: 6.0 MB (5997064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b73ddd0ce7a9700293b283147579823192fa9d6cfb4e74b057be298b7c378ca`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a58f3e29fdada327192e4ccad2fc576d77134eaf59898e76b3963a432ba5b`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6df982fe3267ab78d832bc1f58bb4ac7d2caff6eee59bc7800e34b18f62e6f6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb66d8e5bd73b4af3a6ffca4587bdd6654b70c0e397aa0e02faf21edcbcb4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 16:07:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 16:08:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:08:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 16:08:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 16:08:34 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 16:08:34 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 16:08:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 16:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 16:08:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1de9b12151a17aa1719d3f173627857887605bfdf1f85c17fffbe50c84dab`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243c502416ddc5daec49327de0a4f5b4839e634c309a98e1df478133e1c99f73`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853550e4b4ac033183cc1f9eb53c48b340f23f8ae0de0e1ef351080952c1cb9`  
		Last Modified: Tue, 13 Sep 2022 16:09:00 GMT  
		Size: 5.0 MB (5027871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ae59ce66b6ceeb787e51b79c6bd6e1e9f04b376c919bd733c3c2a0442886e`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c6fd322e368b57339070af206933b4db0cb8686b52c730740d07721817a84`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5b1c678ffa2f82afd070f83e792d634ccf3a9c8c809d886cf98645950152f7c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31317986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160c3624a2ed934293f7a4a408d751dd7d806fd358adedb0e1795a2e200e793e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 02:03:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 02:03:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 02:03:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 02:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 02:03:57 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 02:03:58 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 02:03:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 02:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defaed76fde0f3b65e06fd9f46b48ad7700b915e5ffddbad8a16167e48d631ab`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ead107aae3168ca5b395778f10b487f08ad9d058aceca1111a51c60937ac95`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76495f29833edcd4dfae059cbdad1bb51c3d68e984768b3b48f5ab4fad6cb08`  
		Last Modified: Wed, 14 Sep 2022 02:04:36 GMT  
		Size: 4.7 MB (4747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbf0bfd3ec1bfd4a66d3202aa908910aa9e5f89b165f050afbb9097f3bde374`  
		Last Modified: Wed, 14 Sep 2022 02:04:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945863be2e4a3b708b817104df1efb5273b99ae8a8d63e7ce124aca615b90252`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dabfac32e33fda6f8543e94730b92bea339bbc2be44525f8a98a2430811f1259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396eee83acf2b887d489bf2916c0f421b5f8b7c76b97c45b924a8e9b38885c47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 15:32:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 15:32:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 15:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 15:32:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 15:32:35 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 15:32:36 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 15:32:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 15:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 15:32:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a2b3a10608f3f1c16f3961525be3093dfac72b60edafff4713a5c36f4a47f`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8952ae8072f5f7b566992352417ca75e515ad92d7f379c654063cee0d1025bc6`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a0dc92476ccd6b2587e63791367f000f63bd9cd44a71ba525f1dc932fdc40`  
		Last Modified: Tue, 13 Sep 2022 15:33:12 GMT  
		Size: 5.3 MB (5270148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d5179d139cbf869c35de3c13a17d7309f06b6c71e5d82d9783af2266481f5d`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe043e7289aba1dcde04e36faa3ea835d38ff5470029d1603ed4bfadfd32f88`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:080a3ea980d3a0cea9e71e608daac41551810d1d1e864065d09d82c3c71c12f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40275724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdec6799a11241ff8e045278507ad92d1c51719d5d5fab38a06aee9786c347f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:38:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 13:38:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:38:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 13:38:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 13:38:32 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 13:38:33 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 13:38:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 13:38:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db4432e37229888ed10498cbb73a3db7967d321668c0fe3a5ff19544ce4058b`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf7f2aa932c3b1343a7a5582ac1b2615872e7bb6de032c757ff8c82697b9cb`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd929440d2f3ee4d86d6505d860ea41e1afa4ec703c48d3a37bc788e6fa735ba`  
		Last Modified: Tue, 13 Sep 2022 13:39:08 GMT  
		Size: 7.9 MB (7888964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5899589487bc133bfdd2d1e78feb31137bbb2802f6d9c4b9ea3922107efe7ef`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe3cf381a26f3297bd9b2623ae878e93eca5772348ca35a0ebc631182724a`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:69da557a701cec978d7b047fcb58b719bc7f73002471092a81156d0ebfc911ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8b856a250d8d3b23ac7e8f3c688d644218eaff92a75e5b7969f1a0ea9c5978`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:18:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 00:19:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:19:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 00:20:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 00:20:45 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 00:20:48 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 00:20:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 00:20:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:20:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453fe9f8f8eeeeac37559150e10691371c767d2109c6c4707ad80c6c81525a5b`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e231dc6f2975ea71e13f71ce249ea36cc1f5b9bc29cf4edb6cb221363a4f9c`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786f0306fa7c793bd8899c30db3c7f7d094115ce42b9cf3743fd6f8314f20ad`  
		Last Modified: Wed, 14 Sep 2022 00:21:17 GMT  
		Size: 5.7 MB (5705126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8411ad45e2cd35b79183d1a54c5718128e54f95133894e7992f363e6e523153`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96301dfd97b62754754bc3f8e044510f2914826da061612de4a79bc2f4e3422`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:219e13c963456313e7f3d64811d97d01c472ed6f8a8d5bf55ee454e85b830cca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dcc529b0d26759e97fa2275e79e6f6e5058f2dfd6496402025839ba28ebf0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:23:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 08:23:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:23:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 08:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 08:24:33 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 08:24:33 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 08:24:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 08:24:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f18e563d25d3c5678e671e27753e3401c7b1ce8b60d60e5ba74ff1a5b858efe`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce19254f672d95be371e0158b1c728d3190e4c0561a7a533c9100fcbaffdeb`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b10a8dacb14f17077045d2e167303c50da8950371763ecb50c3886473fa2f`  
		Last Modified: Wed, 05 Oct 2022 08:25:11 GMT  
		Size: 6.0 MB (5998253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfe8808d03f72c63cf023c8a969140f3f940b2c718f2d2b518ec0cf6427077`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919707dce66a31120cdb5e4f928e6741464a96036f4d2076533bd94f81789bd`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:a6d6dc4c4fe5489f96d3eb044c7239d7528ebc7ee73337c3c53f0e15dccd3069
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34840409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14179e00a209732b609dfcc1b387f488c420760228b4dffb6675104fe0b2b9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 03:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:25:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 03:25:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 03:25:58 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 03:25:58 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 03:25:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:25:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:25:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af006c53786c75badcea31a45fa2e8e9bb3ab687d59cc0727fd2c48e18cbf76a`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb4dbf0ea8ead55cceb2c17b6d3faff2c5bf1d95624ed864dd0f305dfc6024d`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66f607cb7e14fb758c615f74a452a8669ccd26b30bbe549c175af95f900244`  
		Last Modified: Wed, 05 Oct 2022 03:26:31 GMT  
		Size: 5.2 MB (5186434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2993ec9272e99c08c4475bbb91800a0f5764a8728cff535e33f02ad29214c3`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99234ee6be52665bc5df00130740b88f466b372811e0638a734211b3ffecddd`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:07ff0a1ef1a50f0745ee97ebd2e91fd2c55a07e8877639d442a143bcb0c82b2c
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:50c8f30f14893fdc35670904e644b7a61a600294dbab4d18238198830510ec5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0a996edc8ef3c7120d02cd6c808d8adca8094539939b1c842bfdc578c3f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 03:46:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 03:46:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 03:46:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 03:46:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 03:46:17 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 03:46:17 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 03:46:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 03:46:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 03:46:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2d1ea22931d8c79f9a9895368cefc8af2039f86e4795ad8e9d3d74ff4f7a6`  
		Last Modified: Thu, 11 Aug 2022 03:46:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b222ded0c4fe977a385f93c4edc434f1284118cb148a13442a3ae08b06718`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a524ad23a1be21e15df07159b163bac902d8251f08372a02c998fcbe1f520`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 199.6 KB (199555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5004c8029cac2bfb365d7b0a52fdccb5b64e8ae2a2c63bf1f5680b877e914189`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811d9f370333f86cfb5b0fdebf56e3d1d77472e98c127219d4d48584c23d8cb`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:d92aed1ecd2051baf2fe4710dba156db5cf91c988114578f8864e1dd2f51eb20
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
$ docker pull spiped@sha256:6581a63ceb222a36c5a066bd9fd25d1089f56f572db6f1de0e4e300086046ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37420421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6ca3f0433ef4d8b38ba7574f6d2b66c9d1ab7b2c3a3488615fbd7e84a837b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 11:50:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 11:50:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 11:50:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 11:51:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 11:51:15 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 11:51:16 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 11:51:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 11:51:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 11:51:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cc092bee51fe89014f3c86fa11250aac6a790fb2db732775e807cda6118b74`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa13df5b7ee9e66563a5595b9d504a159a89ff918027e6e9e2429f1abf47aa`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65647ffa5253661353974d53cc8c42a7e872a9a0eb746ed6429c4bee1320447`  
		Last Modified: Wed, 05 Oct 2022 11:51:34 GMT  
		Size: 6.0 MB (5997064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b73ddd0ce7a9700293b283147579823192fa9d6cfb4e74b057be298b7c378ca`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a58f3e29fdada327192e4ccad2fc576d77134eaf59898e76b3963a432ba5b`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6df982fe3267ab78d832bc1f58bb4ac7d2caff6eee59bc7800e34b18f62e6f6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb66d8e5bd73b4af3a6ffca4587bdd6654b70c0e397aa0e02faf21edcbcb4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 16:07:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 16:08:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:08:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 16:08:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 16:08:34 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 16:08:34 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 16:08:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 16:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 16:08:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1de9b12151a17aa1719d3f173627857887605bfdf1f85c17fffbe50c84dab`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243c502416ddc5daec49327de0a4f5b4839e634c309a98e1df478133e1c99f73`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853550e4b4ac033183cc1f9eb53c48b340f23f8ae0de0e1ef351080952c1cb9`  
		Last Modified: Tue, 13 Sep 2022 16:09:00 GMT  
		Size: 5.0 MB (5027871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ae59ce66b6ceeb787e51b79c6bd6e1e9f04b376c919bd733c3c2a0442886e`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c6fd322e368b57339070af206933b4db0cb8686b52c730740d07721817a84`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5b1c678ffa2f82afd070f83e792d634ccf3a9c8c809d886cf98645950152f7c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31317986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160c3624a2ed934293f7a4a408d751dd7d806fd358adedb0e1795a2e200e793e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 02:03:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 02:03:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 02:03:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 02:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 02:03:57 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 02:03:58 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 02:03:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 02:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defaed76fde0f3b65e06fd9f46b48ad7700b915e5ffddbad8a16167e48d631ab`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ead107aae3168ca5b395778f10b487f08ad9d058aceca1111a51c60937ac95`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76495f29833edcd4dfae059cbdad1bb51c3d68e984768b3b48f5ab4fad6cb08`  
		Last Modified: Wed, 14 Sep 2022 02:04:36 GMT  
		Size: 4.7 MB (4747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbf0bfd3ec1bfd4a66d3202aa908910aa9e5f89b165f050afbb9097f3bde374`  
		Last Modified: Wed, 14 Sep 2022 02:04:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945863be2e4a3b708b817104df1efb5273b99ae8a8d63e7ce124aca615b90252`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dabfac32e33fda6f8543e94730b92bea339bbc2be44525f8a98a2430811f1259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396eee83acf2b887d489bf2916c0f421b5f8b7c76b97c45b924a8e9b38885c47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 15:32:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 15:32:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 15:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 15:32:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 15:32:35 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 15:32:36 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 15:32:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 15:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 15:32:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a2b3a10608f3f1c16f3961525be3093dfac72b60edafff4713a5c36f4a47f`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8952ae8072f5f7b566992352417ca75e515ad92d7f379c654063cee0d1025bc6`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a0dc92476ccd6b2587e63791367f000f63bd9cd44a71ba525f1dc932fdc40`  
		Last Modified: Tue, 13 Sep 2022 15:33:12 GMT  
		Size: 5.3 MB (5270148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d5179d139cbf869c35de3c13a17d7309f06b6c71e5d82d9783af2266481f5d`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe043e7289aba1dcde04e36faa3ea835d38ff5470029d1603ed4bfadfd32f88`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:080a3ea980d3a0cea9e71e608daac41551810d1d1e864065d09d82c3c71c12f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40275724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdec6799a11241ff8e045278507ad92d1c51719d5d5fab38a06aee9786c347f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:38:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 13:38:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:38:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 13:38:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 13:38:32 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 13:38:33 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 13:38:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 13:38:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db4432e37229888ed10498cbb73a3db7967d321668c0fe3a5ff19544ce4058b`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf7f2aa932c3b1343a7a5582ac1b2615872e7bb6de032c757ff8c82697b9cb`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd929440d2f3ee4d86d6505d860ea41e1afa4ec703c48d3a37bc788e6fa735ba`  
		Last Modified: Tue, 13 Sep 2022 13:39:08 GMT  
		Size: 7.9 MB (7888964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5899589487bc133bfdd2d1e78feb31137bbb2802f6d9c4b9ea3922107efe7ef`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe3cf381a26f3297bd9b2623ae878e93eca5772348ca35a0ebc631182724a`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:69da557a701cec978d7b047fcb58b719bc7f73002471092a81156d0ebfc911ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8b856a250d8d3b23ac7e8f3c688d644218eaff92a75e5b7969f1a0ea9c5978`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:18:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 00:19:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:19:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 00:20:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 00:20:45 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 00:20:48 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 00:20:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 00:20:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:20:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453fe9f8f8eeeeac37559150e10691371c767d2109c6c4707ad80c6c81525a5b`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e231dc6f2975ea71e13f71ce249ea36cc1f5b9bc29cf4edb6cb221363a4f9c`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786f0306fa7c793bd8899c30db3c7f7d094115ce42b9cf3743fd6f8314f20ad`  
		Last Modified: Wed, 14 Sep 2022 00:21:17 GMT  
		Size: 5.7 MB (5705126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8411ad45e2cd35b79183d1a54c5718128e54f95133894e7992f363e6e523153`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96301dfd97b62754754bc3f8e044510f2914826da061612de4a79bc2f4e3422`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:219e13c963456313e7f3d64811d97d01c472ed6f8a8d5bf55ee454e85b830cca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dcc529b0d26759e97fa2275e79e6f6e5058f2dfd6496402025839ba28ebf0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:23:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 08:23:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:23:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 08:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 08:24:33 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 08:24:33 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 08:24:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 08:24:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f18e563d25d3c5678e671e27753e3401c7b1ce8b60d60e5ba74ff1a5b858efe`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce19254f672d95be371e0158b1c728d3190e4c0561a7a533c9100fcbaffdeb`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b10a8dacb14f17077045d2e167303c50da8950371763ecb50c3886473fa2f`  
		Last Modified: Wed, 05 Oct 2022 08:25:11 GMT  
		Size: 6.0 MB (5998253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfe8808d03f72c63cf023c8a969140f3f940b2c718f2d2b518ec0cf6427077`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919707dce66a31120cdb5e4f928e6741464a96036f4d2076533bd94f81789bd`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:a6d6dc4c4fe5489f96d3eb044c7239d7528ebc7ee73337c3c53f0e15dccd3069
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34840409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14179e00a209732b609dfcc1b387f488c420760228b4dffb6675104fe0b2b9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 03:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:25:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 03:25:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 03:25:58 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 03:25:58 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 03:25:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:25:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:25:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af006c53786c75badcea31a45fa2e8e9bb3ab687d59cc0727fd2c48e18cbf76a`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb4dbf0ea8ead55cceb2c17b6d3faff2c5bf1d95624ed864dd0f305dfc6024d`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66f607cb7e14fb758c615f74a452a8669ccd26b30bbe549c175af95f900244`  
		Last Modified: Wed, 05 Oct 2022 03:26:31 GMT  
		Size: 5.2 MB (5186434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2993ec9272e99c08c4475bbb91800a0f5764a8728cff535e33f02ad29214c3`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99234ee6be52665bc5df00130740b88f466b372811e0638a734211b3ffecddd`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:07ff0a1ef1a50f0745ee97ebd2e91fd2c55a07e8877639d442a143bcb0c82b2c
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:50c8f30f14893fdc35670904e644b7a61a600294dbab4d18238198830510ec5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0a996edc8ef3c7120d02cd6c808d8adca8094539939b1c842bfdc578c3f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 03:46:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 03:46:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 03:46:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 03:46:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 03:46:17 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 03:46:17 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 03:46:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 03:46:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 03:46:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2d1ea22931d8c79f9a9895368cefc8af2039f86e4795ad8e9d3d74ff4f7a6`  
		Last Modified: Thu, 11 Aug 2022 03:46:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b222ded0c4fe977a385f93c4edc434f1284118cb148a13442a3ae08b06718`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a524ad23a1be21e15df07159b163bac902d8251f08372a02c998fcbe1f520`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 199.6 KB (199555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5004c8029cac2bfb365d7b0a52fdccb5b64e8ae2a2c63bf1f5680b877e914189`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811d9f370333f86cfb5b0fdebf56e3d1d77472e98c127219d4d48584c23d8cb`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:d92aed1ecd2051baf2fe4710dba156db5cf91c988114578f8864e1dd2f51eb20
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
$ docker pull spiped@sha256:6581a63ceb222a36c5a066bd9fd25d1089f56f572db6f1de0e4e300086046ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37420421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6ca3f0433ef4d8b38ba7574f6d2b66c9d1ab7b2c3a3488615fbd7e84a837b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 11:50:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 11:50:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 11:50:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 11:51:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 11:51:15 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 11:51:16 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 11:51:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 11:51:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 11:51:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cc092bee51fe89014f3c86fa11250aac6a790fb2db732775e807cda6118b74`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa13df5b7ee9e66563a5595b9d504a159a89ff918027e6e9e2429f1abf47aa`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65647ffa5253661353974d53cc8c42a7e872a9a0eb746ed6429c4bee1320447`  
		Last Modified: Wed, 05 Oct 2022 11:51:34 GMT  
		Size: 6.0 MB (5997064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b73ddd0ce7a9700293b283147579823192fa9d6cfb4e74b057be298b7c378ca`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a58f3e29fdada327192e4ccad2fc576d77134eaf59898e76b3963a432ba5b`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6df982fe3267ab78d832bc1f58bb4ac7d2caff6eee59bc7800e34b18f62e6f6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb66d8e5bd73b4af3a6ffca4587bdd6654b70c0e397aa0e02faf21edcbcb4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 16:07:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 16:08:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:08:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 16:08:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 16:08:34 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 16:08:34 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 16:08:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 16:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 16:08:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1de9b12151a17aa1719d3f173627857887605bfdf1f85c17fffbe50c84dab`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243c502416ddc5daec49327de0a4f5b4839e634c309a98e1df478133e1c99f73`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853550e4b4ac033183cc1f9eb53c48b340f23f8ae0de0e1ef351080952c1cb9`  
		Last Modified: Tue, 13 Sep 2022 16:09:00 GMT  
		Size: 5.0 MB (5027871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ae59ce66b6ceeb787e51b79c6bd6e1e9f04b376c919bd733c3c2a0442886e`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c6fd322e368b57339070af206933b4db0cb8686b52c730740d07721817a84`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5b1c678ffa2f82afd070f83e792d634ccf3a9c8c809d886cf98645950152f7c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31317986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160c3624a2ed934293f7a4a408d751dd7d806fd358adedb0e1795a2e200e793e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 02:03:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 02:03:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 02:03:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 02:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 02:03:57 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 02:03:58 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 02:03:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 02:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defaed76fde0f3b65e06fd9f46b48ad7700b915e5ffddbad8a16167e48d631ab`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ead107aae3168ca5b395778f10b487f08ad9d058aceca1111a51c60937ac95`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76495f29833edcd4dfae059cbdad1bb51c3d68e984768b3b48f5ab4fad6cb08`  
		Last Modified: Wed, 14 Sep 2022 02:04:36 GMT  
		Size: 4.7 MB (4747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbf0bfd3ec1bfd4a66d3202aa908910aa9e5f89b165f050afbb9097f3bde374`  
		Last Modified: Wed, 14 Sep 2022 02:04:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945863be2e4a3b708b817104df1efb5273b99ae8a8d63e7ce124aca615b90252`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dabfac32e33fda6f8543e94730b92bea339bbc2be44525f8a98a2430811f1259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396eee83acf2b887d489bf2916c0f421b5f8b7c76b97c45b924a8e9b38885c47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 15:32:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 15:32:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 15:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 15:32:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 15:32:35 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 15:32:36 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 15:32:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 15:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 15:32:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a2b3a10608f3f1c16f3961525be3093dfac72b60edafff4713a5c36f4a47f`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8952ae8072f5f7b566992352417ca75e515ad92d7f379c654063cee0d1025bc6`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a0dc92476ccd6b2587e63791367f000f63bd9cd44a71ba525f1dc932fdc40`  
		Last Modified: Tue, 13 Sep 2022 15:33:12 GMT  
		Size: 5.3 MB (5270148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d5179d139cbf869c35de3c13a17d7309f06b6c71e5d82d9783af2266481f5d`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe043e7289aba1dcde04e36faa3ea835d38ff5470029d1603ed4bfadfd32f88`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:080a3ea980d3a0cea9e71e608daac41551810d1d1e864065d09d82c3c71c12f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40275724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdec6799a11241ff8e045278507ad92d1c51719d5d5fab38a06aee9786c347f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:38:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 13:38:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:38:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 13:38:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 13:38:32 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 13:38:33 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 13:38:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 13:38:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db4432e37229888ed10498cbb73a3db7967d321668c0fe3a5ff19544ce4058b`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf7f2aa932c3b1343a7a5582ac1b2615872e7bb6de032c757ff8c82697b9cb`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd929440d2f3ee4d86d6505d860ea41e1afa4ec703c48d3a37bc788e6fa735ba`  
		Last Modified: Tue, 13 Sep 2022 13:39:08 GMT  
		Size: 7.9 MB (7888964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5899589487bc133bfdd2d1e78feb31137bbb2802f6d9c4b9ea3922107efe7ef`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe3cf381a26f3297bd9b2623ae878e93eca5772348ca35a0ebc631182724a`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:69da557a701cec978d7b047fcb58b719bc7f73002471092a81156d0ebfc911ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8b856a250d8d3b23ac7e8f3c688d644218eaff92a75e5b7969f1a0ea9c5978`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:18:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 00:19:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:19:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 00:20:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 00:20:45 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 00:20:48 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 00:20:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 00:20:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:20:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453fe9f8f8eeeeac37559150e10691371c767d2109c6c4707ad80c6c81525a5b`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e231dc6f2975ea71e13f71ce249ea36cc1f5b9bc29cf4edb6cb221363a4f9c`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786f0306fa7c793bd8899c30db3c7f7d094115ce42b9cf3743fd6f8314f20ad`  
		Last Modified: Wed, 14 Sep 2022 00:21:17 GMT  
		Size: 5.7 MB (5705126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8411ad45e2cd35b79183d1a54c5718128e54f95133894e7992f363e6e523153`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96301dfd97b62754754bc3f8e044510f2914826da061612de4a79bc2f4e3422`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:219e13c963456313e7f3d64811d97d01c472ed6f8a8d5bf55ee454e85b830cca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dcc529b0d26759e97fa2275e79e6f6e5058f2dfd6496402025839ba28ebf0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:23:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 08:23:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:23:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 08:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 08:24:33 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 08:24:33 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 08:24:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 08:24:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f18e563d25d3c5678e671e27753e3401c7b1ce8b60d60e5ba74ff1a5b858efe`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce19254f672d95be371e0158b1c728d3190e4c0561a7a533c9100fcbaffdeb`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b10a8dacb14f17077045d2e167303c50da8950371763ecb50c3886473fa2f`  
		Last Modified: Wed, 05 Oct 2022 08:25:11 GMT  
		Size: 6.0 MB (5998253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfe8808d03f72c63cf023c8a969140f3f940b2c718f2d2b518ec0cf6427077`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919707dce66a31120cdb5e4f928e6741464a96036f4d2076533bd94f81789bd`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:a6d6dc4c4fe5489f96d3eb044c7239d7528ebc7ee73337c3c53f0e15dccd3069
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34840409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14179e00a209732b609dfcc1b387f488c420760228b4dffb6675104fe0b2b9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 03:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:25:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 03:25:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 03:25:58 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 03:25:58 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 03:25:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:25:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:25:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af006c53786c75badcea31a45fa2e8e9bb3ab687d59cc0727fd2c48e18cbf76a`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb4dbf0ea8ead55cceb2c17b6d3faff2c5bf1d95624ed864dd0f305dfc6024d`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66f607cb7e14fb758c615f74a452a8669ccd26b30bbe549c175af95f900244`  
		Last Modified: Wed, 05 Oct 2022 03:26:31 GMT  
		Size: 5.2 MB (5186434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2993ec9272e99c08c4475bbb91800a0f5764a8728cff535e33f02ad29214c3`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99234ee6be52665bc5df00130740b88f466b372811e0638a734211b3ffecddd`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:07ff0a1ef1a50f0745ee97ebd2e91fd2c55a07e8877639d442a143bcb0c82b2c
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:50c8f30f14893fdc35670904e644b7a61a600294dbab4d18238198830510ec5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0a996edc8ef3c7120d02cd6c808d8adca8094539939b1c842bfdc578c3f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 03:46:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 03:46:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 03:46:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 03:46:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 03:46:17 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 03:46:17 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 03:46:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 03:46:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 03:46:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2d1ea22931d8c79f9a9895368cefc8af2039f86e4795ad8e9d3d74ff4f7a6`  
		Last Modified: Thu, 11 Aug 2022 03:46:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b222ded0c4fe977a385f93c4edc434f1284118cb148a13442a3ae08b06718`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a524ad23a1be21e15df07159b163bac902d8251f08372a02c998fcbe1f520`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 199.6 KB (199555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5004c8029cac2bfb365d7b0a52fdccb5b64e8ae2a2c63bf1f5680b877e914189`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811d9f370333f86cfb5b0fdebf56e3d1d77472e98c127219d4d48584c23d8cb`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:07ff0a1ef1a50f0745ee97ebd2e91fd2c55a07e8877639d442a143bcb0c82b2c
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:50c8f30f14893fdc35670904e644b7a61a600294dbab4d18238198830510ec5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0a996edc8ef3c7120d02cd6c808d8adca8094539939b1c842bfdc578c3f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 03:46:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 03:46:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 03:46:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 03:46:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 03:46:17 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 03:46:17 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 03:46:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 03:46:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 03:46:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2d1ea22931d8c79f9a9895368cefc8af2039f86e4795ad8e9d3d74ff4f7a6`  
		Last Modified: Thu, 11 Aug 2022 03:46:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b222ded0c4fe977a385f93c4edc434f1284118cb148a13442a3ae08b06718`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a524ad23a1be21e15df07159b163bac902d8251f08372a02c998fcbe1f520`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 199.6 KB (199555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5004c8029cac2bfb365d7b0a52fdccb5b64e8ae2a2c63bf1f5680b877e914189`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811d9f370333f86cfb5b0fdebf56e3d1d77472e98c127219d4d48584c23d8cb`  
		Last Modified: Thu, 11 Aug 2022 03:46:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:d92aed1ecd2051baf2fe4710dba156db5cf91c988114578f8864e1dd2f51eb20
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
$ docker pull spiped@sha256:6581a63ceb222a36c5a066bd9fd25d1089f56f572db6f1de0e4e300086046ff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37420421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6ca3f0433ef4d8b38ba7574f6d2b66c9d1ab7b2c3a3488615fbd7e84a837b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 11:50:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 11:50:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 11:50:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 11:51:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 11:51:15 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 11:51:16 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 11:51:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 11:51:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 11:51:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cc092bee51fe89014f3c86fa11250aac6a790fb2db732775e807cda6118b74`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa13df5b7ee9e66563a5595b9d504a159a89ff918027e6e9e2429f1abf47aa`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65647ffa5253661353974d53cc8c42a7e872a9a0eb746ed6429c4bee1320447`  
		Last Modified: Wed, 05 Oct 2022 11:51:34 GMT  
		Size: 6.0 MB (5997064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b73ddd0ce7a9700293b283147579823192fa9d6cfb4e74b057be298b7c378ca`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a58f3e29fdada327192e4ccad2fc576d77134eaf59898e76b3963a432ba5b`  
		Last Modified: Wed, 05 Oct 2022 11:51:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6df982fe3267ab78d832bc1f58bb4ac7d2caff6eee59bc7800e34b18f62e6f6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb66d8e5bd73b4af3a6ffca4587bdd6654b70c0e397aa0e02faf21edcbcb4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 16:07:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 16:08:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:08:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 16:08:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 16:08:34 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 16:08:34 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 16:08:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 16:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 16:08:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1de9b12151a17aa1719d3f173627857887605bfdf1f85c17fffbe50c84dab`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243c502416ddc5daec49327de0a4f5b4839e634c309a98e1df478133e1c99f73`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853550e4b4ac033183cc1f9eb53c48b340f23f8ae0de0e1ef351080952c1cb9`  
		Last Modified: Tue, 13 Sep 2022 16:09:00 GMT  
		Size: 5.0 MB (5027871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ae59ce66b6ceeb787e51b79c6bd6e1e9f04b376c919bd733c3c2a0442886e`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c6fd322e368b57339070af206933b4db0cb8686b52c730740d07721817a84`  
		Last Modified: Tue, 13 Sep 2022 16:08:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5b1c678ffa2f82afd070f83e792d634ccf3a9c8c809d886cf98645950152f7c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31317986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160c3624a2ed934293f7a4a408d751dd7d806fd358adedb0e1795a2e200e793e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 02:03:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 02:03:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 02:03:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 02:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 02:03:57 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 02:03:58 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 02:03:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 02:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defaed76fde0f3b65e06fd9f46b48ad7700b915e5ffddbad8a16167e48d631ab`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ead107aae3168ca5b395778f10b487f08ad9d058aceca1111a51c60937ac95`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76495f29833edcd4dfae059cbdad1bb51c3d68e984768b3b48f5ab4fad6cb08`  
		Last Modified: Wed, 14 Sep 2022 02:04:36 GMT  
		Size: 4.7 MB (4747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbf0bfd3ec1bfd4a66d3202aa908910aa9e5f89b165f050afbb9097f3bde374`  
		Last Modified: Wed, 14 Sep 2022 02:04:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945863be2e4a3b708b817104df1efb5273b99ae8a8d63e7ce124aca615b90252`  
		Last Modified: Wed, 14 Sep 2022 02:04:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dabfac32e33fda6f8543e94730b92bea339bbc2be44525f8a98a2430811f1259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396eee83acf2b887d489bf2916c0f421b5f8b7c76b97c45b924a8e9b38885c47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 15:32:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 15:32:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 15:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 15:32:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 15:32:35 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 15:32:36 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 15:32:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 15:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 15:32:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a2b3a10608f3f1c16f3961525be3093dfac72b60edafff4713a5c36f4a47f`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8952ae8072f5f7b566992352417ca75e515ad92d7f379c654063cee0d1025bc6`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a0dc92476ccd6b2587e63791367f000f63bd9cd44a71ba525f1dc932fdc40`  
		Last Modified: Tue, 13 Sep 2022 15:33:12 GMT  
		Size: 5.3 MB (5270148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d5179d139cbf869c35de3c13a17d7309f06b6c71e5d82d9783af2266481f5d`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe043e7289aba1dcde04e36faa3ea835d38ff5470029d1603ed4bfadfd32f88`  
		Last Modified: Tue, 13 Sep 2022 15:33:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:080a3ea980d3a0cea9e71e608daac41551810d1d1e864065d09d82c3c71c12f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40275724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdec6799a11241ff8e045278507ad92d1c51719d5d5fab38a06aee9786c347f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:38:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Sep 2022 13:38:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:38:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Sep 2022 13:38:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Sep 2022 13:38:32 GMT
VOLUME [/spiped]
# Tue, 13 Sep 2022 13:38:33 GMT
WORKDIR /spiped
# Tue, 13 Sep 2022 13:38:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 13:38:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db4432e37229888ed10498cbb73a3db7967d321668c0fe3a5ff19544ce4058b`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf7f2aa932c3b1343a7a5582ac1b2615872e7bb6de032c757ff8c82697b9cb`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd929440d2f3ee4d86d6505d860ea41e1afa4ec703c48d3a37bc788e6fa735ba`  
		Last Modified: Tue, 13 Sep 2022 13:39:08 GMT  
		Size: 7.9 MB (7888964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5899589487bc133bfdd2d1e78feb31137bbb2802f6d9c4b9ea3922107efe7ef`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe3cf381a26f3297bd9b2623ae878e93eca5772348ca35a0ebc631182724a`  
		Last Modified: Tue, 13 Sep 2022 13:39:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:69da557a701cec978d7b047fcb58b719bc7f73002471092a81156d0ebfc911ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8b856a250d8d3b23ac7e8f3c688d644218eaff92a75e5b7969f1a0ea9c5978`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:18:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Sep 2022 00:19:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:19:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Sep 2022 00:20:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Sep 2022 00:20:45 GMT
VOLUME [/spiped]
# Wed, 14 Sep 2022 00:20:48 GMT
WORKDIR /spiped
# Wed, 14 Sep 2022 00:20:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Sep 2022 00:20:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:20:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453fe9f8f8eeeeac37559150e10691371c767d2109c6c4707ad80c6c81525a5b`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e231dc6f2975ea71e13f71ce249ea36cc1f5b9bc29cf4edb6cb221363a4f9c`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786f0306fa7c793bd8899c30db3c7f7d094115ce42b9cf3743fd6f8314f20ad`  
		Last Modified: Wed, 14 Sep 2022 00:21:17 GMT  
		Size: 5.7 MB (5705126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8411ad45e2cd35b79183d1a54c5718128e54f95133894e7992f363e6e523153`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96301dfd97b62754754bc3f8e044510f2914826da061612de4a79bc2f4e3422`  
		Last Modified: Wed, 14 Sep 2022 00:21:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:219e13c963456313e7f3d64811d97d01c472ed6f8a8d5bf55ee454e85b830cca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dcc529b0d26759e97fa2275e79e6f6e5058f2dfd6496402025839ba28ebf0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:23:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 08:23:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:23:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 08:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 08:24:33 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 08:24:33 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 08:24:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:24:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 08:24:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f18e563d25d3c5678e671e27753e3401c7b1ce8b60d60e5ba74ff1a5b858efe`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce19254f672d95be371e0158b1c728d3190e4c0561a7a533c9100fcbaffdeb`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b10a8dacb14f17077045d2e167303c50da8950371763ecb50c3886473fa2f`  
		Last Modified: Wed, 05 Oct 2022 08:25:11 GMT  
		Size: 6.0 MB (5998253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfe8808d03f72c63cf023c8a969140f3f940b2c718f2d2b518ec0cf6427077`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919707dce66a31120cdb5e4f928e6741464a96036f4d2076533bd94f81789bd`  
		Last Modified: Wed, 05 Oct 2022 08:25:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a6d6dc4c4fe5489f96d3eb044c7239d7528ebc7ee73337c3c53f0e15dccd3069
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34840409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14179e00a209732b609dfcc1b387f488c420760228b4dffb6675104fe0b2b9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 03:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:25:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 03:25:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 03:25:58 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 03:25:58 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 03:25:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:25:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:25:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af006c53786c75badcea31a45fa2e8e9bb3ab687d59cc0727fd2c48e18cbf76a`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb4dbf0ea8ead55cceb2c17b6d3faff2c5bf1d95624ed864dd0f305dfc6024d`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66f607cb7e14fb758c615f74a452a8669ccd26b30bbe549c175af95f900244`  
		Last Modified: Wed, 05 Oct 2022 03:26:31 GMT  
		Size: 5.2 MB (5186434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2993ec9272e99c08c4475bbb91800a0f5764a8728cff535e33f02ad29214c3`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99234ee6be52665bc5df00130740b88f466b372811e0638a734211b3ffecddd`  
		Last Modified: Wed, 05 Oct 2022 03:26:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
