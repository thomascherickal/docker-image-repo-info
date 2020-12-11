<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:0145321212df052b489f5fef55ab3840bbb95ec8b3f418ffd7d5ac1a8bbcd075
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:b70503b69019891d4cae6a73067331efbf9c08f4e55a87ca0d408079fa6d25e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36267459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec44c1c0ed84b7fbe46f9d5453e100c34dea0c499dd852232c4a006bef9457a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 13:47:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 13:47:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:47:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:48:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 13:48:40 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:48:40 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:48:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:48:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:48:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f088369daceaf12c60584296e97813fb90183b2fff771160b1fd96b7c5937fa`  
		Last Modified: Fri, 11 Dec 2020 13:49:33 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeee36f70866684ce2fdd7d0e5598b3a084def283faa4a6d781bc3acda81ca`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 2.1 MB (2128414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6952ade103afb5f7675b378b1bb1cfb3dc59fe93338f7809d23abf406a5651`  
		Last Modified: Fri, 11 Dec 2020 13:49:35 GMT  
		Size: 7.0 MB (7037576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02814f9871b1bbfc2ac4ff5a867d76c19768ccc662a529a1f0f4f9e7430d1327`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd233c9045827a349549f1127fd653a92dea5892d87f2a6b4366a57109f087`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

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

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a513890a4a60df2247f6dccc7653cabb7aeeaf714f61d5a033254c52cf53bbd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29755145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e60d806bd81493904ea4aa090f734e8521097248805928bf5ebfe01796e74a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:27:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:27:20 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:27:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:27:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:29:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:29:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:29:21 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:29:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:29:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70eaca4fcc4bf8d5349c4c51729a8a5fe4ec5096738b125906bc6a61321a67`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bb05d6edfa8afd9da042285cc1b838af06ff979d214eb61fca2cadc9874ef`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.8 MB (1759685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f301c7b3184b18c5c2b0e251dffb42d3b9a5a0afa07dad8c390a4c6e116c48a`  
		Last Modified: Fri, 11 Dec 2020 15:31:08 GMT  
		Size: 5.3 MB (5285581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d3717dd7447cb44b962f4371cc3b97e1f584a494854168c916acc403eabbf`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1005525dfe4639b2d06ca88406938d747ca514b6a7860d2e6e1827089ee3a178`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c39957371b54dec0f5035640166669330fd33bc8a933bb271083b1bfb5cb2e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c1a1bbf83b27152cd44e528cc169a71a780e6c43394b0eaa524d0294edda1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:10:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:10:57 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:10:59 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:11:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:11:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:12:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:12:58 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:12:59 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:13:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:13:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777b01c09490eb8a60024360d8c297492fed4d246ec064eea91ef22d7520ca9`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bd8e2ecbacaf68ce5cfa1223a89f70cde7e3fc10b5d5b000303944c328c71`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 2.0 MB (2007879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855018be21026b8daea564c92a38b64d55e8e6230d01c005c180982daa00a1a5`  
		Last Modified: Fri, 11 Dec 2020 15:14:51 GMT  
		Size: 5.9 MB (5905564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0f966b8d1a0ae3352aaea3a99e3bf3cc63968735baaa4f94d4b5a6ef7bd4d9`  
		Last Modified: Fri, 11 Dec 2020 15:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1367c4fe725130c3f5e952f8de259dc52c87eed2ad61f165dbe0570549db`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:87bcda61e147fbb82abf403b3f949cc538ead86b0d4a3c8e57d67470cecea2df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41525528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb1d7d1ddc31b0ade4574e83588b815b45e1c379ffa32b2197a5d229a1ad606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:43:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 21:43:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 21:44:08 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:08 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af34c29f353c648ead0ab29c798a6d35b9e44dd1b5e34f6f96d74bc6bc1bf6`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bca0243e7a14ad567c4236c55819f0c6494082d3ab31381cc43349c9d7d4da`  
		Last Modified: Fri, 11 Dec 2020 21:44:56 GMT  
		Size: 2.1 MB (2132541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb869285df2e67da209d9cea554b6ffb713f59ad6fb106052ce2bf8d9b80b1b`  
		Last Modified: Fri, 11 Dec 2020 21:44:58 GMT  
		Size: 11.6 MB (11633234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd191981c0d2ce6722e39be186a94cfebcf3c768b4256bf9f709a2a2410379`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f4c5bc92eb9599f23b3b00ab05cb1c7f3dd9a3db5849786cc2bd9362623cf`  
		Last Modified: Fri, 11 Dec 2020 21:44:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:3980e91094fdd4eb3445349ec70494774082b478940c4db737b1cb7e4041eec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33900635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a92365cc5751331561e294d04907b4bd5a18c8d8a42009e19654002fbdf5cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:38:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:39:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:40:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:40:15 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:40:15 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:40:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:40:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:40:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27a37c8b2b631512a43f72ab8628244a7fd00774bbcf78d86fb6fd23488332`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91356804f75d117151c24b7824d4531df4012687cdcd1013906d86eff42404e1`  
		Last Modified: Fri, 11 Dec 2020 15:40:42 GMT  
		Size: 1.7 MB (1712328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb01417bef7602410870d979b8b3a38ec2dc991751a91c032700042ac00a`  
		Last Modified: Fri, 11 Dec 2020 15:40:47 GMT  
		Size: 6.4 MB (6416253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150db14f59de441192315b01a36447e87b530f23b43ca19bab483d51fdcac75e`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45792ec3ccf32743d729d912b0f84c8ac12f893d80f5a088e8a65ee4da400d6d`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

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

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:0145321212df052b489f5fef55ab3840bbb95ec8b3f418ffd7d5ac1a8bbcd075
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:b70503b69019891d4cae6a73067331efbf9c08f4e55a87ca0d408079fa6d25e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36267459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec44c1c0ed84b7fbe46f9d5453e100c34dea0c499dd852232c4a006bef9457a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 13:47:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 13:47:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:47:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:48:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 13:48:40 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:48:40 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:48:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:48:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:48:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f088369daceaf12c60584296e97813fb90183b2fff771160b1fd96b7c5937fa`  
		Last Modified: Fri, 11 Dec 2020 13:49:33 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeee36f70866684ce2fdd7d0e5598b3a084def283faa4a6d781bc3acda81ca`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 2.1 MB (2128414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6952ade103afb5f7675b378b1bb1cfb3dc59fe93338f7809d23abf406a5651`  
		Last Modified: Fri, 11 Dec 2020 13:49:35 GMT  
		Size: 7.0 MB (7037576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02814f9871b1bbfc2ac4ff5a867d76c19768ccc662a529a1f0f4f9e7430d1327`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd233c9045827a349549f1127fd653a92dea5892d87f2a6b4366a57109f087`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

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

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a513890a4a60df2247f6dccc7653cabb7aeeaf714f61d5a033254c52cf53bbd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29755145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e60d806bd81493904ea4aa090f734e8521097248805928bf5ebfe01796e74a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:27:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:27:20 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:27:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:27:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:29:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:29:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:29:21 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:29:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:29:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70eaca4fcc4bf8d5349c4c51729a8a5fe4ec5096738b125906bc6a61321a67`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bb05d6edfa8afd9da042285cc1b838af06ff979d214eb61fca2cadc9874ef`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.8 MB (1759685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f301c7b3184b18c5c2b0e251dffb42d3b9a5a0afa07dad8c390a4c6e116c48a`  
		Last Modified: Fri, 11 Dec 2020 15:31:08 GMT  
		Size: 5.3 MB (5285581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d3717dd7447cb44b962f4371cc3b97e1f584a494854168c916acc403eabbf`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1005525dfe4639b2d06ca88406938d747ca514b6a7860d2e6e1827089ee3a178`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c39957371b54dec0f5035640166669330fd33bc8a933bb271083b1bfb5cb2e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c1a1bbf83b27152cd44e528cc169a71a780e6c43394b0eaa524d0294edda1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:10:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:10:57 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:10:59 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:11:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:11:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:12:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:12:58 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:12:59 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:13:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:13:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777b01c09490eb8a60024360d8c297492fed4d246ec064eea91ef22d7520ca9`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bd8e2ecbacaf68ce5cfa1223a89f70cde7e3fc10b5d5b000303944c328c71`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 2.0 MB (2007879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855018be21026b8daea564c92a38b64d55e8e6230d01c005c180982daa00a1a5`  
		Last Modified: Fri, 11 Dec 2020 15:14:51 GMT  
		Size: 5.9 MB (5905564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0f966b8d1a0ae3352aaea3a99e3bf3cc63968735baaa4f94d4b5a6ef7bd4d9`  
		Last Modified: Fri, 11 Dec 2020 15:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1367c4fe725130c3f5e952f8de259dc52c87eed2ad61f165dbe0570549db`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:87bcda61e147fbb82abf403b3f949cc538ead86b0d4a3c8e57d67470cecea2df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41525528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb1d7d1ddc31b0ade4574e83588b815b45e1c379ffa32b2197a5d229a1ad606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:43:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 21:43:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 21:44:08 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:08 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af34c29f353c648ead0ab29c798a6d35b9e44dd1b5e34f6f96d74bc6bc1bf6`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bca0243e7a14ad567c4236c55819f0c6494082d3ab31381cc43349c9d7d4da`  
		Last Modified: Fri, 11 Dec 2020 21:44:56 GMT  
		Size: 2.1 MB (2132541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb869285df2e67da209d9cea554b6ffb713f59ad6fb106052ce2bf8d9b80b1b`  
		Last Modified: Fri, 11 Dec 2020 21:44:58 GMT  
		Size: 11.6 MB (11633234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd191981c0d2ce6722e39be186a94cfebcf3c768b4256bf9f709a2a2410379`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f4c5bc92eb9599f23b3b00ab05cb1c7f3dd9a3db5849786cc2bd9362623cf`  
		Last Modified: Fri, 11 Dec 2020 21:44:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:3980e91094fdd4eb3445349ec70494774082b478940c4db737b1cb7e4041eec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33900635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a92365cc5751331561e294d04907b4bd5a18c8d8a42009e19654002fbdf5cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:38:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:39:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:40:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:40:15 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:40:15 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:40:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:40:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:40:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27a37c8b2b631512a43f72ab8628244a7fd00774bbcf78d86fb6fd23488332`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91356804f75d117151c24b7824d4531df4012687cdcd1013906d86eff42404e1`  
		Last Modified: Fri, 11 Dec 2020 15:40:42 GMT  
		Size: 1.7 MB (1712328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb01417bef7602410870d979b8b3a38ec2dc991751a91c032700042ac00a`  
		Last Modified: Fri, 11 Dec 2020 15:40:47 GMT  
		Size: 6.4 MB (6416253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150db14f59de441192315b01a36447e87b530f23b43ca19bab483d51fdcac75e`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45792ec3ccf32743d729d912b0f84c8ac12f893d80f5a088e8a65ee4da400d6d`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

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

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:0145321212df052b489f5fef55ab3840bbb95ec8b3f418ffd7d5ac1a8bbcd075
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:b70503b69019891d4cae6a73067331efbf9c08f4e55a87ca0d408079fa6d25e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36267459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec44c1c0ed84b7fbe46f9d5453e100c34dea0c499dd852232c4a006bef9457a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 13:47:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 13:47:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:47:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:48:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 13:48:40 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:48:40 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:48:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:48:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:48:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f088369daceaf12c60584296e97813fb90183b2fff771160b1fd96b7c5937fa`  
		Last Modified: Fri, 11 Dec 2020 13:49:33 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeee36f70866684ce2fdd7d0e5598b3a084def283faa4a6d781bc3acda81ca`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 2.1 MB (2128414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6952ade103afb5f7675b378b1bb1cfb3dc59fe93338f7809d23abf406a5651`  
		Last Modified: Fri, 11 Dec 2020 13:49:35 GMT  
		Size: 7.0 MB (7037576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02814f9871b1bbfc2ac4ff5a867d76c19768ccc662a529a1f0f4f9e7430d1327`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd233c9045827a349549f1127fd653a92dea5892d87f2a6b4366a57109f087`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

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

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a513890a4a60df2247f6dccc7653cabb7aeeaf714f61d5a033254c52cf53bbd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29755145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e60d806bd81493904ea4aa090f734e8521097248805928bf5ebfe01796e74a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:27:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:27:20 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:27:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:27:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:29:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:29:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:29:21 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:29:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:29:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70eaca4fcc4bf8d5349c4c51729a8a5fe4ec5096738b125906bc6a61321a67`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bb05d6edfa8afd9da042285cc1b838af06ff979d214eb61fca2cadc9874ef`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.8 MB (1759685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f301c7b3184b18c5c2b0e251dffb42d3b9a5a0afa07dad8c390a4c6e116c48a`  
		Last Modified: Fri, 11 Dec 2020 15:31:08 GMT  
		Size: 5.3 MB (5285581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d3717dd7447cb44b962f4371cc3b97e1f584a494854168c916acc403eabbf`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1005525dfe4639b2d06ca88406938d747ca514b6a7860d2e6e1827089ee3a178`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c39957371b54dec0f5035640166669330fd33bc8a933bb271083b1bfb5cb2e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c1a1bbf83b27152cd44e528cc169a71a780e6c43394b0eaa524d0294edda1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:10:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:10:57 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:10:59 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:11:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:11:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:12:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:12:58 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:12:59 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:13:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:13:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777b01c09490eb8a60024360d8c297492fed4d246ec064eea91ef22d7520ca9`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bd8e2ecbacaf68ce5cfa1223a89f70cde7e3fc10b5d5b000303944c328c71`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 2.0 MB (2007879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855018be21026b8daea564c92a38b64d55e8e6230d01c005c180982daa00a1a5`  
		Last Modified: Fri, 11 Dec 2020 15:14:51 GMT  
		Size: 5.9 MB (5905564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0f966b8d1a0ae3352aaea3a99e3bf3cc63968735baaa4f94d4b5a6ef7bd4d9`  
		Last Modified: Fri, 11 Dec 2020 15:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1367c4fe725130c3f5e952f8de259dc52c87eed2ad61f165dbe0570549db`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:87bcda61e147fbb82abf403b3f949cc538ead86b0d4a3c8e57d67470cecea2df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41525528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb1d7d1ddc31b0ade4574e83588b815b45e1c379ffa32b2197a5d229a1ad606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:43:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 21:43:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 21:44:08 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:08 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af34c29f353c648ead0ab29c798a6d35b9e44dd1b5e34f6f96d74bc6bc1bf6`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bca0243e7a14ad567c4236c55819f0c6494082d3ab31381cc43349c9d7d4da`  
		Last Modified: Fri, 11 Dec 2020 21:44:56 GMT  
		Size: 2.1 MB (2132541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb869285df2e67da209d9cea554b6ffb713f59ad6fb106052ce2bf8d9b80b1b`  
		Last Modified: Fri, 11 Dec 2020 21:44:58 GMT  
		Size: 11.6 MB (11633234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd191981c0d2ce6722e39be186a94cfebcf3c768b4256bf9f709a2a2410379`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f4c5bc92eb9599f23b3b00ab05cb1c7f3dd9a3db5849786cc2bd9362623cf`  
		Last Modified: Fri, 11 Dec 2020 21:44:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:3980e91094fdd4eb3445349ec70494774082b478940c4db737b1cb7e4041eec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33900635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a92365cc5751331561e294d04907b4bd5a18c8d8a42009e19654002fbdf5cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:38:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:39:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:40:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:40:15 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:40:15 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:40:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:40:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:40:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27a37c8b2b631512a43f72ab8628244a7fd00774bbcf78d86fb6fd23488332`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91356804f75d117151c24b7824d4531df4012687cdcd1013906d86eff42404e1`  
		Last Modified: Fri, 11 Dec 2020 15:40:42 GMT  
		Size: 1.7 MB (1712328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb01417bef7602410870d979b8b3a38ec2dc991751a91c032700042ac00a`  
		Last Modified: Fri, 11 Dec 2020 15:40:47 GMT  
		Size: 6.4 MB (6416253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150db14f59de441192315b01a36447e87b530f23b43ca19bab483d51fdcac75e`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45792ec3ccf32743d729d912b0f84c8ac12f893d80f5a088e8a65ee4da400d6d`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

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

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:f158db94fd4f943dab2d83295c0c6e2731b8123a4f19f6f49322295ce8b2c2d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b36665543fb15f1237e247cdc1e31c5a124077203da11818b3b0fb136d17aaf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb5c0620d02cde7a18e4d721e93454411385f48f32a609809dba66e0f15fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 13:48:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:49:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 13:49:17 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:49:17 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:49:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:49:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:49:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71fbe7bc43fd8f5c2e88856836ab0cb20daedafbb7d94c94fc57e33b77175d`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0dffb6112c85d6e2f2b928b1631fe4cdf436c387dbc9c951cb07f02b25232`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa205c2404dd6d7a1c86ee038388ed3bd317b221dcfcd16cdd143b894862490`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 211.4 KB (211440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502754e69f8659cd0de6baec7bff058cbb3e7ee303310b7b52e9bf4ee6c1e29b`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712ab91ea61b13fda64e87e604f0e50c14c822f3f9b713992cfef0ff3bdf91dc`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:b3a90a9d2dfda78464003631c5ced5e74a88e33d37fb7e00706247c06e3e62fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c47a888b294c38da1db4714cf43ea4146f1aa8e7f1f389209d83f6aa5b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:29:45 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:29:50 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:29:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:29:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:29:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:30:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:30:22 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:30:23 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:30:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:30:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b2d4dad8d362fffcdec7d8c1d7c97d7de39e9a5eece83234d8c2cd84903f68`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9922214e3002ea40e3cd5f9128f90dab186be6cbb6d1858ca0c46123b8d04`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e926fd9cf24045ba66a4570c4770800908a41ff32640a231d5a67e7124a7dba`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 191.6 KB (191641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1908264eb97b44ff1f2c1f2d4580427ff5759da2c07e1271041f84708cf626d7`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b49057b37c88c17261eba50168832ff2fb073dcde023aaebaf12222e1c0fb54`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3ffffa76be1c4efabf31a89d1b07248ab0c322d51cb891128609beb1a119ad25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4bdcf84f14049fcf62e12452cb30552c4831652fe073f5c45f8171837b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:13:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:13:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:13:27 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:13:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:13:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:14:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:14:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:14:20 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:14:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:14:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:14:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc04d94cd67b3040c524d9c7dae1d4e5a8665d5d8481eca8e3e3fc338cf96b97`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bec32bc4579f02b12688cb1e53b4aeee41a24943f1da0c766b3936c78a6fca9`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ea176f26cf4e6711dfe6a720b1fb1214d7dbf99930a0f58c226aaaed5e13a`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 203.8 KB (203817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e6d1a9aa36fc516b44efaed84c94d2a64bf6896b159100f8b63d29443240`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b808f34294db1e2726b3a16deafd555c57acbffe4c9e3c07ba4dadaa9bdc1c`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:04b442844d79a30e1bf8265a917b2017e5dac178c8353a7b91f93ed7f37a9873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a29fcba7c398a1c8d8e9bf496c410859b4e94baedd16580dd239eb348bb960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 21:44:15 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 21:44:16 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:44:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 21:44:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9711e94e3d4acb87ac979443e476919a1d9433dcc45d2167186c7c8de6918b8`  
		Last Modified: Fri, 11 Dec 2020 21:45:08 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb34a0ca99748b461d39274e5cb1333c4f4c120b7f9e257381d6ae484dac90f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f73a702f9c5fe81bbc01d32a43dbcad48785f544c26f9e8484188b6c02bf825`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 221.2 KB (221227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177df2fbfd860811a4ba157fa1d25cd799c8425d6f5cc09767bad5a13434cc2f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486cd174808c0b19cec9b2349bc1fd370857e063a0c0a09ff78cacafd19f25a`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:f158db94fd4f943dab2d83295c0c6e2731b8123a4f19f6f49322295ce8b2c2d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b36665543fb15f1237e247cdc1e31c5a124077203da11818b3b0fb136d17aaf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb5c0620d02cde7a18e4d721e93454411385f48f32a609809dba66e0f15fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 13:48:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:49:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 13:49:17 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:49:17 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:49:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:49:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:49:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71fbe7bc43fd8f5c2e88856836ab0cb20daedafbb7d94c94fc57e33b77175d`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0dffb6112c85d6e2f2b928b1631fe4cdf436c387dbc9c951cb07f02b25232`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa205c2404dd6d7a1c86ee038388ed3bd317b221dcfcd16cdd143b894862490`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 211.4 KB (211440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502754e69f8659cd0de6baec7bff058cbb3e7ee303310b7b52e9bf4ee6c1e29b`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712ab91ea61b13fda64e87e604f0e50c14c822f3f9b713992cfef0ff3bdf91dc`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:b3a90a9d2dfda78464003631c5ced5e74a88e33d37fb7e00706247c06e3e62fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c47a888b294c38da1db4714cf43ea4146f1aa8e7f1f389209d83f6aa5b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:29:45 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:29:50 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:29:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:29:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:29:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:30:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:30:22 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:30:23 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:30:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:30:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b2d4dad8d362fffcdec7d8c1d7c97d7de39e9a5eece83234d8c2cd84903f68`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9922214e3002ea40e3cd5f9128f90dab186be6cbb6d1858ca0c46123b8d04`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e926fd9cf24045ba66a4570c4770800908a41ff32640a231d5a67e7124a7dba`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 191.6 KB (191641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1908264eb97b44ff1f2c1f2d4580427ff5759da2c07e1271041f84708cf626d7`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b49057b37c88c17261eba50168832ff2fb073dcde023aaebaf12222e1c0fb54`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3ffffa76be1c4efabf31a89d1b07248ab0c322d51cb891128609beb1a119ad25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4bdcf84f14049fcf62e12452cb30552c4831652fe073f5c45f8171837b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:13:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:13:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:13:27 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:13:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:13:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:14:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:14:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:14:20 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:14:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:14:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:14:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc04d94cd67b3040c524d9c7dae1d4e5a8665d5d8481eca8e3e3fc338cf96b97`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bec32bc4579f02b12688cb1e53b4aeee41a24943f1da0c766b3936c78a6fca9`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ea176f26cf4e6711dfe6a720b1fb1214d7dbf99930a0f58c226aaaed5e13a`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 203.8 KB (203817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e6d1a9aa36fc516b44efaed84c94d2a64bf6896b159100f8b63d29443240`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b808f34294db1e2726b3a16deafd555c57acbffe4c9e3c07ba4dadaa9bdc1c`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:04b442844d79a30e1bf8265a917b2017e5dac178c8353a7b91f93ed7f37a9873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a29fcba7c398a1c8d8e9bf496c410859b4e94baedd16580dd239eb348bb960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 21:44:15 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 21:44:16 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:44:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 21:44:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9711e94e3d4acb87ac979443e476919a1d9433dcc45d2167186c7c8de6918b8`  
		Last Modified: Fri, 11 Dec 2020 21:45:08 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb34a0ca99748b461d39274e5cb1333c4f4c120b7f9e257381d6ae484dac90f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f73a702f9c5fe81bbc01d32a43dbcad48785f544c26f9e8484188b6c02bf825`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 221.2 KB (221227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177df2fbfd860811a4ba157fa1d25cd799c8425d6f5cc09767bad5a13434cc2f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486cd174808c0b19cec9b2349bc1fd370857e063a0c0a09ff78cacafd19f25a`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:f158db94fd4f943dab2d83295c0c6e2731b8123a4f19f6f49322295ce8b2c2d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b36665543fb15f1237e247cdc1e31c5a124077203da11818b3b0fb136d17aaf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb5c0620d02cde7a18e4d721e93454411385f48f32a609809dba66e0f15fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 13:48:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:49:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 13:49:17 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:49:17 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:49:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:49:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:49:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71fbe7bc43fd8f5c2e88856836ab0cb20daedafbb7d94c94fc57e33b77175d`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0dffb6112c85d6e2f2b928b1631fe4cdf436c387dbc9c951cb07f02b25232`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa205c2404dd6d7a1c86ee038388ed3bd317b221dcfcd16cdd143b894862490`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 211.4 KB (211440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502754e69f8659cd0de6baec7bff058cbb3e7ee303310b7b52e9bf4ee6c1e29b`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712ab91ea61b13fda64e87e604f0e50c14c822f3f9b713992cfef0ff3bdf91dc`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:b3a90a9d2dfda78464003631c5ced5e74a88e33d37fb7e00706247c06e3e62fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c47a888b294c38da1db4714cf43ea4146f1aa8e7f1f389209d83f6aa5b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:29:45 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:29:50 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:29:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:29:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:29:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:30:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:30:22 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:30:23 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:30:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:30:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b2d4dad8d362fffcdec7d8c1d7c97d7de39e9a5eece83234d8c2cd84903f68`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9922214e3002ea40e3cd5f9128f90dab186be6cbb6d1858ca0c46123b8d04`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e926fd9cf24045ba66a4570c4770800908a41ff32640a231d5a67e7124a7dba`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 191.6 KB (191641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1908264eb97b44ff1f2c1f2d4580427ff5759da2c07e1271041f84708cf626d7`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b49057b37c88c17261eba50168832ff2fb073dcde023aaebaf12222e1c0fb54`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3ffffa76be1c4efabf31a89d1b07248ab0c322d51cb891128609beb1a119ad25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4bdcf84f14049fcf62e12452cb30552c4831652fe073f5c45f8171837b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:13:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:13:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:13:27 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:13:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:13:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:14:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:14:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:14:20 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:14:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:14:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:14:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc04d94cd67b3040c524d9c7dae1d4e5a8665d5d8481eca8e3e3fc338cf96b97`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bec32bc4579f02b12688cb1e53b4aeee41a24943f1da0c766b3936c78a6fca9`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ea176f26cf4e6711dfe6a720b1fb1214d7dbf99930a0f58c226aaaed5e13a`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 203.8 KB (203817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e6d1a9aa36fc516b44efaed84c94d2a64bf6896b159100f8b63d29443240`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b808f34294db1e2726b3a16deafd555c57acbffe4c9e3c07ba4dadaa9bdc1c`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:04b442844d79a30e1bf8265a917b2017e5dac178c8353a7b91f93ed7f37a9873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a29fcba7c398a1c8d8e9bf496c410859b4e94baedd16580dd239eb348bb960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 21:44:15 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 21:44:16 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:44:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 21:44:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9711e94e3d4acb87ac979443e476919a1d9433dcc45d2167186c7c8de6918b8`  
		Last Modified: Fri, 11 Dec 2020 21:45:08 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb34a0ca99748b461d39274e5cb1333c4f4c120b7f9e257381d6ae484dac90f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f73a702f9c5fe81bbc01d32a43dbcad48785f544c26f9e8484188b6c02bf825`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 221.2 KB (221227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177df2fbfd860811a4ba157fa1d25cd799c8425d6f5cc09767bad5a13434cc2f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486cd174808c0b19cec9b2349bc1fd370857e063a0c0a09ff78cacafd19f25a`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:f158db94fd4f943dab2d83295c0c6e2731b8123a4f19f6f49322295ce8b2c2d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b36665543fb15f1237e247cdc1e31c5a124077203da11818b3b0fb136d17aaf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb5c0620d02cde7a18e4d721e93454411385f48f32a609809dba66e0f15fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 13:48:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:49:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 13:49:17 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:49:17 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:49:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:49:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:49:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71fbe7bc43fd8f5c2e88856836ab0cb20daedafbb7d94c94fc57e33b77175d`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0dffb6112c85d6e2f2b928b1631fe4cdf436c387dbc9c951cb07f02b25232`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa205c2404dd6d7a1c86ee038388ed3bd317b221dcfcd16cdd143b894862490`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 211.4 KB (211440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502754e69f8659cd0de6baec7bff058cbb3e7ee303310b7b52e9bf4ee6c1e29b`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712ab91ea61b13fda64e87e604f0e50c14c822f3f9b713992cfef0ff3bdf91dc`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:b3a90a9d2dfda78464003631c5ced5e74a88e33d37fb7e00706247c06e3e62fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c47a888b294c38da1db4714cf43ea4146f1aa8e7f1f389209d83f6aa5b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:29:45 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:29:50 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:29:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:29:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:29:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:30:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:30:22 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:30:23 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:30:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:30:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b2d4dad8d362fffcdec7d8c1d7c97d7de39e9a5eece83234d8c2cd84903f68`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9922214e3002ea40e3cd5f9128f90dab186be6cbb6d1858ca0c46123b8d04`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e926fd9cf24045ba66a4570c4770800908a41ff32640a231d5a67e7124a7dba`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 191.6 KB (191641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1908264eb97b44ff1f2c1f2d4580427ff5759da2c07e1271041f84708cf626d7`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b49057b37c88c17261eba50168832ff2fb073dcde023aaebaf12222e1c0fb54`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3ffffa76be1c4efabf31a89d1b07248ab0c322d51cb891128609beb1a119ad25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4bdcf84f14049fcf62e12452cb30552c4831652fe073f5c45f8171837b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:13:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:13:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:13:27 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:13:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:13:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:14:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:14:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:14:20 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:14:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:14:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:14:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc04d94cd67b3040c524d9c7dae1d4e5a8665d5d8481eca8e3e3fc338cf96b97`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bec32bc4579f02b12688cb1e53b4aeee41a24943f1da0c766b3936c78a6fca9`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ea176f26cf4e6711dfe6a720b1fb1214d7dbf99930a0f58c226aaaed5e13a`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 203.8 KB (203817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e6d1a9aa36fc516b44efaed84c94d2a64bf6896b159100f8b63d29443240`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b808f34294db1e2726b3a16deafd555c57acbffe4c9e3c07ba4dadaa9bdc1c`  
		Last Modified: Fri, 11 Dec 2020 15:15:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:04b442844d79a30e1bf8265a917b2017e5dac178c8353a7b91f93ed7f37a9873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a29fcba7c398a1c8d8e9bf496c410859b4e94baedd16580dd239eb348bb960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 21:44:15 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 21:44:16 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:44:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 21:44:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9711e94e3d4acb87ac979443e476919a1d9433dcc45d2167186c7c8de6918b8`  
		Last Modified: Fri, 11 Dec 2020 21:45:08 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb34a0ca99748b461d39274e5cb1333c4f4c120b7f9e257381d6ae484dac90f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f73a702f9c5fe81bbc01d32a43dbcad48785f544c26f9e8484188b6c02bf825`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 221.2 KB (221227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177df2fbfd860811a4ba157fa1d25cd799c8425d6f5cc09767bad5a13434cc2f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486cd174808c0b19cec9b2349bc1fd370857e063a0c0a09ff78cacafd19f25a`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:0145321212df052b489f5fef55ab3840bbb95ec8b3f418ffd7d5ac1a8bbcd075
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
$ docker pull spiped@sha256:b70503b69019891d4cae6a73067331efbf9c08f4e55a87ca0d408079fa6d25e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36267459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec44c1c0ed84b7fbe46f9d5453e100c34dea0c499dd852232c4a006bef9457a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 13:47:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 13:47:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:47:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:47:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:48:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 13:48:40 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:48:40 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:48:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:48:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:48:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f088369daceaf12c60584296e97813fb90183b2fff771160b1fd96b7c5937fa`  
		Last Modified: Fri, 11 Dec 2020 13:49:33 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeee36f70866684ce2fdd7d0e5598b3a084def283faa4a6d781bc3acda81ca`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 2.1 MB (2128414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6952ade103afb5f7675b378b1bb1cfb3dc59fe93338f7809d23abf406a5651`  
		Last Modified: Fri, 11 Dec 2020 13:49:35 GMT  
		Size: 7.0 MB (7037576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02814f9871b1bbfc2ac4ff5a867d76c19768ccc662a529a1f0f4f9e7430d1327`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bd233c9045827a349549f1127fd653a92dea5892d87f2a6b4366a57109f087`  
		Last Modified: Fri, 11 Dec 2020 13:49:34 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:a513890a4a60df2247f6dccc7653cabb7aeeaf714f61d5a033254c52cf53bbd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29755145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e60d806bd81493904ea4aa090f734e8521097248805928bf5ebfe01796e74a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:26:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:27:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:27:20 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:27:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:27:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:29:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:29:19 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:29:21 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:29:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:29:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70eaca4fcc4bf8d5349c4c51729a8a5fe4ec5096738b125906bc6a61321a67`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bb05d6edfa8afd9da042285cc1b838af06ff979d214eb61fca2cadc9874ef`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 1.8 MB (1759685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f301c7b3184b18c5c2b0e251dffb42d3b9a5a0afa07dad8c390a4c6e116c48a`  
		Last Modified: Fri, 11 Dec 2020 15:31:08 GMT  
		Size: 5.3 MB (5285581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d3717dd7447cb44b962f4371cc3b97e1f584a494854168c916acc403eabbf`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1005525dfe4639b2d06ca88406938d747ca514b6a7860d2e6e1827089ee3a178`  
		Last Modified: Fri, 11 Dec 2020 15:31:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c39957371b54dec0f5035640166669330fd33bc8a933bb271083b1bfb5cb2e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c1a1bbf83b27152cd44e528cc169a71a780e6c43394b0eaa524d0294edda1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:10:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:10:57 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:10:59 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:11:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:11:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:12:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:12:58 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:12:59 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:13:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:13:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777b01c09490eb8a60024360d8c297492fed4d246ec064eea91ef22d7520ca9`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bd8e2ecbacaf68ce5cfa1223a89f70cde7e3fc10b5d5b000303944c328c71`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 2.0 MB (2007879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855018be21026b8daea564c92a38b64d55e8e6230d01c005c180982daa00a1a5`  
		Last Modified: Fri, 11 Dec 2020 15:14:51 GMT  
		Size: 5.9 MB (5905564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0f966b8d1a0ae3352aaea3a99e3bf3cc63968735baaa4f94d4b5a6ef7bd4d9`  
		Last Modified: Fri, 11 Dec 2020 15:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1367c4fe725130c3f5e952f8de259dc52c87eed2ad61f165dbe0570549db`  
		Last Modified: Fri, 11 Dec 2020 15:14:50 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:87bcda61e147fbb82abf403b3f949cc538ead86b0d4a3c8e57d67470cecea2df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41525528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb1d7d1ddc31b0ade4574e83588b815b45e1c379ffa32b2197a5d229a1ad606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:43:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 21:43:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 21:44:08 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:08 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af34c29f353c648ead0ab29c798a6d35b9e44dd1b5e34f6f96d74bc6bc1bf6`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bca0243e7a14ad567c4236c55819f0c6494082d3ab31381cc43349c9d7d4da`  
		Last Modified: Fri, 11 Dec 2020 21:44:56 GMT  
		Size: 2.1 MB (2132541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb869285df2e67da209d9cea554b6ffb713f59ad6fb106052ce2bf8d9b80b1b`  
		Last Modified: Fri, 11 Dec 2020 21:44:58 GMT  
		Size: 11.6 MB (11633234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd191981c0d2ce6722e39be186a94cfebcf3c768b4256bf9f709a2a2410379`  
		Last Modified: Fri, 11 Dec 2020 21:44:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34f4c5bc92eb9599f23b3b00ab05cb1c7f3dd9a3db5849786cc2bd9362623cf`  
		Last Modified: Fri, 11 Dec 2020 21:44:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:3980e91094fdd4eb3445349ec70494774082b478940c4db737b1cb7e4041eec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33900635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a92365cc5751331561e294d04907b4bd5a18c8d8a42009e19654002fbdf5cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:38:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 15:39:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:39:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:40:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 15:40:15 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:40:15 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:40:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:40:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:40:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27a37c8b2b631512a43f72ab8628244a7fd00774bbcf78d86fb6fd23488332`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91356804f75d117151c24b7824d4531df4012687cdcd1013906d86eff42404e1`  
		Last Modified: Fri, 11 Dec 2020 15:40:42 GMT  
		Size: 1.7 MB (1712328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb01417bef7602410870d979b8b3a38ec2dc991751a91c032700042ac00a`  
		Last Modified: Fri, 11 Dec 2020 15:40:47 GMT  
		Size: 6.4 MB (6416253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150db14f59de441192315b01a36447e87b530f23b43ca19bab483d51fdcac75e`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45792ec3ccf32743d729d912b0f84c8ac12f893d80f5a088e8a65ee4da400d6d`  
		Last Modified: Fri, 11 Dec 2020 15:40:41 GMT  
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
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
