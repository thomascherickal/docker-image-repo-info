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
$ docker pull spiped@sha256:60792d5ef43f552360d6b77b9576a01228bebdbc2af4928bb707a3ee2549733c
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
$ docker pull spiped@sha256:485847df99592ce46f57b80602930020570589bc92a57bcf52c0f12576823a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33949464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edd13d49980a223e5a1a05715139ed281b0a6eb541dade9ed3f270ad4cd0bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 13:50:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 13:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 13:51:10 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 13:51:10 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 13:51:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:51:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647fed87ad0da4e5831b9907161c1b43ec672b65a95198be6094e7480d581bad`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788b6b58021116fa18c299ebb7fd9914e26e5b7845b44641398fe8122b749519`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f22319e31ec1e1bba11547c2d32e6210b87ed0647fdf4dd64143be50dc2a30`  
		Last Modified: Wed, 05 Oct 2022 13:51:31 GMT  
		Size: 5.0 MB (5027834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79612caf3d4ffa418788cd8c7a273b28bfcb96d8c83830d22736b42d59752f99`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3e9d639a80e9684a0fd3b86d20666922b4d42f0448143b7065898439f5d98`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:be1ad2cbf3c4749f4f3ad1901e49f28ce59e393f77a5e8bbdc1934e9dc7f06b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31330089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615d8374859d2dc36d580e1ebc964ba4372deb8348516c86ea093fc7de8fe4bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:27:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:27:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:27:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:27:40 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:27:41 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:27:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df40850a697b1085bcb37facda4649675c11747ceda87157bf7c9c485c5ce49`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a82a9536a373fdbbbf4da2ce7b24365418abbd6ec023ca2e087e071f7168eb3`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1716079ee90134175f14061acb4ed8f20fdd29fcc172fe6084aacd233b75d20`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 4.7 MB (4747637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db88c4deabc13e23b2452cc73b4731feb1b5fadd585289195eb377197614f6`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96859a7277435ad4739e871037f955a296c0e4840e0c8388887ebe08a09da32d`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:47adb086ffbc8238cc87a374d5545eb53d0e867848ace36033c5d207ed2868c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f97b2795173eb5045fd9730321b818e919dc60c5ecb739c65b4660fcbe02e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:23:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:23:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:23:29 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:23:30 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:23:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:23:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301477fc358e3377ddd636b2616c84fcf5124bd247b627567141c87be9f6de1`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302fdee302af51fa37c04770a7b242e609fcccfd0cfd6ff1f84255fd78fddc2`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae3b94946b96722b37618a3af96e0d185b745edae682b8ce313a98448c0c78`  
		Last Modified: Wed, 05 Oct 2022 14:24:02 GMT  
		Size: 5.3 MB (5270141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56107eb63a27bf608f2ed332d5a8af7040e6d0a2ea0d71bc4889978c765af4`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdd8dce6303958fb1fd5e08767c354bfb5f383d72f0a746b331d1994526d8dc`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:28d8bdf2af4f3d895db835d3a8746fd5a569f41f63fb1ecfa5f1f7cfd8c8daa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40288236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c91f70f71153acda4d046f399b07518ac65cd5150c34e1701fc88987574e1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:09:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:09:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:09:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:09:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:09:45 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:09:46 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:09:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:09:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:09:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d3a5b3eec462b1c6ac59cb81a82a136592cec8dd1e4b01a7ff18f94fb6732`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d16e767b1ff67a46f1f079896d403560a4418176d4f3e8edd740703875ee2bd`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089c61d4bb583ef72de3d4af7e734b4b2c6db1c19ce43112038140b60539d3f`  
		Last Modified: Wed, 05 Oct 2022 14:10:19 GMT  
		Size: 7.9 MB (7888980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d79866b3db5ee7887f80f5f15edc439162fc445b37ebee95562f558be876c30`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ce86fb3faa98b26c3f4b6ca4fe16aba6bb731583f47837c5e19b3624ee014`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:123ccf6bf7870f663a836d6b42768cb49fc6a2a67fe65eab98898130fbacb91a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35348950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5779a3f203e4c018cb40a9c1887dbd52b5852288eebd13cc7d46a2f593510175`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:02:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:02:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:03:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:04:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:04:30 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:04:33 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:04:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:04:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:04:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fef092d9f7ba63a39ca1cdb3fe82522c963b4831657b64e7d9a20fb87c0d549`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74beea1ecce269e87b3fa3a679d9c1426eb65ee3a9ca732085c10b4bbfdb95`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1d5db219d406d5845647ae1c960c206474eead0677d57a375a5ddd4cfb2312`  
		Last Modified: Thu, 06 Oct 2022 05:05:04 GMT  
		Size: 5.7 MB (5705121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d137b8d414adcef161b5b3df846629e84076f81350be9239b039a150906325`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a5107ab173d0c81c031796885923796c56aa6822395457a89160d0b4b62f1`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
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
$ docker pull spiped@sha256:630610f34fd40312ea2ebbab4d205c98d11f71ce40d3d2c89e43d7caa99569ff
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
$ docker pull spiped@sha256:83b7108c070944539ec82ed9729e69afa1a5ad91eed9163efc95bcd8a3455efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8704d25dde580015332a57e745db366aa241d3d99f8949b2c12e3f7c9ae8606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:17:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 04:17:55 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 04:17:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 04:18:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 04:18:06 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 04:18:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 04:18:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 04:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:18:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163365ead583145f60498102a9de8f3de170409f2ae8cecf962cf3ab512bb7b6`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ebb86b08f67f6638bc3391b020d7e3c07ac692076e469c99ba197a3dc6180d`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0d696472090a4ef1527e0ceea219db2e5ca85866d16132e7f6a560e73c84d3`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 221.2 KB (221183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad76fb7ed47c485b828ec98e173c844febdb11324b807d8befb613a1c8f4e06`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598391454db346484a0ec6968962627ae778f5ab04cf800247c9dd1ce7ab6878`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:e5b68da77cb9db28f4d5f80f8220af5803599cf23e9cce57f4b25405f32853f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681bb24795641aec826f9fcf710d73e0f839c1d83231b15da58521db752ad663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:37:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:37:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:37:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:54 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:55 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7901c95a1447d090815ba8f9d5afa5abbdd9cdd431c948e1cac143e5cdacea73`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081551fa64d93cc14b0e29df21933895b17862a013e29ac667046d4ea8db0b14`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94947ded225af3a68fa2d3e89d286cd5424a073fd1597c34b8fd81fd125c0684`  
		Last Modified: Fri, 07 Oct 2022 07:38:26 GMT  
		Size: 214.3 KB (214266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443d577082fa11b6c6c4af1a7cf3bcc77598280a04be75044d38d529083f988`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141acab92005d5c00bc4f4d6679742fb826be835ac933c9bc5495eb8256eb7e6`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6423a7f534f20d885a95067600857ce072688766c2ffa6bb9010fc6d7f7231ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7719409551ce46332256dc9374bbbe5ebad7eebb18d4f5c3e768b35cabfc11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:06:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 02:06:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 02:06:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 02:06:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 02:06:41 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 02:06:42 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 02:06:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:06:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:06:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fdd64c4ca701476bab0ba1a71f21a0405e2b79db064444f6f738b3bdb2683`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c854898389b43dbb9cdd413e814a0799ae7a3efd037dc62a2ab580f223d09dd9`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8e6b40665d81d34cbfaf2714f35b8921a3441a7458b416a69479dda6fded73`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 231.3 KB (231328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75809d30c75c96ac8571a0aad6037398080e8464c1fe900186204d14ed97ee5`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7f4311d12b79d5b5ed076ae0276fdc41d636eb2425cce1969ffbbecfaa48f`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:23f7c4e2894e2b69ec8f99ad3e5bfc9eb384bfb0867a580c0a14296e9fda6808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea36cd4aae1294ce2738686854cda02fd8af9cb087470d67f42ae503ef53dbe2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:36:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:36:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:05 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6730e71fd53d14fc64b230b13be77ded2ae164bb8e0b21103c39d2320db3c383`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a98530f24008a28aeac69a847b3e388d2db70cb4ec34485f3b180da38729d98`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 7.7 KB (7744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c3cac559b59708bf223d2fd843ed2dfd7083c5bb42e2bdc5459c77bb508bf`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 220.3 KB (220251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8832c249dd749cdd6d7eea870aa3a8ee137af08153d1b9a6cd50600958066aa`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4f5e799656197f8bfd5fad27d5caf0993b2a631ac187a703a21cf24dcc448`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
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
$ docker pull spiped@sha256:60792d5ef43f552360d6b77b9576a01228bebdbc2af4928bb707a3ee2549733c
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
$ docker pull spiped@sha256:485847df99592ce46f57b80602930020570589bc92a57bcf52c0f12576823a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33949464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edd13d49980a223e5a1a05715139ed281b0a6eb541dade9ed3f270ad4cd0bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 13:50:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 13:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 13:51:10 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 13:51:10 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 13:51:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:51:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647fed87ad0da4e5831b9907161c1b43ec672b65a95198be6094e7480d581bad`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788b6b58021116fa18c299ebb7fd9914e26e5b7845b44641398fe8122b749519`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f22319e31ec1e1bba11547c2d32e6210b87ed0647fdf4dd64143be50dc2a30`  
		Last Modified: Wed, 05 Oct 2022 13:51:31 GMT  
		Size: 5.0 MB (5027834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79612caf3d4ffa418788cd8c7a273b28bfcb96d8c83830d22736b42d59752f99`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3e9d639a80e9684a0fd3b86d20666922b4d42f0448143b7065898439f5d98`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:be1ad2cbf3c4749f4f3ad1901e49f28ce59e393f77a5e8bbdc1934e9dc7f06b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31330089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615d8374859d2dc36d580e1ebc964ba4372deb8348516c86ea093fc7de8fe4bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:27:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:27:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:27:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:27:40 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:27:41 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:27:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df40850a697b1085bcb37facda4649675c11747ceda87157bf7c9c485c5ce49`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a82a9536a373fdbbbf4da2ce7b24365418abbd6ec023ca2e087e071f7168eb3`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1716079ee90134175f14061acb4ed8f20fdd29fcc172fe6084aacd233b75d20`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 4.7 MB (4747637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db88c4deabc13e23b2452cc73b4731feb1b5fadd585289195eb377197614f6`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96859a7277435ad4739e871037f955a296c0e4840e0c8388887ebe08a09da32d`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:47adb086ffbc8238cc87a374d5545eb53d0e867848ace36033c5d207ed2868c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f97b2795173eb5045fd9730321b818e919dc60c5ecb739c65b4660fcbe02e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:23:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:23:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:23:29 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:23:30 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:23:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:23:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301477fc358e3377ddd636b2616c84fcf5124bd247b627567141c87be9f6de1`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302fdee302af51fa37c04770a7b242e609fcccfd0cfd6ff1f84255fd78fddc2`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae3b94946b96722b37618a3af96e0d185b745edae682b8ce313a98448c0c78`  
		Last Modified: Wed, 05 Oct 2022 14:24:02 GMT  
		Size: 5.3 MB (5270141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56107eb63a27bf608f2ed332d5a8af7040e6d0a2ea0d71bc4889978c765af4`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdd8dce6303958fb1fd5e08767c354bfb5f383d72f0a746b331d1994526d8dc`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:28d8bdf2af4f3d895db835d3a8746fd5a569f41f63fb1ecfa5f1f7cfd8c8daa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40288236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c91f70f71153acda4d046f399b07518ac65cd5150c34e1701fc88987574e1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:09:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:09:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:09:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:09:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:09:45 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:09:46 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:09:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:09:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:09:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d3a5b3eec462b1c6ac59cb81a82a136592cec8dd1e4b01a7ff18f94fb6732`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d16e767b1ff67a46f1f079896d403560a4418176d4f3e8edd740703875ee2bd`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089c61d4bb583ef72de3d4af7e734b4b2c6db1c19ce43112038140b60539d3f`  
		Last Modified: Wed, 05 Oct 2022 14:10:19 GMT  
		Size: 7.9 MB (7888980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d79866b3db5ee7887f80f5f15edc439162fc445b37ebee95562f558be876c30`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ce86fb3faa98b26c3f4b6ca4fe16aba6bb731583f47837c5e19b3624ee014`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:123ccf6bf7870f663a836d6b42768cb49fc6a2a67fe65eab98898130fbacb91a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35348950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5779a3f203e4c018cb40a9c1887dbd52b5852288eebd13cc7d46a2f593510175`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:02:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:02:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:03:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:04:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:04:30 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:04:33 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:04:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:04:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:04:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fef092d9f7ba63a39ca1cdb3fe82522c963b4831657b64e7d9a20fb87c0d549`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74beea1ecce269e87b3fa3a679d9c1426eb65ee3a9ca732085c10b4bbfdb95`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1d5db219d406d5845647ae1c960c206474eead0677d57a375a5ddd4cfb2312`  
		Last Modified: Thu, 06 Oct 2022 05:05:04 GMT  
		Size: 5.7 MB (5705121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d137b8d414adcef161b5b3df846629e84076f81350be9239b039a150906325`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a5107ab173d0c81c031796885923796c56aa6822395457a89160d0b4b62f1`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
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
$ docker pull spiped@sha256:630610f34fd40312ea2ebbab4d205c98d11f71ce40d3d2c89e43d7caa99569ff
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
$ docker pull spiped@sha256:83b7108c070944539ec82ed9729e69afa1a5ad91eed9163efc95bcd8a3455efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8704d25dde580015332a57e745db366aa241d3d99f8949b2c12e3f7c9ae8606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:17:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 04:17:55 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 04:17:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 04:18:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 04:18:06 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 04:18:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 04:18:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 04:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:18:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163365ead583145f60498102a9de8f3de170409f2ae8cecf962cf3ab512bb7b6`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ebb86b08f67f6638bc3391b020d7e3c07ac692076e469c99ba197a3dc6180d`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0d696472090a4ef1527e0ceea219db2e5ca85866d16132e7f6a560e73c84d3`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 221.2 KB (221183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad76fb7ed47c485b828ec98e173c844febdb11324b807d8befb613a1c8f4e06`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598391454db346484a0ec6968962627ae778f5ab04cf800247c9dd1ce7ab6878`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:e5b68da77cb9db28f4d5f80f8220af5803599cf23e9cce57f4b25405f32853f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681bb24795641aec826f9fcf710d73e0f839c1d83231b15da58521db752ad663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:37:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:37:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:37:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:54 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:55 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7901c95a1447d090815ba8f9d5afa5abbdd9cdd431c948e1cac143e5cdacea73`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081551fa64d93cc14b0e29df21933895b17862a013e29ac667046d4ea8db0b14`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94947ded225af3a68fa2d3e89d286cd5424a073fd1597c34b8fd81fd125c0684`  
		Last Modified: Fri, 07 Oct 2022 07:38:26 GMT  
		Size: 214.3 KB (214266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443d577082fa11b6c6c4af1a7cf3bcc77598280a04be75044d38d529083f988`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141acab92005d5c00bc4f4d6679742fb826be835ac933c9bc5495eb8256eb7e6`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6423a7f534f20d885a95067600857ce072688766c2ffa6bb9010fc6d7f7231ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7719409551ce46332256dc9374bbbe5ebad7eebb18d4f5c3e768b35cabfc11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:06:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 02:06:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 02:06:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 02:06:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 02:06:41 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 02:06:42 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 02:06:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:06:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:06:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fdd64c4ca701476bab0ba1a71f21a0405e2b79db064444f6f738b3bdb2683`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c854898389b43dbb9cdd413e814a0799ae7a3efd037dc62a2ab580f223d09dd9`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8e6b40665d81d34cbfaf2714f35b8921a3441a7458b416a69479dda6fded73`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 231.3 KB (231328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75809d30c75c96ac8571a0aad6037398080e8464c1fe900186204d14ed97ee5`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7f4311d12b79d5b5ed076ae0276fdc41d636eb2425cce1969ffbbecfaa48f`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:23f7c4e2894e2b69ec8f99ad3e5bfc9eb384bfb0867a580c0a14296e9fda6808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea36cd4aae1294ce2738686854cda02fd8af9cb087470d67f42ae503ef53dbe2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:36:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:36:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:05 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6730e71fd53d14fc64b230b13be77ded2ae164bb8e0b21103c39d2320db3c383`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a98530f24008a28aeac69a847b3e388d2db70cb4ec34485f3b180da38729d98`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 7.7 KB (7744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c3cac559b59708bf223d2fd843ed2dfd7083c5bb42e2bdc5459c77bb508bf`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 220.3 KB (220251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8832c249dd749cdd6d7eea870aa3a8ee137af08153d1b9a6cd50600958066aa`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4f5e799656197f8bfd5fad27d5caf0993b2a631ac187a703a21cf24dcc448`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
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
$ docker pull spiped@sha256:60792d5ef43f552360d6b77b9576a01228bebdbc2af4928bb707a3ee2549733c
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
$ docker pull spiped@sha256:485847df99592ce46f57b80602930020570589bc92a57bcf52c0f12576823a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33949464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edd13d49980a223e5a1a05715139ed281b0a6eb541dade9ed3f270ad4cd0bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 13:50:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 13:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 13:51:10 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 13:51:10 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 13:51:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:51:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647fed87ad0da4e5831b9907161c1b43ec672b65a95198be6094e7480d581bad`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788b6b58021116fa18c299ebb7fd9914e26e5b7845b44641398fe8122b749519`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f22319e31ec1e1bba11547c2d32e6210b87ed0647fdf4dd64143be50dc2a30`  
		Last Modified: Wed, 05 Oct 2022 13:51:31 GMT  
		Size: 5.0 MB (5027834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79612caf3d4ffa418788cd8c7a273b28bfcb96d8c83830d22736b42d59752f99`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3e9d639a80e9684a0fd3b86d20666922b4d42f0448143b7065898439f5d98`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:be1ad2cbf3c4749f4f3ad1901e49f28ce59e393f77a5e8bbdc1934e9dc7f06b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31330089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615d8374859d2dc36d580e1ebc964ba4372deb8348516c86ea093fc7de8fe4bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:27:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:27:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:27:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:27:40 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:27:41 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:27:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df40850a697b1085bcb37facda4649675c11747ceda87157bf7c9c485c5ce49`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a82a9536a373fdbbbf4da2ce7b24365418abbd6ec023ca2e087e071f7168eb3`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1716079ee90134175f14061acb4ed8f20fdd29fcc172fe6084aacd233b75d20`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 4.7 MB (4747637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db88c4deabc13e23b2452cc73b4731feb1b5fadd585289195eb377197614f6`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96859a7277435ad4739e871037f955a296c0e4840e0c8388887ebe08a09da32d`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:47adb086ffbc8238cc87a374d5545eb53d0e867848ace36033c5d207ed2868c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f97b2795173eb5045fd9730321b818e919dc60c5ecb739c65b4660fcbe02e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:23:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:23:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:23:29 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:23:30 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:23:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:23:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301477fc358e3377ddd636b2616c84fcf5124bd247b627567141c87be9f6de1`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302fdee302af51fa37c04770a7b242e609fcccfd0cfd6ff1f84255fd78fddc2`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae3b94946b96722b37618a3af96e0d185b745edae682b8ce313a98448c0c78`  
		Last Modified: Wed, 05 Oct 2022 14:24:02 GMT  
		Size: 5.3 MB (5270141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56107eb63a27bf608f2ed332d5a8af7040e6d0a2ea0d71bc4889978c765af4`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdd8dce6303958fb1fd5e08767c354bfb5f383d72f0a746b331d1994526d8dc`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:28d8bdf2af4f3d895db835d3a8746fd5a569f41f63fb1ecfa5f1f7cfd8c8daa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40288236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c91f70f71153acda4d046f399b07518ac65cd5150c34e1701fc88987574e1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:09:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:09:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:09:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:09:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:09:45 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:09:46 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:09:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:09:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:09:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d3a5b3eec462b1c6ac59cb81a82a136592cec8dd1e4b01a7ff18f94fb6732`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d16e767b1ff67a46f1f079896d403560a4418176d4f3e8edd740703875ee2bd`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089c61d4bb583ef72de3d4af7e734b4b2c6db1c19ce43112038140b60539d3f`  
		Last Modified: Wed, 05 Oct 2022 14:10:19 GMT  
		Size: 7.9 MB (7888980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d79866b3db5ee7887f80f5f15edc439162fc445b37ebee95562f558be876c30`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ce86fb3faa98b26c3f4b6ca4fe16aba6bb731583f47837c5e19b3624ee014`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:123ccf6bf7870f663a836d6b42768cb49fc6a2a67fe65eab98898130fbacb91a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35348950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5779a3f203e4c018cb40a9c1887dbd52b5852288eebd13cc7d46a2f593510175`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:02:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:02:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:03:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:04:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:04:30 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:04:33 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:04:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:04:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:04:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fef092d9f7ba63a39ca1cdb3fe82522c963b4831657b64e7d9a20fb87c0d549`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74beea1ecce269e87b3fa3a679d9c1426eb65ee3a9ca732085c10b4bbfdb95`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1d5db219d406d5845647ae1c960c206474eead0677d57a375a5ddd4cfb2312`  
		Last Modified: Thu, 06 Oct 2022 05:05:04 GMT  
		Size: 5.7 MB (5705121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d137b8d414adcef161b5b3df846629e84076f81350be9239b039a150906325`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a5107ab173d0c81c031796885923796c56aa6822395457a89160d0b4b62f1`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
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
$ docker pull spiped@sha256:630610f34fd40312ea2ebbab4d205c98d11f71ce40d3d2c89e43d7caa99569ff
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
$ docker pull spiped@sha256:83b7108c070944539ec82ed9729e69afa1a5ad91eed9163efc95bcd8a3455efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8704d25dde580015332a57e745db366aa241d3d99f8949b2c12e3f7c9ae8606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:17:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 04:17:55 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 04:17:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 04:18:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 04:18:06 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 04:18:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 04:18:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 04:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:18:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163365ead583145f60498102a9de8f3de170409f2ae8cecf962cf3ab512bb7b6`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ebb86b08f67f6638bc3391b020d7e3c07ac692076e469c99ba197a3dc6180d`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0d696472090a4ef1527e0ceea219db2e5ca85866d16132e7f6a560e73c84d3`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 221.2 KB (221183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad76fb7ed47c485b828ec98e173c844febdb11324b807d8befb613a1c8f4e06`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598391454db346484a0ec6968962627ae778f5ab04cf800247c9dd1ce7ab6878`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:e5b68da77cb9db28f4d5f80f8220af5803599cf23e9cce57f4b25405f32853f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681bb24795641aec826f9fcf710d73e0f839c1d83231b15da58521db752ad663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:37:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:37:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:37:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:54 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:55 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7901c95a1447d090815ba8f9d5afa5abbdd9cdd431c948e1cac143e5cdacea73`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081551fa64d93cc14b0e29df21933895b17862a013e29ac667046d4ea8db0b14`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94947ded225af3a68fa2d3e89d286cd5424a073fd1597c34b8fd81fd125c0684`  
		Last Modified: Fri, 07 Oct 2022 07:38:26 GMT  
		Size: 214.3 KB (214266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443d577082fa11b6c6c4af1a7cf3bcc77598280a04be75044d38d529083f988`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141acab92005d5c00bc4f4d6679742fb826be835ac933c9bc5495eb8256eb7e6`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6423a7f534f20d885a95067600857ce072688766c2ffa6bb9010fc6d7f7231ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7719409551ce46332256dc9374bbbe5ebad7eebb18d4f5c3e768b35cabfc11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:06:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 02:06:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 02:06:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 02:06:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 02:06:41 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 02:06:42 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 02:06:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:06:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:06:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fdd64c4ca701476bab0ba1a71f21a0405e2b79db064444f6f738b3bdb2683`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c854898389b43dbb9cdd413e814a0799ae7a3efd037dc62a2ab580f223d09dd9`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8e6b40665d81d34cbfaf2714f35b8921a3441a7458b416a69479dda6fded73`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 231.3 KB (231328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75809d30c75c96ac8571a0aad6037398080e8464c1fe900186204d14ed97ee5`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7f4311d12b79d5b5ed076ae0276fdc41d636eb2425cce1969ffbbecfaa48f`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:23f7c4e2894e2b69ec8f99ad3e5bfc9eb384bfb0867a580c0a14296e9fda6808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea36cd4aae1294ce2738686854cda02fd8af9cb087470d67f42ae503ef53dbe2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:36:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:36:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:05 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6730e71fd53d14fc64b230b13be77ded2ae164bb8e0b21103c39d2320db3c383`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a98530f24008a28aeac69a847b3e388d2db70cb4ec34485f3b180da38729d98`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 7.7 KB (7744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c3cac559b59708bf223d2fd843ed2dfd7083c5bb42e2bdc5459c77bb508bf`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 220.3 KB (220251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8832c249dd749cdd6d7eea870aa3a8ee137af08153d1b9a6cd50600958066aa`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4f5e799656197f8bfd5fad27d5caf0993b2a631ac187a703a21cf24dcc448`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
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
$ docker pull spiped@sha256:630610f34fd40312ea2ebbab4d205c98d11f71ce40d3d2c89e43d7caa99569ff
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
$ docker pull spiped@sha256:83b7108c070944539ec82ed9729e69afa1a5ad91eed9163efc95bcd8a3455efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8704d25dde580015332a57e745db366aa241d3d99f8949b2c12e3f7c9ae8606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:17:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 04:17:55 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 04:17:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 04:18:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 04:18:06 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 04:18:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 04:18:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 04:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:18:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163365ead583145f60498102a9de8f3de170409f2ae8cecf962cf3ab512bb7b6`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ebb86b08f67f6638bc3391b020d7e3c07ac692076e469c99ba197a3dc6180d`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0d696472090a4ef1527e0ceea219db2e5ca85866d16132e7f6a560e73c84d3`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 221.2 KB (221183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad76fb7ed47c485b828ec98e173c844febdb11324b807d8befb613a1c8f4e06`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598391454db346484a0ec6968962627ae778f5ab04cf800247c9dd1ce7ab6878`  
		Last Modified: Fri, 07 Oct 2022 04:18:24 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:e5b68da77cb9db28f4d5f80f8220af5803599cf23e9cce57f4b25405f32853f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681bb24795641aec826f9fcf710d73e0f839c1d83231b15da58521db752ad663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:37:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:37:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:37:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:54 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:55 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7901c95a1447d090815ba8f9d5afa5abbdd9cdd431c948e1cac143e5cdacea73`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081551fa64d93cc14b0e29df21933895b17862a013e29ac667046d4ea8db0b14`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94947ded225af3a68fa2d3e89d286cd5424a073fd1597c34b8fd81fd125c0684`  
		Last Modified: Fri, 07 Oct 2022 07:38:26 GMT  
		Size: 214.3 KB (214266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443d577082fa11b6c6c4af1a7cf3bcc77598280a04be75044d38d529083f988`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141acab92005d5c00bc4f4d6679742fb826be835ac933c9bc5495eb8256eb7e6`  
		Last Modified: Fri, 07 Oct 2022 07:38:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:6423a7f534f20d885a95067600857ce072688766c2ffa6bb9010fc6d7f7231ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7719409551ce46332256dc9374bbbe5ebad7eebb18d4f5c3e768b35cabfc11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:06:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 02:06:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 02:06:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 02:06:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 02:06:41 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 02:06:42 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 02:06:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:06:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:06:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fdd64c4ca701476bab0ba1a71f21a0405e2b79db064444f6f738b3bdb2683`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c854898389b43dbb9cdd413e814a0799ae7a3efd037dc62a2ab580f223d09dd9`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 7.7 KB (7713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8e6b40665d81d34cbfaf2714f35b8921a3441a7458b416a69479dda6fded73`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 231.3 KB (231328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75809d30c75c96ac8571a0aad6037398080e8464c1fe900186204d14ed97ee5`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7f4311d12b79d5b5ed076ae0276fdc41d636eb2425cce1969ffbbecfaa48f`  
		Last Modified: Fri, 07 Oct 2022 02:07:15 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:23f7c4e2894e2b69ec8f99ad3e5bfc9eb384bfb0867a580c0a14296e9fda6808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea36cd4aae1294ce2738686854cda02fd8af9cb087470d67f42ae503ef53dbe2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:36:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 07 Oct 2022 07:36:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 07 Oct 2022 07:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 07 Oct 2022 07:37:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:37:05 GMT
VOLUME [/spiped]
# Fri, 07 Oct 2022 07:37:06 GMT
WORKDIR /spiped
# Fri, 07 Oct 2022 07:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 07 Oct 2022 07:37:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 07:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6730e71fd53d14fc64b230b13be77ded2ae164bb8e0b21103c39d2320db3c383`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a98530f24008a28aeac69a847b3e388d2db70cb4ec34485f3b180da38729d98`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 7.7 KB (7744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c3cac559b59708bf223d2fd843ed2dfd7083c5bb42e2bdc5459c77bb508bf`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 220.3 KB (220251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8832c249dd749cdd6d7eea870aa3a8ee137af08153d1b9a6cd50600958066aa`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4f5e799656197f8bfd5fad27d5caf0993b2a631ac187a703a21cf24dcc448`  
		Last Modified: Fri, 07 Oct 2022 07:37:35 GMT  
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
$ docker pull spiped@sha256:60792d5ef43f552360d6b77b9576a01228bebdbc2af4928bb707a3ee2549733c
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
$ docker pull spiped@sha256:485847df99592ce46f57b80602930020570589bc92a57bcf52c0f12576823a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33949464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edd13d49980a223e5a1a05715139ed281b0a6eb541dade9ed3f270ad4cd0bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 13:50:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:50:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 13:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 13:51:10 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 13:51:10 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 13:51:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:51:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647fed87ad0da4e5831b9907161c1b43ec672b65a95198be6094e7480d581bad`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788b6b58021116fa18c299ebb7fd9914e26e5b7845b44641398fe8122b749519`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f22319e31ec1e1bba11547c2d32e6210b87ed0647fdf4dd64143be50dc2a30`  
		Last Modified: Wed, 05 Oct 2022 13:51:31 GMT  
		Size: 5.0 MB (5027834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79612caf3d4ffa418788cd8c7a273b28bfcb96d8c83830d22736b42d59752f99`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3e9d639a80e9684a0fd3b86d20666922b4d42f0448143b7065898439f5d98`  
		Last Modified: Wed, 05 Oct 2022 13:51:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:be1ad2cbf3c4749f4f3ad1901e49f28ce59e393f77a5e8bbdc1934e9dc7f06b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31330089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615d8374859d2dc36d580e1ebc964ba4372deb8348516c86ea093fc7de8fe4bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:27:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:27:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:27:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:27:40 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:27:41 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:27:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:27:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df40850a697b1085bcb37facda4649675c11747ceda87157bf7c9c485c5ce49`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a82a9536a373fdbbbf4da2ce7b24365418abbd6ec023ca2e087e071f7168eb3`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1716079ee90134175f14061acb4ed8f20fdd29fcc172fe6084aacd233b75d20`  
		Last Modified: Thu, 06 Oct 2022 05:28:14 GMT  
		Size: 4.7 MB (4747637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db88c4deabc13e23b2452cc73b4731feb1b5fadd585289195eb377197614f6`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96859a7277435ad4739e871037f955a296c0e4840e0c8388887ebe08a09da32d`  
		Last Modified: Thu, 06 Oct 2022 05:28:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:47adb086ffbc8238cc87a374d5545eb53d0e867848ace36033c5d207ed2868c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f97b2795173eb5045fd9730321b818e919dc60c5ecb739c65b4660fcbe02e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:23:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:23:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:23:29 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:23:30 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:23:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:23:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301477fc358e3377ddd636b2616c84fcf5124bd247b627567141c87be9f6de1`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302fdee302af51fa37c04770a7b242e609fcccfd0cfd6ff1f84255fd78fddc2`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae3b94946b96722b37618a3af96e0d185b745edae682b8ce313a98448c0c78`  
		Last Modified: Wed, 05 Oct 2022 14:24:02 GMT  
		Size: 5.3 MB (5270141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56107eb63a27bf608f2ed332d5a8af7040e6d0a2ea0d71bc4889978c765af4`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdd8dce6303958fb1fd5e08767c354bfb5f383d72f0a746b331d1994526d8dc`  
		Last Modified: Wed, 05 Oct 2022 14:24:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:28d8bdf2af4f3d895db835d3a8746fd5a569f41f63fb1ecfa5f1f7cfd8c8daa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40288236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c91f70f71153acda4d046f399b07518ac65cd5150c34e1701fc88987574e1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:09:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Oct 2022 14:09:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:09:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Oct 2022 14:09:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 14:09:45 GMT
VOLUME [/spiped]
# Wed, 05 Oct 2022 14:09:46 GMT
WORKDIR /spiped
# Wed, 05 Oct 2022 14:09:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Oct 2022 14:09:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 14:09:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d3a5b3eec462b1c6ac59cb81a82a136592cec8dd1e4b01a7ff18f94fb6732`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d16e767b1ff67a46f1f079896d403560a4418176d4f3e8edd740703875ee2bd`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089c61d4bb583ef72de3d4af7e734b4b2c6db1c19ce43112038140b60539d3f`  
		Last Modified: Wed, 05 Oct 2022 14:10:19 GMT  
		Size: 7.9 MB (7888980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d79866b3db5ee7887f80f5f15edc439162fc445b37ebee95562f558be876c30`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ce86fb3faa98b26c3f4b6ca4fe16aba6bb731583f47837c5e19b3624ee014`  
		Last Modified: Wed, 05 Oct 2022 14:10:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:123ccf6bf7870f663a836d6b42768cb49fc6a2a67fe65eab98898130fbacb91a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35348950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5779a3f203e4c018cb40a9c1887dbd52b5852288eebd13cc7d46a2f593510175`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 05:02:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 06 Oct 2022 05:02:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:03:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 06 Oct 2022 05:04:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 06 Oct 2022 05:04:30 GMT
VOLUME [/spiped]
# Thu, 06 Oct 2022 05:04:33 GMT
WORKDIR /spiped
# Thu, 06 Oct 2022 05:04:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 06 Oct 2022 05:04:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 05:04:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fef092d9f7ba63a39ca1cdb3fe82522c963b4831657b64e7d9a20fb87c0d549`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74beea1ecce269e87b3fa3a679d9c1426eb65ee3a9ca732085c10b4bbfdb95`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1d5db219d406d5845647ae1c960c206474eead0677d57a375a5ddd4cfb2312`  
		Last Modified: Thu, 06 Oct 2022 05:05:04 GMT  
		Size: 5.7 MB (5705121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d137b8d414adcef161b5b3df846629e84076f81350be9239b039a150906325`  
		Last Modified: Thu, 06 Oct 2022 05:04:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a5107ab173d0c81c031796885923796c56aa6822395457a89160d0b4b62f1`  
		Last Modified: Thu, 06 Oct 2022 05:04:58 GMT  
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
