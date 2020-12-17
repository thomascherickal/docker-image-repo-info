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
$ docker pull spiped@sha256:49ce008f1914ccbf54fddf359fd9347255d6b81b362abb051b33ca1501b14ade
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
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:49ce008f1914ccbf54fddf359fd9347255d6b81b362abb051b33ca1501b14ade
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
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:49ce008f1914ccbf54fddf359fd9347255d6b81b362abb051b33ca1501b14ade
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
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:49ce008f1914ccbf54fddf359fd9347255d6b81b362abb051b33ca1501b14ade
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
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
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
