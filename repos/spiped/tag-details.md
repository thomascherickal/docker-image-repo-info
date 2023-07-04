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
$ docker pull spiped@sha256:f928473f4a25a4088f0257498bf9dea02300e338eb193e736dec2d1fb9154bbf
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
$ docker pull spiped@sha256:64c9ff6d4e90807fd06162f08c850797563f8a574f8d88c0e2177bba5343f9f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5caff7b7b3c368e50a4fe67474a9e454e570e0b9caf6a8fe447aea979e74ea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 03:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:14:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 03:14:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:14:32 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 03:14:32 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 03:14:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:14:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b92b5954cfa789f1b5a0f545fd5a9a7e46a792aefca79339341f124d855f4dc`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6444d4e339eab2f9fb3ed43a84bcf11ef6cd483c5053f3176367a1b14fff3c61`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 2.6 MB (2586434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1621f45212a870ec5dd0e4ef6e3378976c464c684c75ea52f65b4c9bb4ce8`  
		Last Modified: Tue, 04 Jul 2023 03:14:50 GMT  
		Size: 6.5 MB (6469003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71d68d11725a63267fb85323478f0f1b5fbda3319b518987790561b52c868e`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9f406c97cfa32a6fd2ae3bc84894bc16b4c74eee2cb342a8174a9a388f783`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:9b440bee75dd7f1e7f9d0e4cbbb2663e618d3e6a5fdc90d3e88f4af031e10796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867620d601095a8e8567c235e241e214f87f9a2fe7450c18bdfc0082e30cc5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:48:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:48:57 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:48:57 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:48:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:48:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8731f6ea8e41da978c9015e88d36b5917a2f6397f9132069cfbc125d7155d3`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8001b7ff14d8d35bc729550ecb3b02f0c53ecadc34c6b03a3535b339fa312`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 2.2 MB (2183972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cf1d352b21ae47c02a9b4657d918ab1054454f186ff9aab730d6cbaecf2ef5`  
		Last Modified: Wed, 14 Jun 2023 16:49:11 GMT  
		Size: 5.1 MB (5134893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccded95a3299daeabfb9850fa9b6a32204aa92961dd6288e83aa254778214432`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55e9caf413a408e12751cc865cc4e045a402f26c8d93524d831fdb0c0518f7b`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:30b5cbc3896fccc9352c469fcefd3f0c394afe7188f476730ef8a47d95ce0ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31723067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb60681760d439d2994426f6abeee60d90b4b4b63fde1c2000b715e2f3344b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:24 GMT
ADD file:e0cfa2ad9282d0f4647498eb8121e93a14380cf8da98ea55054b555c1533bfff in / 
# Mon, 12 Jun 2023 23:58:24 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:32:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:32:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:33:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:33:01 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:33:01 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:53c17f790ffc929ad5caba471fff88bccc04ac924bce8725b7a0349e2ca1acde`  
		Last Modified: Tue, 13 Jun 2023 00:03:45 GMT  
		Size: 24.8 MB (24801257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6ba319270a3bcefa828a485037c6f5f97aad3b53f81e7e6ad9c1383262710`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974039e6afa1c8198b3faaf97d47978b6020ea7ea3f37bbec3b871671e94300`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 2.0 MB (2043272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726afe3ebe0c48219cc3501b2ce061bd07e4bc54ce71cabcb7a3c14a5dff6e1`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 4.9 MB (4876941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702ebc89990308a116eb63ee03c99be16434bad89b65c4ee7622309b4af002b2`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804a58e1a7bdce1bfdf3c45c3e4756e7e7772624b50326aa58f5cfc036212bc3`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:556ca8f88ef7cc81403a9a97d0dd87ad757320e01e6f95a2522a1e484cbd8a87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37061466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e9f2acd14674c9a7a1532aa4d74d686a7be75fff598ab6a90b3255c9821c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:38:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 06:38:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:38:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 06:39:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 06:39:29 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 06:39:29 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 06:39:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:39:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f130b8e8cb6a295db062a4bbd961e61a2665697e73c689ac96183c240872c9`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742747b981049267ff027c5437b4368631be7b5a687e9c963ee77d09f7bd78b2`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 2.4 MB (2429788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4eb4de7b3cfe458146fa063dbe2fce0476cb0cfc426c84b4877b2782619fa3`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 5.5 MB (5477622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c07ebf28daed63c65f5c1c0c32d379413c009c45813f2820a71fdee4c94fc4`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb28d7721e6f6a19bee631d7041934ff8e5db42d32cbeea54c91b8f701f043c`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:6d43aa8eebb100dc3902b2eaa5f40157469896c21bd164f77a06f3026a93c0d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38665743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993cd2fb56db3a2adeeb9114bffeae8eebba23542470b19cb60f7cdce843e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:38:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:39:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:39:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:39:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:39:34 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:39:34 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:39:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:39:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685167f1ee90548b2f936c06be0065bf15d334019d1e813cda5976a5faac51c`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356b3aaf212a1206664cfa580d6494f684712648172e626a5763e533f2c299d`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 2.6 MB (2583523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ce596d3d2605c349675410e1dfb1fca82b059b70aff89bf88ffc1fc97db9d5`  
		Last Modified: Wed, 14 Jun 2023 16:39:46 GMT  
		Size: 5.9 MB (5939881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d386251a97c8b66dba4287f8f25b1c909088233cadccdf0e309f8eaa985ad4a`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb9777f0312b075ad06ae71992bbb8bcc27c8bf98e792b890b735d9bb363ab`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:50832426d7cb80d309089d746661f34c44035d7e84bd18b7fcb4723ff1997d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36751873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69867d0746d2fd9d2480898e231157b8f393d8f2494a99e7a366a96048090c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:07:47 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:09:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:09:45 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:09:48 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:09:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:09:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db93178c77bcf3593248cad8b6debe8211f889bab334155486932dcdda101114`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf95eb82740eff246297f431c228de764d013565cb9ecf1e4dcedb0d520b534`  
		Last Modified: Wed, 14 Jun 2023 17:10:17 GMT  
		Size: 1.8 MB (1831650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1200cbabde345fbda9a6bbc760be93debd257049c125a67b59e79f1c555ae8`  
		Last Modified: Wed, 14 Jun 2023 17:10:20 GMT  
		Size: 5.8 MB (5800581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f3295ef8123cce31a6f517bef21b5685b9fea7f14b9869d286d0a18a359f33`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92a5c67d2822f5a3bb9b16dfa8366ab2138da333657bc937313ab8bda4e687f`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:f442dd454e56427ca33cb68a25d0a2ce387abcb81ca2070b5366e3f18d67c71e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42302809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4d6c06c55a4f1d2d84745e1910b74b5b60ccd5d5ac8b65cbe89c9d741ade45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:16:53 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:17:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:17:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:17:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:17:49 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:17:49 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:17:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:17:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ba44a5f009fb88ac04074f22f429b6a2b2af33d421b72db5cca0d672c71c2`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f9739d0b82c3102ad8e4d8d7077bca691e114e60870be5667589758e19dce9`  
		Last Modified: Wed, 14 Jun 2023 16:18:14 GMT  
		Size: 2.8 MB (2764939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002910d3fc58c5a9633efc7916165b4d36ce0111cd382c9a8961532731eb3c4b`  
		Last Modified: Wed, 14 Jun 2023 16:18:15 GMT  
		Size: 6.4 MB (6419551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ce6d2ff5db3cde73486e9687d83ec5c5018b427354a99801e5cc76f85d7c99`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceae632d9532021a35833afdf67e328b295eec28535fdc00f40db00d7f1b4be`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:7da21e08b694c65fccd8bd9db69ad2f20813743d119ee28dc199d12fb9dc3028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35129685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e8f381b5476bc8e56f26338b037055a33cc30082f7f78dcfb3ed05fe124662`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 17:32:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 15 Jun 2023 17:32:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 15 Jun 2023 17:32:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:33:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 15 Jun 2023 17:33:06 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:33:06 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:33:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56005098175a3f774a51986990ea797e5c84e146dbba376788635dfff9883d0d`  
		Last Modified: Thu, 15 Jun 2023 17:39:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e66f9f2f9f8e8b78cd7100f536392d10d1f3e77b071f0f34672c9b46413d22`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 2.3 MB (2257953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb80d8c82f6c1399d6b56aed13f0a3b145fb5d3d4bed63fe7fe0c86051890b9`  
		Last Modified: Thu, 15 Jun 2023 17:39:22 GMT  
		Size: 5.4 MB (5382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cb16cc5602b4e3f0fed2448ba36f83a4d8a7722477985c0952f5e7fa485c56`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71f6513b8c3f865bc1564ec946f9af84c82a10111dc2a5a1401b289fe455dc`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e1b7c497848f6c414b718267c003c183a28c1d2d7bafd57382329cf3703f5a51
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
$ docker pull spiped@sha256:b30ffb11062d050f5e82aaf7d78c68bfba0145bcaf9d552e60e5d4a1ff989f01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22627799e7a16dc63c4a87f5a10aab25a0208b38b355991ec5c1746ba6e307f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:22:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 04:22:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 04:22:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 04:22:19 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 04:22:19 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 04:22:19 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 04:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:22:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7009e83c06c17eb996625171bf08b8b88dfc800b7110240cee783b8df3bdab`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968c07669fd5c8684973e30777b3d7aa561332751af2fbaa4d903a96942787f`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 1.5 MB (1483166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb34038a914a6100cd46d4fc4ba06b2406f05cb528f07affe5cf1d0bcc3f012e`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 221.3 KB (221304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3bb3dbe0ec4d1442cc10f5a9d0dfc971ced50a1b024748a0441f7717259a62`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865d54f1b59ecbcdd28db4a8ed51db52bced0b9103c08b4e3bd60d9ab5092ea`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:06db8f6e615702076a78b5544ab4972b3d852851a43606bcff093be29bae66a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4558718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acff564be060667f5e783e1a68645d35ad3986c948318d77a247b6669f8e22d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:21:32 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:21:34 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:21:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:21:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:21:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:21:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:21:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:21:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:21:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db263a5aca0de0797095f3bd22056067e9842fc931f78f7ae95d38a25236c185`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31a87286e0f4dd73f465a80b19111ac981d83ea1469375bd2531510958a9b9`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.2 MB (1239671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cdb69483917a1a97a1e4517bf749631474cd4947b581bf545fc8ec922d82e3`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 206.4 KB (206394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ffc82f232844968ce89b84e87c160a076403e5187688166db3012478b0ee8f`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b99c8d7cfe4e601948b514fd305b8847633003b25cef4243a97e5e6349e033c`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:69eaa2a0c21e8170650365f7d40d3a7c233b81d7661ece405dcca3b032e1bb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7dde6285f1cdcbb4a49836abd7fa495595c255ae308325befc9aaee20f12ce9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:40:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 05:40:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 05:40:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 05:40:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 05:40:33 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 05:40:33 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 05:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 05:40:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 05:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37196072c4a2a985d715b1ad2657cf1978ca9533fc1e523c12b328715e0b45d5`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c46b5d561cfca9315d84fc298ad4d230bdc1a7cf8bd49a1249df54078185`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.2 MB (1166836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf9facf339fdeab9ce293f598a0921e55287c3b97644313fe1f8cc691a0eda`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 200.1 KB (200145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49e7526be5915de8b82401cadb9a075e97c38dc51550ef1b5d3377544cb685`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c7d118f25d5783b96754c98b6ec37c70b99f774f36ebf6beecdf0db3bfd9e0`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39b5750e18a31bff98637650ea090af4ebc2d29f321aeaf965038c4e2a11c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4841122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394fb835324ff4abcf12b18a1d05aa12b83540c07cc3241c429d63e413d753f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:08:11 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 07:08:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 07:08:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 07:08:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:08:20 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 07:08:20 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 07:08:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:08:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6ff8e6bcf8348815f9192563a0933c7bc36aa5d93a52b5258a1a07b53b55f0`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248e544999c4dd4330d208a807fcd37535d8118fd64bcca8b650bd19e40426f`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 1.4 MB (1362530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1e61b9ecdab1e8cdd80bf9885ebfaaf129ac359a883b68cf2b4dfb4eeeb56`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 215.7 KB (215717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa66ada810775bdb91cc1b2e9a36c42109d101de16f2e51bd1cf29a3e818690`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be54027b5c58467b7d758c1d7fc00b3569858d0fa4f8762f9a0097939e0218f1`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a0ef5e3831fe6edff2cbb0e86a938d1221c7cb3722165a2d84a75bb80c331700
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bda906f8180f69c7a88e6bb9dd0306173696c2dfdb7ea927ee728006fc8806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:19:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:19:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:19:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:19:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:19:36 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:19:36 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:19:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:19:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6dc9f335c57afbc7b1e16495708b766aea73dd4a701c48f8224c9969059fe6`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173a46948db93064f235acd48f05a36d8367fddd933d24bd195f318e84c8e88`  
		Last Modified: Thu, 15 Jun 2023 06:19:50 GMT  
		Size: 1.5 MB (1485192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf49c77ef03f39d9e293ebf197f230f3d09bd0dbcb18574059bfaa8a4e1023`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 231.6 KB (231638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434ea8ac7b673d5a898062b978fcf0b4eee889fe01aa4cdfc06a430063672d`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb416f535d69f288a9157a121afd70395a1694248283a278a68424ad083d83`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:07ecd79bdc7a73cc105de98257e8352a6bbc78539c96c60e473a591118cdda19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5023242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fa10dec34d7740e8f6b2e886e38be9267b07f9095199b6a90e5a3c788b983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 11:48:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 11:48:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 11:48:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 11:48:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 11:48:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 11:48:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 11:48:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 11:48:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 11:48:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb229d3396558a9569778f23d7302b803f3a32894ac72bb66aaa18d7763b75`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1b258a7d74d686736b6459d63f65e7b84802c25eb69c14593c702eeaa36ab`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 1.4 MB (1411537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427ace77d047161132485d0d1e849e6313bfd3ac5906bdc5c1a14581ec615eef`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 220.1 KB (220063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2245c7f6798c644fb92a427974afb750eff040bedc67839f23f819021b988e3`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2beec732ed9fea5742f56cb7c9fc3dcf72541cb5df22e9e59570e15f9e953e0`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:557bc9f87a1e1bc52642bb8952d0a879ac5593a353c14796cddddb156582cb3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4606776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62d68f98632f8097320aac6902f7c602c1dcffd7a6bdae0b0673d9543a6c0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 17:34:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 17:34:18 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 17:34:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:34:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 17:34:24 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:34:24 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:34:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:34:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:34:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5897952b7e299dca2b896d423bfda7066b1acf478f8cc0e7913cbd37a49389`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06405603908eb28e88f899138f60655b0e1f1f3f8e70dbeef03e6548c4a45ddf`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.2 MB (1221484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8625783f9b107b57ae6b8ab2323a93270e807b4525dec5b9f73667ed5b0aa9`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 208.7 KB (208656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d5c1789ad20269529284a4f65d9b868bdac4d431802fe12c463e47fb289b7`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdbe4b7a1197ad5630c73bd6de30fc339c371645e88f9859514654b6dd44ee`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:f928473f4a25a4088f0257498bf9dea02300e338eb193e736dec2d1fb9154bbf
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
$ docker pull spiped@sha256:64c9ff6d4e90807fd06162f08c850797563f8a574f8d88c0e2177bba5343f9f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5caff7b7b3c368e50a4fe67474a9e454e570e0b9caf6a8fe447aea979e74ea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 03:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:14:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 03:14:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:14:32 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 03:14:32 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 03:14:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:14:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b92b5954cfa789f1b5a0f545fd5a9a7e46a792aefca79339341f124d855f4dc`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6444d4e339eab2f9fb3ed43a84bcf11ef6cd483c5053f3176367a1b14fff3c61`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 2.6 MB (2586434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1621f45212a870ec5dd0e4ef6e3378976c464c684c75ea52f65b4c9bb4ce8`  
		Last Modified: Tue, 04 Jul 2023 03:14:50 GMT  
		Size: 6.5 MB (6469003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71d68d11725a63267fb85323478f0f1b5fbda3319b518987790561b52c868e`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9f406c97cfa32a6fd2ae3bc84894bc16b4c74eee2cb342a8174a9a388f783`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:9b440bee75dd7f1e7f9d0e4cbbb2663e618d3e6a5fdc90d3e88f4af031e10796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867620d601095a8e8567c235e241e214f87f9a2fe7450c18bdfc0082e30cc5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:48:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:48:57 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:48:57 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:48:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:48:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8731f6ea8e41da978c9015e88d36b5917a2f6397f9132069cfbc125d7155d3`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8001b7ff14d8d35bc729550ecb3b02f0c53ecadc34c6b03a3535b339fa312`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 2.2 MB (2183972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cf1d352b21ae47c02a9b4657d918ab1054454f186ff9aab730d6cbaecf2ef5`  
		Last Modified: Wed, 14 Jun 2023 16:49:11 GMT  
		Size: 5.1 MB (5134893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccded95a3299daeabfb9850fa9b6a32204aa92961dd6288e83aa254778214432`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55e9caf413a408e12751cc865cc4e045a402f26c8d93524d831fdb0c0518f7b`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:30b5cbc3896fccc9352c469fcefd3f0c394afe7188f476730ef8a47d95ce0ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31723067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb60681760d439d2994426f6abeee60d90b4b4b63fde1c2000b715e2f3344b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:24 GMT
ADD file:e0cfa2ad9282d0f4647498eb8121e93a14380cf8da98ea55054b555c1533bfff in / 
# Mon, 12 Jun 2023 23:58:24 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:32:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:32:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:33:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:33:01 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:33:01 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:53c17f790ffc929ad5caba471fff88bccc04ac924bce8725b7a0349e2ca1acde`  
		Last Modified: Tue, 13 Jun 2023 00:03:45 GMT  
		Size: 24.8 MB (24801257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6ba319270a3bcefa828a485037c6f5f97aad3b53f81e7e6ad9c1383262710`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974039e6afa1c8198b3faaf97d47978b6020ea7ea3f37bbec3b871671e94300`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 2.0 MB (2043272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726afe3ebe0c48219cc3501b2ce061bd07e4bc54ce71cabcb7a3c14a5dff6e1`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 4.9 MB (4876941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702ebc89990308a116eb63ee03c99be16434bad89b65c4ee7622309b4af002b2`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804a58e1a7bdce1bfdf3c45c3e4756e7e7772624b50326aa58f5cfc036212bc3`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:556ca8f88ef7cc81403a9a97d0dd87ad757320e01e6f95a2522a1e484cbd8a87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37061466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e9f2acd14674c9a7a1532aa4d74d686a7be75fff598ab6a90b3255c9821c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:38:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 06:38:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:38:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 06:39:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 06:39:29 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 06:39:29 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 06:39:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:39:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f130b8e8cb6a295db062a4bbd961e61a2665697e73c689ac96183c240872c9`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742747b981049267ff027c5437b4368631be7b5a687e9c963ee77d09f7bd78b2`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 2.4 MB (2429788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4eb4de7b3cfe458146fa063dbe2fce0476cb0cfc426c84b4877b2782619fa3`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 5.5 MB (5477622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c07ebf28daed63c65f5c1c0c32d379413c009c45813f2820a71fdee4c94fc4`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb28d7721e6f6a19bee631d7041934ff8e5db42d32cbeea54c91b8f701f043c`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:6d43aa8eebb100dc3902b2eaa5f40157469896c21bd164f77a06f3026a93c0d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38665743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993cd2fb56db3a2adeeb9114bffeae8eebba23542470b19cb60f7cdce843e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:38:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:39:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:39:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:39:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:39:34 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:39:34 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:39:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:39:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685167f1ee90548b2f936c06be0065bf15d334019d1e813cda5976a5faac51c`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356b3aaf212a1206664cfa580d6494f684712648172e626a5763e533f2c299d`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 2.6 MB (2583523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ce596d3d2605c349675410e1dfb1fca82b059b70aff89bf88ffc1fc97db9d5`  
		Last Modified: Wed, 14 Jun 2023 16:39:46 GMT  
		Size: 5.9 MB (5939881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d386251a97c8b66dba4287f8f25b1c909088233cadccdf0e309f8eaa985ad4a`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb9777f0312b075ad06ae71992bbb8bcc27c8bf98e792b890b735d9bb363ab`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:50832426d7cb80d309089d746661f34c44035d7e84bd18b7fcb4723ff1997d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36751873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69867d0746d2fd9d2480898e231157b8f393d8f2494a99e7a366a96048090c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:07:47 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:09:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:09:45 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:09:48 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:09:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:09:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db93178c77bcf3593248cad8b6debe8211f889bab334155486932dcdda101114`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf95eb82740eff246297f431c228de764d013565cb9ecf1e4dcedb0d520b534`  
		Last Modified: Wed, 14 Jun 2023 17:10:17 GMT  
		Size: 1.8 MB (1831650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1200cbabde345fbda9a6bbc760be93debd257049c125a67b59e79f1c555ae8`  
		Last Modified: Wed, 14 Jun 2023 17:10:20 GMT  
		Size: 5.8 MB (5800581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f3295ef8123cce31a6f517bef21b5685b9fea7f14b9869d286d0a18a359f33`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92a5c67d2822f5a3bb9b16dfa8366ab2138da333657bc937313ab8bda4e687f`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:f442dd454e56427ca33cb68a25d0a2ce387abcb81ca2070b5366e3f18d67c71e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42302809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4d6c06c55a4f1d2d84745e1910b74b5b60ccd5d5ac8b65cbe89c9d741ade45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:16:53 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:17:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:17:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:17:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:17:49 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:17:49 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:17:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:17:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ba44a5f009fb88ac04074f22f429b6a2b2af33d421b72db5cca0d672c71c2`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f9739d0b82c3102ad8e4d8d7077bca691e114e60870be5667589758e19dce9`  
		Last Modified: Wed, 14 Jun 2023 16:18:14 GMT  
		Size: 2.8 MB (2764939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002910d3fc58c5a9633efc7916165b4d36ce0111cd382c9a8961532731eb3c4b`  
		Last Modified: Wed, 14 Jun 2023 16:18:15 GMT  
		Size: 6.4 MB (6419551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ce6d2ff5db3cde73486e9687d83ec5c5018b427354a99801e5cc76f85d7c99`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceae632d9532021a35833afdf67e328b295eec28535fdc00f40db00d7f1b4be`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:7da21e08b694c65fccd8bd9db69ad2f20813743d119ee28dc199d12fb9dc3028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35129685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e8f381b5476bc8e56f26338b037055a33cc30082f7f78dcfb3ed05fe124662`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 17:32:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 15 Jun 2023 17:32:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 15 Jun 2023 17:32:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:33:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 15 Jun 2023 17:33:06 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:33:06 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:33:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56005098175a3f774a51986990ea797e5c84e146dbba376788635dfff9883d0d`  
		Last Modified: Thu, 15 Jun 2023 17:39:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e66f9f2f9f8e8b78cd7100f536392d10d1f3e77b071f0f34672c9b46413d22`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 2.3 MB (2257953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb80d8c82f6c1399d6b56aed13f0a3b145fb5d3d4bed63fe7fe0c86051890b9`  
		Last Modified: Thu, 15 Jun 2023 17:39:22 GMT  
		Size: 5.4 MB (5382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cb16cc5602b4e3f0fed2448ba36f83a4d8a7722477985c0952f5e7fa485c56`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71f6513b8c3f865bc1564ec946f9af84c82a10111dc2a5a1401b289fe455dc`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e1b7c497848f6c414b718267c003c183a28c1d2d7bafd57382329cf3703f5a51
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
$ docker pull spiped@sha256:b30ffb11062d050f5e82aaf7d78c68bfba0145bcaf9d552e60e5d4a1ff989f01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22627799e7a16dc63c4a87f5a10aab25a0208b38b355991ec5c1746ba6e307f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:22:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 04:22:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 04:22:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 04:22:19 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 04:22:19 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 04:22:19 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 04:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:22:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7009e83c06c17eb996625171bf08b8b88dfc800b7110240cee783b8df3bdab`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968c07669fd5c8684973e30777b3d7aa561332751af2fbaa4d903a96942787f`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 1.5 MB (1483166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb34038a914a6100cd46d4fc4ba06b2406f05cb528f07affe5cf1d0bcc3f012e`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 221.3 KB (221304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3bb3dbe0ec4d1442cc10f5a9d0dfc971ced50a1b024748a0441f7717259a62`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865d54f1b59ecbcdd28db4a8ed51db52bced0b9103c08b4e3bd60d9ab5092ea`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:06db8f6e615702076a78b5544ab4972b3d852851a43606bcff093be29bae66a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4558718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acff564be060667f5e783e1a68645d35ad3986c948318d77a247b6669f8e22d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:21:32 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:21:34 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:21:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:21:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:21:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:21:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:21:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:21:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:21:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db263a5aca0de0797095f3bd22056067e9842fc931f78f7ae95d38a25236c185`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31a87286e0f4dd73f465a80b19111ac981d83ea1469375bd2531510958a9b9`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.2 MB (1239671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cdb69483917a1a97a1e4517bf749631474cd4947b581bf545fc8ec922d82e3`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 206.4 KB (206394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ffc82f232844968ce89b84e87c160a076403e5187688166db3012478b0ee8f`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b99c8d7cfe4e601948b514fd305b8847633003b25cef4243a97e5e6349e033c`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:69eaa2a0c21e8170650365f7d40d3a7c233b81d7661ece405dcca3b032e1bb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7dde6285f1cdcbb4a49836abd7fa495595c255ae308325befc9aaee20f12ce9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:40:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 05:40:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 05:40:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 05:40:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 05:40:33 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 05:40:33 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 05:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 05:40:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 05:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37196072c4a2a985d715b1ad2657cf1978ca9533fc1e523c12b328715e0b45d5`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c46b5d561cfca9315d84fc298ad4d230bdc1a7cf8bd49a1249df54078185`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.2 MB (1166836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf9facf339fdeab9ce293f598a0921e55287c3b97644313fe1f8cc691a0eda`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 200.1 KB (200145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49e7526be5915de8b82401cadb9a075e97c38dc51550ef1b5d3377544cb685`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c7d118f25d5783b96754c98b6ec37c70b99f774f36ebf6beecdf0db3bfd9e0`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39b5750e18a31bff98637650ea090af4ebc2d29f321aeaf965038c4e2a11c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4841122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394fb835324ff4abcf12b18a1d05aa12b83540c07cc3241c429d63e413d753f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:08:11 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 07:08:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 07:08:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 07:08:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:08:20 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 07:08:20 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 07:08:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:08:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6ff8e6bcf8348815f9192563a0933c7bc36aa5d93a52b5258a1a07b53b55f0`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248e544999c4dd4330d208a807fcd37535d8118fd64bcca8b650bd19e40426f`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 1.4 MB (1362530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1e61b9ecdab1e8cdd80bf9885ebfaaf129ac359a883b68cf2b4dfb4eeeb56`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 215.7 KB (215717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa66ada810775bdb91cc1b2e9a36c42109d101de16f2e51bd1cf29a3e818690`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be54027b5c58467b7d758c1d7fc00b3569858d0fa4f8762f9a0097939e0218f1`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a0ef5e3831fe6edff2cbb0e86a938d1221c7cb3722165a2d84a75bb80c331700
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bda906f8180f69c7a88e6bb9dd0306173696c2dfdb7ea927ee728006fc8806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:19:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:19:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:19:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:19:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:19:36 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:19:36 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:19:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:19:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6dc9f335c57afbc7b1e16495708b766aea73dd4a701c48f8224c9969059fe6`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173a46948db93064f235acd48f05a36d8367fddd933d24bd195f318e84c8e88`  
		Last Modified: Thu, 15 Jun 2023 06:19:50 GMT  
		Size: 1.5 MB (1485192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf49c77ef03f39d9e293ebf197f230f3d09bd0dbcb18574059bfaa8a4e1023`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 231.6 KB (231638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434ea8ac7b673d5a898062b978fcf0b4eee889fe01aa4cdfc06a430063672d`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb416f535d69f288a9157a121afd70395a1694248283a278a68424ad083d83`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:07ecd79bdc7a73cc105de98257e8352a6bbc78539c96c60e473a591118cdda19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5023242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fa10dec34d7740e8f6b2e886e38be9267b07f9095199b6a90e5a3c788b983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 11:48:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 11:48:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 11:48:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 11:48:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 11:48:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 11:48:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 11:48:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 11:48:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 11:48:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb229d3396558a9569778f23d7302b803f3a32894ac72bb66aaa18d7763b75`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1b258a7d74d686736b6459d63f65e7b84802c25eb69c14593c702eeaa36ab`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 1.4 MB (1411537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427ace77d047161132485d0d1e849e6313bfd3ac5906bdc5c1a14581ec615eef`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 220.1 KB (220063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2245c7f6798c644fb92a427974afb750eff040bedc67839f23f819021b988e3`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2beec732ed9fea5742f56cb7c9fc3dcf72541cb5df22e9e59570e15f9e953e0`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:557bc9f87a1e1bc52642bb8952d0a879ac5593a353c14796cddddb156582cb3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4606776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62d68f98632f8097320aac6902f7c602c1dcffd7a6bdae0b0673d9543a6c0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 17:34:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 17:34:18 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 17:34:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:34:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 17:34:24 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:34:24 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:34:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:34:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:34:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5897952b7e299dca2b896d423bfda7066b1acf478f8cc0e7913cbd37a49389`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06405603908eb28e88f899138f60655b0e1f1f3f8e70dbeef03e6548c4a45ddf`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.2 MB (1221484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8625783f9b107b57ae6b8ab2323a93270e807b4525dec5b9f73667ed5b0aa9`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 208.7 KB (208656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d5c1789ad20269529284a4f65d9b868bdac4d431802fe12c463e47fb289b7`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdbe4b7a1197ad5630c73bd6de30fc339c371645e88f9859514654b6dd44ee`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:f928473f4a25a4088f0257498bf9dea02300e338eb193e736dec2d1fb9154bbf
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
$ docker pull spiped@sha256:64c9ff6d4e90807fd06162f08c850797563f8a574f8d88c0e2177bba5343f9f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5caff7b7b3c368e50a4fe67474a9e454e570e0b9caf6a8fe447aea979e74ea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 03:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:14:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 03:14:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:14:32 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 03:14:32 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 03:14:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:14:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b92b5954cfa789f1b5a0f545fd5a9a7e46a792aefca79339341f124d855f4dc`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6444d4e339eab2f9fb3ed43a84bcf11ef6cd483c5053f3176367a1b14fff3c61`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 2.6 MB (2586434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1621f45212a870ec5dd0e4ef6e3378976c464c684c75ea52f65b4c9bb4ce8`  
		Last Modified: Tue, 04 Jul 2023 03:14:50 GMT  
		Size: 6.5 MB (6469003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71d68d11725a63267fb85323478f0f1b5fbda3319b518987790561b52c868e`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9f406c97cfa32a6fd2ae3bc84894bc16b4c74eee2cb342a8174a9a388f783`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:9b440bee75dd7f1e7f9d0e4cbbb2663e618d3e6a5fdc90d3e88f4af031e10796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867620d601095a8e8567c235e241e214f87f9a2fe7450c18bdfc0082e30cc5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:48:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:48:57 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:48:57 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:48:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:48:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8731f6ea8e41da978c9015e88d36b5917a2f6397f9132069cfbc125d7155d3`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8001b7ff14d8d35bc729550ecb3b02f0c53ecadc34c6b03a3535b339fa312`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 2.2 MB (2183972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cf1d352b21ae47c02a9b4657d918ab1054454f186ff9aab730d6cbaecf2ef5`  
		Last Modified: Wed, 14 Jun 2023 16:49:11 GMT  
		Size: 5.1 MB (5134893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccded95a3299daeabfb9850fa9b6a32204aa92961dd6288e83aa254778214432`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55e9caf413a408e12751cc865cc4e045a402f26c8d93524d831fdb0c0518f7b`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:30b5cbc3896fccc9352c469fcefd3f0c394afe7188f476730ef8a47d95ce0ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31723067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb60681760d439d2994426f6abeee60d90b4b4b63fde1c2000b715e2f3344b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:24 GMT
ADD file:e0cfa2ad9282d0f4647498eb8121e93a14380cf8da98ea55054b555c1533bfff in / 
# Mon, 12 Jun 2023 23:58:24 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:32:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:32:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:33:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:33:01 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:33:01 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:53c17f790ffc929ad5caba471fff88bccc04ac924bce8725b7a0349e2ca1acde`  
		Last Modified: Tue, 13 Jun 2023 00:03:45 GMT  
		Size: 24.8 MB (24801257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6ba319270a3bcefa828a485037c6f5f97aad3b53f81e7e6ad9c1383262710`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974039e6afa1c8198b3faaf97d47978b6020ea7ea3f37bbec3b871671e94300`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 2.0 MB (2043272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726afe3ebe0c48219cc3501b2ce061bd07e4bc54ce71cabcb7a3c14a5dff6e1`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 4.9 MB (4876941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702ebc89990308a116eb63ee03c99be16434bad89b65c4ee7622309b4af002b2`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804a58e1a7bdce1bfdf3c45c3e4756e7e7772624b50326aa58f5cfc036212bc3`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:556ca8f88ef7cc81403a9a97d0dd87ad757320e01e6f95a2522a1e484cbd8a87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37061466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e9f2acd14674c9a7a1532aa4d74d686a7be75fff598ab6a90b3255c9821c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:38:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 06:38:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:38:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 06:39:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 06:39:29 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 06:39:29 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 06:39:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:39:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f130b8e8cb6a295db062a4bbd961e61a2665697e73c689ac96183c240872c9`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742747b981049267ff027c5437b4368631be7b5a687e9c963ee77d09f7bd78b2`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 2.4 MB (2429788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4eb4de7b3cfe458146fa063dbe2fce0476cb0cfc426c84b4877b2782619fa3`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 5.5 MB (5477622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c07ebf28daed63c65f5c1c0c32d379413c009c45813f2820a71fdee4c94fc4`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb28d7721e6f6a19bee631d7041934ff8e5db42d32cbeea54c91b8f701f043c`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:6d43aa8eebb100dc3902b2eaa5f40157469896c21bd164f77a06f3026a93c0d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38665743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993cd2fb56db3a2adeeb9114bffeae8eebba23542470b19cb60f7cdce843e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:38:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:39:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:39:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:39:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:39:34 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:39:34 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:39:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:39:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685167f1ee90548b2f936c06be0065bf15d334019d1e813cda5976a5faac51c`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356b3aaf212a1206664cfa580d6494f684712648172e626a5763e533f2c299d`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 2.6 MB (2583523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ce596d3d2605c349675410e1dfb1fca82b059b70aff89bf88ffc1fc97db9d5`  
		Last Modified: Wed, 14 Jun 2023 16:39:46 GMT  
		Size: 5.9 MB (5939881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d386251a97c8b66dba4287f8f25b1c909088233cadccdf0e309f8eaa985ad4a`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb9777f0312b075ad06ae71992bbb8bcc27c8bf98e792b890b735d9bb363ab`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:50832426d7cb80d309089d746661f34c44035d7e84bd18b7fcb4723ff1997d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36751873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69867d0746d2fd9d2480898e231157b8f393d8f2494a99e7a366a96048090c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:07:47 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:09:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:09:45 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:09:48 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:09:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:09:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db93178c77bcf3593248cad8b6debe8211f889bab334155486932dcdda101114`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf95eb82740eff246297f431c228de764d013565cb9ecf1e4dcedb0d520b534`  
		Last Modified: Wed, 14 Jun 2023 17:10:17 GMT  
		Size: 1.8 MB (1831650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1200cbabde345fbda9a6bbc760be93debd257049c125a67b59e79f1c555ae8`  
		Last Modified: Wed, 14 Jun 2023 17:10:20 GMT  
		Size: 5.8 MB (5800581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f3295ef8123cce31a6f517bef21b5685b9fea7f14b9869d286d0a18a359f33`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92a5c67d2822f5a3bb9b16dfa8366ab2138da333657bc937313ab8bda4e687f`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:f442dd454e56427ca33cb68a25d0a2ce387abcb81ca2070b5366e3f18d67c71e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42302809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4d6c06c55a4f1d2d84745e1910b74b5b60ccd5d5ac8b65cbe89c9d741ade45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:16:53 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:17:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:17:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:17:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:17:49 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:17:49 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:17:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:17:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ba44a5f009fb88ac04074f22f429b6a2b2af33d421b72db5cca0d672c71c2`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f9739d0b82c3102ad8e4d8d7077bca691e114e60870be5667589758e19dce9`  
		Last Modified: Wed, 14 Jun 2023 16:18:14 GMT  
		Size: 2.8 MB (2764939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002910d3fc58c5a9633efc7916165b4d36ce0111cd382c9a8961532731eb3c4b`  
		Last Modified: Wed, 14 Jun 2023 16:18:15 GMT  
		Size: 6.4 MB (6419551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ce6d2ff5db3cde73486e9687d83ec5c5018b427354a99801e5cc76f85d7c99`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceae632d9532021a35833afdf67e328b295eec28535fdc00f40db00d7f1b4be`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:7da21e08b694c65fccd8bd9db69ad2f20813743d119ee28dc199d12fb9dc3028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35129685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e8f381b5476bc8e56f26338b037055a33cc30082f7f78dcfb3ed05fe124662`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 17:32:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 15 Jun 2023 17:32:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 15 Jun 2023 17:32:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:33:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 15 Jun 2023 17:33:06 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:33:06 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:33:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56005098175a3f774a51986990ea797e5c84e146dbba376788635dfff9883d0d`  
		Last Modified: Thu, 15 Jun 2023 17:39:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e66f9f2f9f8e8b78cd7100f536392d10d1f3e77b071f0f34672c9b46413d22`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 2.3 MB (2257953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb80d8c82f6c1399d6b56aed13f0a3b145fb5d3d4bed63fe7fe0c86051890b9`  
		Last Modified: Thu, 15 Jun 2023 17:39:22 GMT  
		Size: 5.4 MB (5382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cb16cc5602b4e3f0fed2448ba36f83a4d8a7722477985c0952f5e7fa485c56`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71f6513b8c3f865bc1564ec946f9af84c82a10111dc2a5a1401b289fe455dc`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e1b7c497848f6c414b718267c003c183a28c1d2d7bafd57382329cf3703f5a51
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
$ docker pull spiped@sha256:b30ffb11062d050f5e82aaf7d78c68bfba0145bcaf9d552e60e5d4a1ff989f01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22627799e7a16dc63c4a87f5a10aab25a0208b38b355991ec5c1746ba6e307f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:22:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 04:22:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 04:22:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 04:22:19 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 04:22:19 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 04:22:19 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 04:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:22:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7009e83c06c17eb996625171bf08b8b88dfc800b7110240cee783b8df3bdab`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968c07669fd5c8684973e30777b3d7aa561332751af2fbaa4d903a96942787f`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 1.5 MB (1483166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb34038a914a6100cd46d4fc4ba06b2406f05cb528f07affe5cf1d0bcc3f012e`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 221.3 KB (221304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3bb3dbe0ec4d1442cc10f5a9d0dfc971ced50a1b024748a0441f7717259a62`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865d54f1b59ecbcdd28db4a8ed51db52bced0b9103c08b4e3bd60d9ab5092ea`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:06db8f6e615702076a78b5544ab4972b3d852851a43606bcff093be29bae66a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4558718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acff564be060667f5e783e1a68645d35ad3986c948318d77a247b6669f8e22d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:21:32 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:21:34 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:21:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:21:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:21:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:21:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:21:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:21:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:21:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db263a5aca0de0797095f3bd22056067e9842fc931f78f7ae95d38a25236c185`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31a87286e0f4dd73f465a80b19111ac981d83ea1469375bd2531510958a9b9`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.2 MB (1239671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cdb69483917a1a97a1e4517bf749631474cd4947b581bf545fc8ec922d82e3`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 206.4 KB (206394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ffc82f232844968ce89b84e87c160a076403e5187688166db3012478b0ee8f`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b99c8d7cfe4e601948b514fd305b8847633003b25cef4243a97e5e6349e033c`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:69eaa2a0c21e8170650365f7d40d3a7c233b81d7661ece405dcca3b032e1bb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7dde6285f1cdcbb4a49836abd7fa495595c255ae308325befc9aaee20f12ce9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:40:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 05:40:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 05:40:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 05:40:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 05:40:33 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 05:40:33 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 05:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 05:40:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 05:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37196072c4a2a985d715b1ad2657cf1978ca9533fc1e523c12b328715e0b45d5`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c46b5d561cfca9315d84fc298ad4d230bdc1a7cf8bd49a1249df54078185`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.2 MB (1166836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf9facf339fdeab9ce293f598a0921e55287c3b97644313fe1f8cc691a0eda`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 200.1 KB (200145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49e7526be5915de8b82401cadb9a075e97c38dc51550ef1b5d3377544cb685`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c7d118f25d5783b96754c98b6ec37c70b99f774f36ebf6beecdf0db3bfd9e0`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39b5750e18a31bff98637650ea090af4ebc2d29f321aeaf965038c4e2a11c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4841122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394fb835324ff4abcf12b18a1d05aa12b83540c07cc3241c429d63e413d753f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:08:11 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 07:08:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 07:08:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 07:08:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:08:20 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 07:08:20 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 07:08:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:08:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6ff8e6bcf8348815f9192563a0933c7bc36aa5d93a52b5258a1a07b53b55f0`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248e544999c4dd4330d208a807fcd37535d8118fd64bcca8b650bd19e40426f`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 1.4 MB (1362530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1e61b9ecdab1e8cdd80bf9885ebfaaf129ac359a883b68cf2b4dfb4eeeb56`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 215.7 KB (215717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa66ada810775bdb91cc1b2e9a36c42109d101de16f2e51bd1cf29a3e818690`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be54027b5c58467b7d758c1d7fc00b3569858d0fa4f8762f9a0097939e0218f1`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a0ef5e3831fe6edff2cbb0e86a938d1221c7cb3722165a2d84a75bb80c331700
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bda906f8180f69c7a88e6bb9dd0306173696c2dfdb7ea927ee728006fc8806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:19:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:19:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:19:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:19:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:19:36 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:19:36 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:19:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:19:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6dc9f335c57afbc7b1e16495708b766aea73dd4a701c48f8224c9969059fe6`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173a46948db93064f235acd48f05a36d8367fddd933d24bd195f318e84c8e88`  
		Last Modified: Thu, 15 Jun 2023 06:19:50 GMT  
		Size: 1.5 MB (1485192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf49c77ef03f39d9e293ebf197f230f3d09bd0dbcb18574059bfaa8a4e1023`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 231.6 KB (231638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434ea8ac7b673d5a898062b978fcf0b4eee889fe01aa4cdfc06a430063672d`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb416f535d69f288a9157a121afd70395a1694248283a278a68424ad083d83`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:07ecd79bdc7a73cc105de98257e8352a6bbc78539c96c60e473a591118cdda19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5023242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fa10dec34d7740e8f6b2e886e38be9267b07f9095199b6a90e5a3c788b983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 11:48:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 11:48:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 11:48:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 11:48:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 11:48:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 11:48:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 11:48:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 11:48:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 11:48:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb229d3396558a9569778f23d7302b803f3a32894ac72bb66aaa18d7763b75`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1b258a7d74d686736b6459d63f65e7b84802c25eb69c14593c702eeaa36ab`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 1.4 MB (1411537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427ace77d047161132485d0d1e849e6313bfd3ac5906bdc5c1a14581ec615eef`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 220.1 KB (220063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2245c7f6798c644fb92a427974afb750eff040bedc67839f23f819021b988e3`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2beec732ed9fea5742f56cb7c9fc3dcf72541cb5df22e9e59570e15f9e953e0`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:557bc9f87a1e1bc52642bb8952d0a879ac5593a353c14796cddddb156582cb3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4606776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62d68f98632f8097320aac6902f7c602c1dcffd7a6bdae0b0673d9543a6c0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 17:34:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 17:34:18 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 17:34:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:34:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 17:34:24 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:34:24 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:34:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:34:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:34:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5897952b7e299dca2b896d423bfda7066b1acf478f8cc0e7913cbd37a49389`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06405603908eb28e88f899138f60655b0e1f1f3f8e70dbeef03e6548c4a45ddf`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.2 MB (1221484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8625783f9b107b57ae6b8ab2323a93270e807b4525dec5b9f73667ed5b0aa9`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 208.7 KB (208656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d5c1789ad20269529284a4f65d9b868bdac4d431802fe12c463e47fb289b7`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdbe4b7a1197ad5630c73bd6de30fc339c371645e88f9859514654b6dd44ee`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e1b7c497848f6c414b718267c003c183a28c1d2d7bafd57382329cf3703f5a51
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
$ docker pull spiped@sha256:b30ffb11062d050f5e82aaf7d78c68bfba0145bcaf9d552e60e5d4a1ff989f01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22627799e7a16dc63c4a87f5a10aab25a0208b38b355991ec5c1746ba6e307f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:22:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 04:22:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 04:22:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 04:22:19 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 04:22:19 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 04:22:19 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 04:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:22:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7009e83c06c17eb996625171bf08b8b88dfc800b7110240cee783b8df3bdab`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968c07669fd5c8684973e30777b3d7aa561332751af2fbaa4d903a96942787f`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 1.5 MB (1483166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb34038a914a6100cd46d4fc4ba06b2406f05cb528f07affe5cf1d0bcc3f012e`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 221.3 KB (221304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3bb3dbe0ec4d1442cc10f5a9d0dfc971ced50a1b024748a0441f7717259a62`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865d54f1b59ecbcdd28db4a8ed51db52bced0b9103c08b4e3bd60d9ab5092ea`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:06db8f6e615702076a78b5544ab4972b3d852851a43606bcff093be29bae66a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4558718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acff564be060667f5e783e1a68645d35ad3986c948318d77a247b6669f8e22d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:21:32 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:21:34 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:21:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:21:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:21:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:21:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:21:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:21:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:21:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db263a5aca0de0797095f3bd22056067e9842fc931f78f7ae95d38a25236c185`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31a87286e0f4dd73f465a80b19111ac981d83ea1469375bd2531510958a9b9`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.2 MB (1239671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cdb69483917a1a97a1e4517bf749631474cd4947b581bf545fc8ec922d82e3`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 206.4 KB (206394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ffc82f232844968ce89b84e87c160a076403e5187688166db3012478b0ee8f`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b99c8d7cfe4e601948b514fd305b8847633003b25cef4243a97e5e6349e033c`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:69eaa2a0c21e8170650365f7d40d3a7c233b81d7661ece405dcca3b032e1bb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7dde6285f1cdcbb4a49836abd7fa495595c255ae308325befc9aaee20f12ce9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:40:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 05:40:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 05:40:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 05:40:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 05:40:33 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 05:40:33 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 05:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 05:40:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 05:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37196072c4a2a985d715b1ad2657cf1978ca9533fc1e523c12b328715e0b45d5`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c46b5d561cfca9315d84fc298ad4d230bdc1a7cf8bd49a1249df54078185`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.2 MB (1166836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf9facf339fdeab9ce293f598a0921e55287c3b97644313fe1f8cc691a0eda`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 200.1 KB (200145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49e7526be5915de8b82401cadb9a075e97c38dc51550ef1b5d3377544cb685`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c7d118f25d5783b96754c98b6ec37c70b99f774f36ebf6beecdf0db3bfd9e0`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39b5750e18a31bff98637650ea090af4ebc2d29f321aeaf965038c4e2a11c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4841122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394fb835324ff4abcf12b18a1d05aa12b83540c07cc3241c429d63e413d753f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:08:11 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 07:08:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 07:08:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 07:08:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:08:20 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 07:08:20 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 07:08:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:08:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6ff8e6bcf8348815f9192563a0933c7bc36aa5d93a52b5258a1a07b53b55f0`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248e544999c4dd4330d208a807fcd37535d8118fd64bcca8b650bd19e40426f`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 1.4 MB (1362530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1e61b9ecdab1e8cdd80bf9885ebfaaf129ac359a883b68cf2b4dfb4eeeb56`  
		Last Modified: Thu, 15 Jun 2023 07:08:32 GMT  
		Size: 215.7 KB (215717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa66ada810775bdb91cc1b2e9a36c42109d101de16f2e51bd1cf29a3e818690`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be54027b5c58467b7d758c1d7fc00b3569858d0fa4f8762f9a0097939e0218f1`  
		Last Modified: Thu, 15 Jun 2023 07:08:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:a0ef5e3831fe6edff2cbb0e86a938d1221c7cb3722165a2d84a75bb80c331700
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bda906f8180f69c7a88e6bb9dd0306173696c2dfdb7ea927ee728006fc8806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:19:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:19:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:19:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:19:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:19:36 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:19:36 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:19:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:19:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6dc9f335c57afbc7b1e16495708b766aea73dd4a701c48f8224c9969059fe6`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173a46948db93064f235acd48f05a36d8367fddd933d24bd195f318e84c8e88`  
		Last Modified: Thu, 15 Jun 2023 06:19:50 GMT  
		Size: 1.5 MB (1485192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf49c77ef03f39d9e293ebf197f230f3d09bd0dbcb18574059bfaa8a4e1023`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 231.6 KB (231638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434ea8ac7b673d5a898062b978fcf0b4eee889fe01aa4cdfc06a430063672d`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb416f535d69f288a9157a121afd70395a1694248283a278a68424ad083d83`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:07ecd79bdc7a73cc105de98257e8352a6bbc78539c96c60e473a591118cdda19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5023242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fa10dec34d7740e8f6b2e886e38be9267b07f9095199b6a90e5a3c788b983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 11:48:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 11:48:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 11:48:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 11:48:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 11:48:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 11:48:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 11:48:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 11:48:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 11:48:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb229d3396558a9569778f23d7302b803f3a32894ac72bb66aaa18d7763b75`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1b258a7d74d686736b6459d63f65e7b84802c25eb69c14593c702eeaa36ab`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 1.4 MB (1411537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427ace77d047161132485d0d1e849e6313bfd3ac5906bdc5c1a14581ec615eef`  
		Last Modified: Thu, 15 Jun 2023 11:49:01 GMT  
		Size: 220.1 KB (220063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2245c7f6798c644fb92a427974afb750eff040bedc67839f23f819021b988e3`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2beec732ed9fea5742f56cb7c9fc3dcf72541cb5df22e9e59570e15f9e953e0`  
		Last Modified: Thu, 15 Jun 2023 11:49:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:557bc9f87a1e1bc52642bb8952d0a879ac5593a353c14796cddddb156582cb3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4606776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62d68f98632f8097320aac6902f7c602c1dcffd7a6bdae0b0673d9543a6c0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 17:34:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 17:34:18 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 17:34:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:34:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 17:34:24 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:34:24 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:34:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:34:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:34:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5897952b7e299dca2b896d423bfda7066b1acf478f8cc0e7913cbd37a49389`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06405603908eb28e88f899138f60655b0e1f1f3f8e70dbeef03e6548c4a45ddf`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 1.2 MB (1221484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8625783f9b107b57ae6b8ab2323a93270e807b4525dec5b9f73667ed5b0aa9`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 208.7 KB (208656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d5c1789ad20269529284a4f65d9b868bdac4d431802fe12c463e47fb289b7`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdbe4b7a1197ad5630c73bd6de30fc339c371645e88f9859514654b6dd44ee`  
		Last Modified: Thu, 15 Jun 2023 17:40:55 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:f928473f4a25a4088f0257498bf9dea02300e338eb193e736dec2d1fb9154bbf
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
$ docker pull spiped@sha256:64c9ff6d4e90807fd06162f08c850797563f8a574f8d88c0e2177bba5343f9f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5caff7b7b3c368e50a4fe67474a9e454e570e0b9caf6a8fe447aea979e74ea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 03:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:14:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 03:14:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:14:32 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 03:14:32 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 03:14:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:14:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b92b5954cfa789f1b5a0f545fd5a9a7e46a792aefca79339341f124d855f4dc`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6444d4e339eab2f9fb3ed43a84bcf11ef6cd483c5053f3176367a1b14fff3c61`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 2.6 MB (2586434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1621f45212a870ec5dd0e4ef6e3378976c464c684c75ea52f65b4c9bb4ce8`  
		Last Modified: Tue, 04 Jul 2023 03:14:50 GMT  
		Size: 6.5 MB (6469003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71d68d11725a63267fb85323478f0f1b5fbda3319b518987790561b52c868e`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9f406c97cfa32a6fd2ae3bc84894bc16b4c74eee2cb342a8174a9a388f783`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:9b440bee75dd7f1e7f9d0e4cbbb2663e618d3e6a5fdc90d3e88f4af031e10796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867620d601095a8e8567c235e241e214f87f9a2fe7450c18bdfc0082e30cc5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:48:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:48:57 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:48:57 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:48:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:48:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8731f6ea8e41da978c9015e88d36b5917a2f6397f9132069cfbc125d7155d3`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8001b7ff14d8d35bc729550ecb3b02f0c53ecadc34c6b03a3535b339fa312`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 2.2 MB (2183972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cf1d352b21ae47c02a9b4657d918ab1054454f186ff9aab730d6cbaecf2ef5`  
		Last Modified: Wed, 14 Jun 2023 16:49:11 GMT  
		Size: 5.1 MB (5134893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccded95a3299daeabfb9850fa9b6a32204aa92961dd6288e83aa254778214432`  
		Last Modified: Wed, 14 Jun 2023 16:49:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55e9caf413a408e12751cc865cc4e045a402f26c8d93524d831fdb0c0518f7b`  
		Last Modified: Wed, 14 Jun 2023 16:49:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:30b5cbc3896fccc9352c469fcefd3f0c394afe7188f476730ef8a47d95ce0ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31723067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb60681760d439d2994426f6abeee60d90b4b4b63fde1c2000b715e2f3344b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:24 GMT
ADD file:e0cfa2ad9282d0f4647498eb8121e93a14380cf8da98ea55054b555c1533bfff in / 
# Mon, 12 Jun 2023 23:58:24 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:32:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:32:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:33:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:33:01 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:33:01 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:53c17f790ffc929ad5caba471fff88bccc04ac924bce8725b7a0349e2ca1acde`  
		Last Modified: Tue, 13 Jun 2023 00:03:45 GMT  
		Size: 24.8 MB (24801257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6ba319270a3bcefa828a485037c6f5f97aad3b53f81e7e6ad9c1383262710`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974039e6afa1c8198b3faaf97d47978b6020ea7ea3f37bbec3b871671e94300`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 2.0 MB (2043272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726afe3ebe0c48219cc3501b2ce061bd07e4bc54ce71cabcb7a3c14a5dff6e1`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 4.9 MB (4876941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702ebc89990308a116eb63ee03c99be16434bad89b65c4ee7622309b4af002b2`  
		Last Modified: Wed, 14 Jun 2023 17:33:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804a58e1a7bdce1bfdf3c45c3e4756e7e7772624b50326aa58f5cfc036212bc3`  
		Last Modified: Wed, 14 Jun 2023 17:33:12 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:556ca8f88ef7cc81403a9a97d0dd87ad757320e01e6f95a2522a1e484cbd8a87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37061466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e9f2acd14674c9a7a1532aa4d74d686a7be75fff598ab6a90b3255c9821c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:38:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 06:38:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:38:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 06:39:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 06:39:29 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 06:39:29 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 06:39:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:39:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f130b8e8cb6a295db062a4bbd961e61a2665697e73c689ac96183c240872c9`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742747b981049267ff027c5437b4368631be7b5a687e9c963ee77d09f7bd78b2`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 2.4 MB (2429788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4eb4de7b3cfe458146fa063dbe2fce0476cb0cfc426c84b4877b2782619fa3`  
		Last Modified: Tue, 04 Jul 2023 06:39:43 GMT  
		Size: 5.5 MB (5477622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c07ebf28daed63c65f5c1c0c32d379413c009c45813f2820a71fdee4c94fc4`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb28d7721e6f6a19bee631d7041934ff8e5db42d32cbeea54c91b8f701f043c`  
		Last Modified: Tue, 04 Jul 2023 06:39:42 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:6d43aa8eebb100dc3902b2eaa5f40157469896c21bd164f77a06f3026a93c0d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38665743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993cd2fb56db3a2adeeb9114bffeae8eebba23542470b19cb60f7cdce843e6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:38:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:39:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:39:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:39:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:39:34 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:39:34 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:39:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:39:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685167f1ee90548b2f936c06be0065bf15d334019d1e813cda5976a5faac51c`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356b3aaf212a1206664cfa580d6494f684712648172e626a5763e533f2c299d`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 2.6 MB (2583523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ce596d3d2605c349675410e1dfb1fca82b059b70aff89bf88ffc1fc97db9d5`  
		Last Modified: Wed, 14 Jun 2023 16:39:46 GMT  
		Size: 5.9 MB (5939881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d386251a97c8b66dba4287f8f25b1c909088233cadccdf0e309f8eaa985ad4a`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eb9777f0312b075ad06ae71992bbb8bcc27c8bf98e792b890b735d9bb363ab`  
		Last Modified: Wed, 14 Jun 2023 16:39:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:50832426d7cb80d309089d746661f34c44035d7e84bd18b7fcb4723ff1997d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36751873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69867d0746d2fd9d2480898e231157b8f393d8f2494a99e7a366a96048090c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:07:47 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 17:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 17:09:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 17:09:45 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 17:09:48 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 17:09:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 17:09:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db93178c77bcf3593248cad8b6debe8211f889bab334155486932dcdda101114`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf95eb82740eff246297f431c228de764d013565cb9ecf1e4dcedb0d520b534`  
		Last Modified: Wed, 14 Jun 2023 17:10:17 GMT  
		Size: 1.8 MB (1831650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1200cbabde345fbda9a6bbc760be93debd257049c125a67b59e79f1c555ae8`  
		Last Modified: Wed, 14 Jun 2023 17:10:20 GMT  
		Size: 5.8 MB (5800581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f3295ef8123cce31a6f517bef21b5685b9fea7f14b9869d286d0a18a359f33`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92a5c67d2822f5a3bb9b16dfa8366ab2138da333657bc937313ab8bda4e687f`  
		Last Modified: Wed, 14 Jun 2023 17:10:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:f442dd454e56427ca33cb68a25d0a2ce387abcb81ca2070b5366e3f18d67c71e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42302809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4d6c06c55a4f1d2d84745e1910b74b5b60ccd5d5ac8b65cbe89c9d741ade45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 16:16:53 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 14 Jun 2023 16:17:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 16:17:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 14 Jun 2023 16:17:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 14 Jun 2023 16:17:49 GMT
VOLUME [/spiped]
# Wed, 14 Jun 2023 16:17:49 GMT
WORKDIR /spiped
# Wed, 14 Jun 2023 16:17:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Jun 2023 16:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 16:17:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ba44a5f009fb88ac04074f22f429b6a2b2af33d421b72db5cca0d672c71c2`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f9739d0b82c3102ad8e4d8d7077bca691e114e60870be5667589758e19dce9`  
		Last Modified: Wed, 14 Jun 2023 16:18:14 GMT  
		Size: 2.8 MB (2764939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002910d3fc58c5a9633efc7916165b4d36ce0111cd382c9a8961532731eb3c4b`  
		Last Modified: Wed, 14 Jun 2023 16:18:15 GMT  
		Size: 6.4 MB (6419551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ce6d2ff5db3cde73486e9687d83ec5c5018b427354a99801e5cc76f85d7c99`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceae632d9532021a35833afdf67e328b295eec28535fdc00f40db00d7f1b4be`  
		Last Modified: Wed, 14 Jun 2023 16:18:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:7da21e08b694c65fccd8bd9db69ad2f20813743d119ee28dc199d12fb9dc3028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35129685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e8f381b5476bc8e56f26338b037055a33cc30082f7f78dcfb3ed05fe124662`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 17:32:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 15 Jun 2023 17:32:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 15 Jun 2023 17:32:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 17:33:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 15 Jun 2023 17:33:06 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 17:33:06 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 17:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 17:33:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 17:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56005098175a3f774a51986990ea797e5c84e146dbba376788635dfff9883d0d`  
		Last Modified: Thu, 15 Jun 2023 17:39:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e66f9f2f9f8e8b78cd7100f536392d10d1f3e77b071f0f34672c9b46413d22`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 2.3 MB (2257953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb80d8c82f6c1399d6b56aed13f0a3b145fb5d3d4bed63fe7fe0c86051890b9`  
		Last Modified: Thu, 15 Jun 2023 17:39:22 GMT  
		Size: 5.4 MB (5382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cb16cc5602b4e3f0fed2448ba36f83a4d8a7722477985c0952f5e7fa485c56`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71f6513b8c3f865bc1564ec946f9af84c82a10111dc2a5a1401b289fe455dc`  
		Last Modified: Thu, 15 Jun 2023 17:39:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
