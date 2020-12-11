## `spiped:latest`

```console
$ docker pull spiped@sha256:8e17d6e90ce440798837886b99327307c27fca74736a2318862a84122569405f
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

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:2a1562d9a8c8bc88d3d6dd14ca19efb88a99fc683968c7e5c5bb643954121da8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36273352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c227ab9e0eaf1b392d1b5ad6a0c3ce294258575158df25fb6c6d0654ee53e911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:10:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:10:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:10:13 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:10:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:10:44 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:10:44 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:10:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:10:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:10:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3417f37af9b9596fad115617f18df29172cc46a854cdc7055a23f38145a58f7`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5044f1165e0e44070848df158eac6e4c5ec565dede6fe9b50224d8089d26c`  
		Last Modified: Wed, 18 Nov 2020 16:11:04 GMT  
		Size: 2.1 MB (2128095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2077c0ed9103b638fe9f16fe236d093e5d52832f7df0295e05f0ede70ff45`  
		Last Modified: Wed, 18 Nov 2020 16:11:05 GMT  
		Size: 7.0 MB (7037598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bad379660d3c468029ddb245cf2b551b49d9b11a892e0c3ab55d00816d856`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4787b232f101a29c0a4c7ca9a61effad8f7bbb98ef9f83a613b1815b923c38d`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8382a6d947e1325a13a4418514b4e1778ca88be8206102eb0e3d3372ecc45ae9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32165056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d4b761eea34290114eb674784d79a9ba452ccfc459a243cb5c63ef7589073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 03:18:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 03:18:36 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 03:18:37 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 03:18:38 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 03:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 03:19:44 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 03:19:46 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 03:19:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db33d41ae1e9c76b9469640f87f593bb4644e3085f6a94fc2ed1985923392019`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e63c2f068f85d42076f8db5942ea78c569062bb6a52233f11c6baa2837c949`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.8 MB (1839441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bd0e0488057327d00c2c57a4d54689cbfc3bf3191ed03cb5f3461b70ee4a14`  
		Last Modified: Fri, 11 Dec 2020 03:20:13 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e867722c47de78ee7eddc4dabbed59b1c64da9e19394ea95d06872535d363`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe8c65d2ad6f0615a68f49a04f3388fedbe1fda01bbfd203fc4487a775ce6b`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:704c22b8b676b28651bdfbc6c270305a1d9c51dd839140ea45ac633c07afa4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdf237415bc56dd43224e7632a35235757d01c6868a15b0053e72466291cd22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:23:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:24:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:24:08 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:24:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:24:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:25:23 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:25:34 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b998896ae01086d1d742538d6adf34407de566efe82ebee5c53075ea9cdf1cf`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09275dfac82d12984d43305a0c4751236ff1270dfa9d4233c677b164cbd7b997`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 2.0 MB (2007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0a55a486b4a21452caace28f1c3f2202530083726583e2a4cd34ea385c9df`  
		Last Modified: Wed, 18 Nov 2020 16:26:11 GMT  
		Size: 5.9 MB (5905523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab3d8fdb677571f99ea2d30d6662ffc0707ad0bc61ce5daf5793fd5ad700a`  
		Last Modified: Wed, 18 Nov 2020 16:26:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc91fb24b5ded88e1a0ae7d5da9a99894c51155f175d6485b1f2882bab175b3`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:801fff27925c8e87ed9c5de2b32b74b636299c69fdbae15c814213d2086e2ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e191926eaea1d0c33716adeb209444a2e64bfae48ecff245fd0ce5f35af1afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:22:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 04:23:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:23:04 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:23:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:23:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 04:25:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:26:04 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:26:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:26:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f5dac353b2538492cef6c8c584ca52b4b8a09452919772325c53333df359b`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51102f02eff28acc6eb89231a81a67a0f7586b40ec7c9406c5e73657b73f92c1`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 2.2 MB (2225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec749be77d5a19cc47dedd00097160b1f0220d9d05ab73bd0d939594be46734f`  
		Last Modified: Fri, 11 Dec 2020 04:28:19 GMT  
		Size: 6.7 MB (6743253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6015004f4454ca6970c723ed1af34bbf7503bca68db79498b742edb6ce292c65`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c5c4333284617f343979a2ae448d1fbdb1580e6c6c41b24d15ee91c92029`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
