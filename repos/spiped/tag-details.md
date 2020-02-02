<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.0`](#spiped160)
-	[`spiped:1.6.0-alpine`](#spiped160-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:a9f2d41c15a40c84435c70e5ef8cace5cee29cd1f84babe1ece1c40f4c2db8aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:94a496399350fa792c12e719637ec1b6288c9df7d1d958434b3bf6f1a4cb35a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7b9f24c6da4ff2db786e27df56dffad1979a1a1b3f8d30f090d43ac5026157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:15:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 06:15:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 06:15:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 06:15:40 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 06:15:40 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 06:15:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:15:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:15:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731399cccc6f318fc2161064db19deeaa2fbb915888b6bfb4f788393478b1793`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd449eddd5c8ce7f92d05d131ce66ac8ec39d6d022327729918564f50d41ec7c`  
		Last Modified: Sun, 02 Feb 2020 06:16:01 GMT  
		Size: 2.1 MB (2128004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc4057ac7a766f5ef045ce99563fa24f1a184dd5314c8c2278373e4e910b03`  
		Last Modified: Sun, 02 Feb 2020 06:16:03 GMT  
		Size: 7.0 MB (7027512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a5937d1f11dff98ab8deee7b992099bf6bc7c104bdb75997f4766ee01289e3`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24862150235a45dafb0089ae7493770b72db3c3d54c0fbf02d7d7540907797a9`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:46c09863fe9de71ed17fe3429d98937b35cca01042ce95a7cfac14a4940e5940
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4854892b43b9226b0bfec04d10d05520d1c3169732ba4d2496373730e06d6c3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:28:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 18:28:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:28:16 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 18:29:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 18:29:04 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 18:29:04 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 18:29:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 18:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 18:29:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd3ed7c8c7f6527fcca82864bf95939d859f70dbd259e58c7b77f2cb9b78fb9`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37608bc89418e7e427b153b07e0f00846c35f85e931ec816c2ec38c9142aaf2a`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.8 MB (1839087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d56a8f81afe86e05571a145096d08791146a0620bdad3a6b7f770d1e46742a`  
		Last Modified: Sat, 01 Feb 2020 18:29:26 GMT  
		Size: 5.5 MB (5472626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9936f33ba62b478e8d90beb45179853a937da89dc8a77ac60274d13f21144963`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774801a174976d8412993bef93bcc4432be10e2db2842e1d568ac473c9317643`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:740ad6efbf90726477deac506ce4164a29631a5ec5d250e48f524191dd95397e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71504de64d0ace9ede0f5de8448e4aad5e678a8538d54fd2b4586548219ff12f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:27:59 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 08:28:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 08:28:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 08:28:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 08:28:54 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 08:28:55 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 08:28:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:29:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cec23850f77792ec02c51a5c3d02d44ef577be63198b96c3d2d32f2e428abd1`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f287c58e653509527769eab1974b77bc7d6f5f0663686f24f171871a9b4d5`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.8 MB (1759406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012d5ec3a62094c0196d0f0f75875328f73bc5e10282349943f20ac1133a4bf`  
		Last Modified: Sun, 02 Feb 2020 08:29:29 GMT  
		Size: 5.3 MB (5279046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e5223531e65090bb4393cd1903cb614c531f1a4ce97dad6f506b9fd5d2c21`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05708d423c4906488d953a0fe15f13369c66cfd800315207045c3bde3c2e3717`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b2e581ed96cd38f9c3feb006901f524f67d672f3c304950ad03b5ba5d85df4b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33759933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5208ab9badd9219190a61349c33a61c6abb0f0c5a9f85c111d8041b17d14ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 11:01:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 11:02:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:02:13 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 11:02:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 11:02:57 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 11:02:58 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 11:02:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 11:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 11:02:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce433f8fd0317821392c343b5116cf0526b6490a1016133e563f1f6c91d4e11`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef79c479a4e994c1a71e4f53a3aac700f92a97e49a59f81c3651ed3c0e139c7d`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 2.0 MB (2007772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54caab845ffff5ee7f081cc3171aba5afdc35c073e36b4a85e13efcf745fa3f7`  
		Last Modified: Sun, 02 Feb 2020 11:03:22 GMT  
		Size: 5.9 MB (5899289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a866034f98905d2f1e9bc020a0fb9b076b92ae72b9ca92db777e18cb04949235`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe61640aba00e184e4ecf0094118dcac5ff70a4e7210c575880abc0076a66b2`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:9b08de941dfabf18ab82637496dd834891465c7825cf3233a85f978770c48762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18dc26279c852de9a9c175279765969a744c699027eab9660eb2727c85fe124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:33:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 09:33:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 09:34:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 09:34:08 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 09:34:08 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 09:34:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b4b2d4ef7209a4b74a85b2268886f21ac7062f11a659fdb2aa6f0778a168b1`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ba6ade7bf16194e5e43284dac9428686f878f227f7f6f6bf775a5b4ac308b`  
		Last Modified: Sun, 02 Feb 2020 09:34:37 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f581d8f56da9341f96479173d238146066351b343ba87abc58e8c5fb2bad72`  
		Last Modified: Sun, 02 Feb 2020 09:34:43 GMT  
		Size: 11.6 MB (11622885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bff5f4bc56cbd458b29d3af1f8a43c3959a79d96399e9edb29952312da744`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6758530d06a785788fe95501c1e5e54c659274c8b2e68be98bba7be1c8e4e`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:2af640b2e5e945fc7a2bbfbb758f836c601e7de4736cc7a2c153e2b6f2341de1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aacf013b516fb925973edd0d5747ae594d30843d4a6e7b05dc75bee90541d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:59:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 02:59:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:00:00 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 03:00:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 03:00:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 03:01:48 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 03:01:50 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 03:01:54 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 03:01:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:02:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a590754624a36c689aa2f868ae093bd0d238306deee026950720a1cef27c3`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d8bb6be0d52570c63debf54f56ca533bf2dd6c63d7ce8608f252b603f2cd7`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 2.2 MB (2224858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee10f5eebb2434c30ad4544e59ecc613b84e9c385e27ae8e436cae5bb7fd5d2`  
		Last Modified: Sun, 02 Feb 2020 03:02:34 GMT  
		Size: 6.7 MB (6735278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef1fcf1f9bae2a0a129a9e502f40627dd016d7570d2ad986f6701448edf1660`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad008d8b0be1cb3825d2601908169faa054d1f30e0e4168421f0672c24b2079a`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:4847e130e4505884571acd096a951f97c04043453c52945dd80eb985050af833
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33463886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52af50aad2f838fc10ccd8fd81eece8695e0daf0811b92c0ebad98de879ac18a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:21:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 22:21:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 22:21:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 22:21:37 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 22:21:37 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 22:21:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:21:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a991d51344d40c0dc65a4bbb295c13f9702296c25aaac1aef4d81bfc979b089`  
		Last Modified: Sat, 01 Feb 2020 22:21:51 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cde9e08e6e33966ecc6eee8880ae741ea240f38b9b7909c2a568a8e2dae10d`  
		Last Modified: Sat, 01 Feb 2020 22:21:56 GMT  
		Size: 1.8 MB (1821708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7642a6ebcfd2be1e13fc5075d371c0ed03f77d355a77755325555f6eb6ef8eb`  
		Last Modified: Sat, 01 Feb 2020 22:21:52 GMT  
		Size: 5.9 MB (5934595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33c4f7cbed3197ee9911e190eeb6e8fee8ed0d5ae49e1f2223d6bf93a9234e`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65e2452f41b088b369c8d479923a093961365f0f22a5e44f9c93fa2a67552ba`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:a9f2d41c15a40c84435c70e5ef8cace5cee29cd1f84babe1ece1c40f4c2db8aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:94a496399350fa792c12e719637ec1b6288c9df7d1d958434b3bf6f1a4cb35a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7b9f24c6da4ff2db786e27df56dffad1979a1a1b3f8d30f090d43ac5026157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:15:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 06:15:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 06:15:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 06:15:40 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 06:15:40 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 06:15:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:15:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:15:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731399cccc6f318fc2161064db19deeaa2fbb915888b6bfb4f788393478b1793`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd449eddd5c8ce7f92d05d131ce66ac8ec39d6d022327729918564f50d41ec7c`  
		Last Modified: Sun, 02 Feb 2020 06:16:01 GMT  
		Size: 2.1 MB (2128004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc4057ac7a766f5ef045ce99563fa24f1a184dd5314c8c2278373e4e910b03`  
		Last Modified: Sun, 02 Feb 2020 06:16:03 GMT  
		Size: 7.0 MB (7027512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a5937d1f11dff98ab8deee7b992099bf6bc7c104bdb75997f4766ee01289e3`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24862150235a45dafb0089ae7493770b72db3c3d54c0fbf02d7d7540907797a9`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:46c09863fe9de71ed17fe3429d98937b35cca01042ce95a7cfac14a4940e5940
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4854892b43b9226b0bfec04d10d05520d1c3169732ba4d2496373730e06d6c3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:28:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 18:28:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:28:16 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 18:29:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 18:29:04 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 18:29:04 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 18:29:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 18:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 18:29:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd3ed7c8c7f6527fcca82864bf95939d859f70dbd259e58c7b77f2cb9b78fb9`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37608bc89418e7e427b153b07e0f00846c35f85e931ec816c2ec38c9142aaf2a`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.8 MB (1839087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d56a8f81afe86e05571a145096d08791146a0620bdad3a6b7f770d1e46742a`  
		Last Modified: Sat, 01 Feb 2020 18:29:26 GMT  
		Size: 5.5 MB (5472626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9936f33ba62b478e8d90beb45179853a937da89dc8a77ac60274d13f21144963`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774801a174976d8412993bef93bcc4432be10e2db2842e1d568ac473c9317643`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:740ad6efbf90726477deac506ce4164a29631a5ec5d250e48f524191dd95397e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71504de64d0ace9ede0f5de8448e4aad5e678a8538d54fd2b4586548219ff12f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:27:59 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 08:28:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 08:28:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 08:28:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 08:28:54 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 08:28:55 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 08:28:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:29:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cec23850f77792ec02c51a5c3d02d44ef577be63198b96c3d2d32f2e428abd1`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f287c58e653509527769eab1974b77bc7d6f5f0663686f24f171871a9b4d5`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.8 MB (1759406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012d5ec3a62094c0196d0f0f75875328f73bc5e10282349943f20ac1133a4bf`  
		Last Modified: Sun, 02 Feb 2020 08:29:29 GMT  
		Size: 5.3 MB (5279046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e5223531e65090bb4393cd1903cb614c531f1a4ce97dad6f506b9fd5d2c21`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05708d423c4906488d953a0fe15f13369c66cfd800315207045c3bde3c2e3717`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b2e581ed96cd38f9c3feb006901f524f67d672f3c304950ad03b5ba5d85df4b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33759933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5208ab9badd9219190a61349c33a61c6abb0f0c5a9f85c111d8041b17d14ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 11:01:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 11:02:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:02:13 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 11:02:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 11:02:57 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 11:02:58 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 11:02:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 11:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 11:02:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce433f8fd0317821392c343b5116cf0526b6490a1016133e563f1f6c91d4e11`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef79c479a4e994c1a71e4f53a3aac700f92a97e49a59f81c3651ed3c0e139c7d`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 2.0 MB (2007772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54caab845ffff5ee7f081cc3171aba5afdc35c073e36b4a85e13efcf745fa3f7`  
		Last Modified: Sun, 02 Feb 2020 11:03:22 GMT  
		Size: 5.9 MB (5899289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a866034f98905d2f1e9bc020a0fb9b076b92ae72b9ca92db777e18cb04949235`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe61640aba00e184e4ecf0094118dcac5ff70a4e7210c575880abc0076a66b2`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:9b08de941dfabf18ab82637496dd834891465c7825cf3233a85f978770c48762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18dc26279c852de9a9c175279765969a744c699027eab9660eb2727c85fe124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:33:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 09:33:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 09:34:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 09:34:08 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 09:34:08 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 09:34:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b4b2d4ef7209a4b74a85b2268886f21ac7062f11a659fdb2aa6f0778a168b1`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ba6ade7bf16194e5e43284dac9428686f878f227f7f6f6bf775a5b4ac308b`  
		Last Modified: Sun, 02 Feb 2020 09:34:37 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f581d8f56da9341f96479173d238146066351b343ba87abc58e8c5fb2bad72`  
		Last Modified: Sun, 02 Feb 2020 09:34:43 GMT  
		Size: 11.6 MB (11622885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bff5f4bc56cbd458b29d3af1f8a43c3959a79d96399e9edb29952312da744`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6758530d06a785788fe95501c1e5e54c659274c8b2e68be98bba7be1c8e4e`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:2af640b2e5e945fc7a2bbfbb758f836c601e7de4736cc7a2c153e2b6f2341de1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aacf013b516fb925973edd0d5747ae594d30843d4a6e7b05dc75bee90541d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:59:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 02:59:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:00:00 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 03:00:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 03:00:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 03:01:48 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 03:01:50 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 03:01:54 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 03:01:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:02:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a590754624a36c689aa2f868ae093bd0d238306deee026950720a1cef27c3`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d8bb6be0d52570c63debf54f56ca533bf2dd6c63d7ce8608f252b603f2cd7`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 2.2 MB (2224858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee10f5eebb2434c30ad4544e59ecc613b84e9c385e27ae8e436cae5bb7fd5d2`  
		Last Modified: Sun, 02 Feb 2020 03:02:34 GMT  
		Size: 6.7 MB (6735278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef1fcf1f9bae2a0a129a9e502f40627dd016d7570d2ad986f6701448edf1660`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad008d8b0be1cb3825d2601908169faa054d1f30e0e4168421f0672c24b2079a`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:4847e130e4505884571acd096a951f97c04043453c52945dd80eb985050af833
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33463886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52af50aad2f838fc10ccd8fd81eece8695e0daf0811b92c0ebad98de879ac18a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:21:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 22:21:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 22:21:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 22:21:37 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 22:21:37 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 22:21:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:21:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a991d51344d40c0dc65a4bbb295c13f9702296c25aaac1aef4d81bfc979b089`  
		Last Modified: Sat, 01 Feb 2020 22:21:51 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cde9e08e6e33966ecc6eee8880ae741ea240f38b9b7909c2a568a8e2dae10d`  
		Last Modified: Sat, 01 Feb 2020 22:21:56 GMT  
		Size: 1.8 MB (1821708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7642a6ebcfd2be1e13fc5075d371c0ed03f77d355a77755325555f6eb6ef8eb`  
		Last Modified: Sat, 01 Feb 2020 22:21:52 GMT  
		Size: 5.9 MB (5934595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33c4f7cbed3197ee9911e190eeb6e8fee8ed0d5ae49e1f2223d6bf93a9234e`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65e2452f41b088b369c8d479923a093961365f0f22a5e44f9c93fa2a67552ba`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.0`

```console
$ docker pull spiped@sha256:a9f2d41c15a40c84435c70e5ef8cace5cee29cd1f84babe1ece1c40f4c2db8aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.0` - linux; amd64

```console
$ docker pull spiped@sha256:94a496399350fa792c12e719637ec1b6288c9df7d1d958434b3bf6f1a4cb35a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7b9f24c6da4ff2db786e27df56dffad1979a1a1b3f8d30f090d43ac5026157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:15:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 06:15:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 06:15:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 06:15:40 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 06:15:40 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 06:15:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:15:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:15:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731399cccc6f318fc2161064db19deeaa2fbb915888b6bfb4f788393478b1793`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd449eddd5c8ce7f92d05d131ce66ac8ec39d6d022327729918564f50d41ec7c`  
		Last Modified: Sun, 02 Feb 2020 06:16:01 GMT  
		Size: 2.1 MB (2128004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc4057ac7a766f5ef045ce99563fa24f1a184dd5314c8c2278373e4e910b03`  
		Last Modified: Sun, 02 Feb 2020 06:16:03 GMT  
		Size: 7.0 MB (7027512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a5937d1f11dff98ab8deee7b992099bf6bc7c104bdb75997f4766ee01289e3`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24862150235a45dafb0089ae7493770b72db3c3d54c0fbf02d7d7540907797a9`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v5

```console
$ docker pull spiped@sha256:46c09863fe9de71ed17fe3429d98937b35cca01042ce95a7cfac14a4940e5940
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4854892b43b9226b0bfec04d10d05520d1c3169732ba4d2496373730e06d6c3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:28:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 18:28:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:28:16 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 18:29:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 18:29:04 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 18:29:04 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 18:29:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 18:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 18:29:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd3ed7c8c7f6527fcca82864bf95939d859f70dbd259e58c7b77f2cb9b78fb9`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37608bc89418e7e427b153b07e0f00846c35f85e931ec816c2ec38c9142aaf2a`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.8 MB (1839087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d56a8f81afe86e05571a145096d08791146a0620bdad3a6b7f770d1e46742a`  
		Last Modified: Sat, 01 Feb 2020 18:29:26 GMT  
		Size: 5.5 MB (5472626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9936f33ba62b478e8d90beb45179853a937da89dc8a77ac60274d13f21144963`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774801a174976d8412993bef93bcc4432be10e2db2842e1d568ac473c9317643`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v7

```console
$ docker pull spiped@sha256:740ad6efbf90726477deac506ce4164a29631a5ec5d250e48f524191dd95397e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71504de64d0ace9ede0f5de8448e4aad5e678a8538d54fd2b4586548219ff12f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:27:59 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 08:28:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 08:28:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 08:28:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 08:28:54 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 08:28:55 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 08:28:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:29:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cec23850f77792ec02c51a5c3d02d44ef577be63198b96c3d2d32f2e428abd1`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f287c58e653509527769eab1974b77bc7d6f5f0663686f24f171871a9b4d5`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.8 MB (1759406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012d5ec3a62094c0196d0f0f75875328f73bc5e10282349943f20ac1133a4bf`  
		Last Modified: Sun, 02 Feb 2020 08:29:29 GMT  
		Size: 5.3 MB (5279046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e5223531e65090bb4393cd1903cb614c531f1a4ce97dad6f506b9fd5d2c21`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05708d423c4906488d953a0fe15f13369c66cfd800315207045c3bde3c2e3717`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b2e581ed96cd38f9c3feb006901f524f67d672f3c304950ad03b5ba5d85df4b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33759933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5208ab9badd9219190a61349c33a61c6abb0f0c5a9f85c111d8041b17d14ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 11:01:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 11:02:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:02:13 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 11:02:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 11:02:57 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 11:02:58 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 11:02:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 11:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 11:02:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce433f8fd0317821392c343b5116cf0526b6490a1016133e563f1f6c91d4e11`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef79c479a4e994c1a71e4f53a3aac700f92a97e49a59f81c3651ed3c0e139c7d`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 2.0 MB (2007772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54caab845ffff5ee7f081cc3171aba5afdc35c073e36b4a85e13efcf745fa3f7`  
		Last Modified: Sun, 02 Feb 2020 11:03:22 GMT  
		Size: 5.9 MB (5899289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a866034f98905d2f1e9bc020a0fb9b076b92ae72b9ca92db777e18cb04949235`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe61640aba00e184e4ecf0094118dcac5ff70a4e7210c575880abc0076a66b2`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; 386

```console
$ docker pull spiped@sha256:9b08de941dfabf18ab82637496dd834891465c7825cf3233a85f978770c48762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18dc26279c852de9a9c175279765969a744c699027eab9660eb2727c85fe124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:33:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 09:33:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 09:34:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 09:34:08 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 09:34:08 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 09:34:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b4b2d4ef7209a4b74a85b2268886f21ac7062f11a659fdb2aa6f0778a168b1`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ba6ade7bf16194e5e43284dac9428686f878f227f7f6f6bf775a5b4ac308b`  
		Last Modified: Sun, 02 Feb 2020 09:34:37 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f581d8f56da9341f96479173d238146066351b343ba87abc58e8c5fb2bad72`  
		Last Modified: Sun, 02 Feb 2020 09:34:43 GMT  
		Size: 11.6 MB (11622885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bff5f4bc56cbd458b29d3af1f8a43c3959a79d96399e9edb29952312da744`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6758530d06a785788fe95501c1e5e54c659274c8b2e68be98bba7be1c8e4e`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; ppc64le

```console
$ docker pull spiped@sha256:2af640b2e5e945fc7a2bbfbb758f836c601e7de4736cc7a2c153e2b6f2341de1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aacf013b516fb925973edd0d5747ae594d30843d4a6e7b05dc75bee90541d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:59:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 02:59:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:00:00 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 03:00:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 03:00:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 03:01:48 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 03:01:50 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 03:01:54 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 03:01:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:02:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a590754624a36c689aa2f868ae093bd0d238306deee026950720a1cef27c3`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d8bb6be0d52570c63debf54f56ca533bf2dd6c63d7ce8608f252b603f2cd7`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 2.2 MB (2224858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee10f5eebb2434c30ad4544e59ecc613b84e9c385e27ae8e436cae5bb7fd5d2`  
		Last Modified: Sun, 02 Feb 2020 03:02:34 GMT  
		Size: 6.7 MB (6735278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef1fcf1f9bae2a0a129a9e502f40627dd016d7570d2ad986f6701448edf1660`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad008d8b0be1cb3825d2601908169faa054d1f30e0e4168421f0672c24b2079a`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; s390x

```console
$ docker pull spiped@sha256:4847e130e4505884571acd096a951f97c04043453c52945dd80eb985050af833
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33463886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52af50aad2f838fc10ccd8fd81eece8695e0daf0811b92c0ebad98de879ac18a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:21:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 22:21:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 22:21:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 22:21:37 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 22:21:37 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 22:21:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:21:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a991d51344d40c0dc65a4bbb295c13f9702296c25aaac1aef4d81bfc979b089`  
		Last Modified: Sat, 01 Feb 2020 22:21:51 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cde9e08e6e33966ecc6eee8880ae741ea240f38b9b7909c2a568a8e2dae10d`  
		Last Modified: Sat, 01 Feb 2020 22:21:56 GMT  
		Size: 1.8 MB (1821708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7642a6ebcfd2be1e13fc5075d371c0ed03f77d355a77755325555f6eb6ef8eb`  
		Last Modified: Sat, 01 Feb 2020 22:21:52 GMT  
		Size: 5.9 MB (5934595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33c4f7cbed3197ee9911e190eeb6e8fee8ed0d5ae49e1f2223d6bf93a9234e`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65e2452f41b088b369c8d479923a093961365f0f22a5e44f9c93fa2a67552ba`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.0-alpine`

```console
$ docker pull spiped@sha256:fbd6b5ae2a27e72d9e8e9d4862d3d26b62fd9727ef023270b72cac02182e6b47
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

### `spiped:1.6.0-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:74ca5fed33829dc0f90af3a054ee92071c3c5978874ccbaeb5fd2b1ff9e8092f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5c590bf78e8b20f0b27c7e2d589ba69e2fb9081b56a0c5a256c65b74251c7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 06:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 06:03:17 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 06:03:17 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 06:03:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 06:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 06:03:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af29ea4904a829b1e0b6731429be3308942a6d6d452a724b6ddf604ed92d84c5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 79.4 KB (79416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544ee78713ff37f3c8a4e37c425af1572bce8ddc4d5881df790219f176f1e6f`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c05cb615fdcca16932db64d693056304dbbd298a8711ce6d9fca7a337235b6`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; 386

```console
$ docker pull spiped@sha256:5826ab876f6c3b2638e73f4c90a6dbc2dc0c21c314d21971465b298f7cd8b140
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7feb8ad3bb5db014f9f05326f7d18ca9bca990695ece591fdb1db79214cbfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 04:05:27 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 04:05:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 04:05:38 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 04:05:38 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 04:05:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:05:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edea154bc79691d4ecf2977913fa71d695d8a5121ff218e768988dc1d3085c5`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 87.7 KB (87711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c140bda32e0e1da819208d29f88cde400caa913cc3a23f4e0405eb569c68a30`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54f8f5bcf5bc5ffc81779754f857a47a3f109f440f7a04d4279efc409447d9b`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:fbd6b5ae2a27e72d9e8e9d4862d3d26b62fd9727ef023270b72cac02182e6b47
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
$ docker pull spiped@sha256:74ca5fed33829dc0f90af3a054ee92071c3c5978874ccbaeb5fd2b1ff9e8092f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5c590bf78e8b20f0b27c7e2d589ba69e2fb9081b56a0c5a256c65b74251c7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 06:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 06:03:17 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 06:03:17 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 06:03:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 06:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 06:03:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af29ea4904a829b1e0b6731429be3308942a6d6d452a724b6ddf604ed92d84c5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 79.4 KB (79416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544ee78713ff37f3c8a4e37c425af1572bce8ddc4d5881df790219f176f1e6f`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c05cb615fdcca16932db64d693056304dbbd298a8711ce6d9fca7a337235b6`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:5826ab876f6c3b2638e73f4c90a6dbc2dc0c21c314d21971465b298f7cd8b140
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7feb8ad3bb5db014f9f05326f7d18ca9bca990695ece591fdb1db79214cbfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 04:05:27 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 04:05:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 04:05:38 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 04:05:38 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 04:05:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:05:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edea154bc79691d4ecf2977913fa71d695d8a5121ff218e768988dc1d3085c5`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 87.7 KB (87711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c140bda32e0e1da819208d29f88cde400caa913cc3a23f4e0405eb569c68a30`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54f8f5bcf5bc5ffc81779754f857a47a3f109f440f7a04d4279efc409447d9b`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:fbd6b5ae2a27e72d9e8e9d4862d3d26b62fd9727ef023270b72cac02182e6b47
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
$ docker pull spiped@sha256:74ca5fed33829dc0f90af3a054ee92071c3c5978874ccbaeb5fd2b1ff9e8092f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5c590bf78e8b20f0b27c7e2d589ba69e2fb9081b56a0c5a256c65b74251c7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 06:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 06:03:17 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 06:03:17 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 06:03:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 06:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 06:03:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af29ea4904a829b1e0b6731429be3308942a6d6d452a724b6ddf604ed92d84c5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 79.4 KB (79416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544ee78713ff37f3c8a4e37c425af1572bce8ddc4d5881df790219f176f1e6f`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c05cb615fdcca16932db64d693056304dbbd298a8711ce6d9fca7a337235b6`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:5826ab876f6c3b2638e73f4c90a6dbc2dc0c21c314d21971465b298f7cd8b140
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7feb8ad3bb5db014f9f05326f7d18ca9bca990695ece591fdb1db79214cbfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 04:05:27 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 04:05:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 04:05:38 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 04:05:38 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 04:05:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:05:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edea154bc79691d4ecf2977913fa71d695d8a5121ff218e768988dc1d3085c5`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 87.7 KB (87711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c140bda32e0e1da819208d29f88cde400caa913cc3a23f4e0405eb569c68a30`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54f8f5bcf5bc5ffc81779754f857a47a3f109f440f7a04d4279efc409447d9b`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:fbd6b5ae2a27e72d9e8e9d4862d3d26b62fd9727ef023270b72cac02182e6b47
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
$ docker pull spiped@sha256:74ca5fed33829dc0f90af3a054ee92071c3c5978874ccbaeb5fd2b1ff9e8092f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5c590bf78e8b20f0b27c7e2d589ba69e2fb9081b56a0c5a256c65b74251c7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 06:03:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 06:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 06:03:17 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 06:03:17 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 06:03:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 06:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 06:03:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af29ea4904a829b1e0b6731429be3308942a6d6d452a724b6ddf604ed92d84c5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 79.4 KB (79416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544ee78713ff37f3c8a4e37c425af1572bce8ddc4d5881df790219f176f1e6f`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c05cb615fdcca16932db64d693056304dbbd298a8711ce6d9fca7a337235b6`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3ae91669334784f7b06ff519d1493b018d6b1946da07f9538b9ce403ba6a806c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2647489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66aceefd2fe95659d0e866344c41b8ab59a1f5edea0d9b102bcfb102808402ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 21:07:16 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 21:07:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 21:07:18 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 21:07:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 21:07:40 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 21:07:41 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 21:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:07:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ca77a0d6c23ca1ab7a1d6247b2f6058a74967635d48c6436eddb9c4ab9dc8b`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 68.0 KB (67990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecc30ce77974a56c9958f85075516bf23a4d87f452a99f0994ba66bbdff2b2f`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d253ce677e060437c999efb2094afda12da7234d44582a95187be47777394`  
		Last Modified: Thu, 23 Jan 2020 21:07:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf6bfcf29967c12ef7c3749eefef9078bd45f60bd4c88f76c983108a3d464f42
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 MB (2448253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccadcaa5909aa00e88b17bf5880f652201851d3584c86fff7fcb9fa620424043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:56:51 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:56:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:57:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:57:11 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:57:11 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:57:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b88556cd7e307bd7aae61fbb97a5a495fd194bc5ca395dae82b60e890550492`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 61.7 KB (61746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7e64f07324c2b74ff72e4b59b8a1693e42d453bf3e54a36e830699e3726c1`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39643304907003481036d0a383c8fc76114ab8f7ef02e7ae8513c2c1d30bfb56`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:20b57cf601ee060aeaf921435a00e6a82a6530d41dd56dcd9e39c61ff91f43ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2800460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1480c1b012f4040b28851a83b09229b746c3f91b19b26a23903e7efe854c889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 23:03:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 23:03:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 23:03:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 23:03:43 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 23:03:44 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 23:03:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:03:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:03:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29117a9c36d3c0a533610608811d712072dc8a92ea2d334dbc8fa9c76ef7c9bf`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 74.6 KB (74633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270709957b90da9fa027a60063ec540960b2cd6f61f5bb3c36a4abadc5bf7311`  
		Last Modified: Thu, 23 Jan 2020 23:04:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e244e62f2ba142b8261afd7ec620d1587573e07661176f4a5cd231fddbd819`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:5826ab876f6c3b2638e73f4c90a6dbc2dc0c21c314d21971465b298f7cd8b140
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2881614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7feb8ad3bb5db014f9f05326f7d18ca9bca990695ece591fdb1db79214cbfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Jan 2020 04:05:27 GMT
ENV SPIPED_VERSION=1.6.0
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Fri, 24 Jan 2020 04:05:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Fri, 24 Jan 2020 04:05:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Jan 2020 04:05:38 GMT
VOLUME [/spiped]
# Fri, 24 Jan 2020 04:05:38 GMT
WORKDIR /spiped
# Fri, 24 Jan 2020 04:05:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:05:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edea154bc79691d4ecf2977913fa71d695d8a5121ff218e768988dc1d3085c5`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 87.7 KB (87711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c140bda32e0e1da819208d29f88cde400caa913cc3a23f4e0405eb569c68a30`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54f8f5bcf5bc5ffc81779754f857a47a3f109f440f7a04d4279efc409447d9b`  
		Last Modified: Fri, 24 Jan 2020 04:05:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:45fde12ba87e9485fa2492800f06b5be74389f0cf0479a9e332b6a5a7c39d354
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2905035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc34cf420e2d6d3376211c900f10d023d74c8aa156616f5de04e90a125b4044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 22:49:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 22:49:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 22:49:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 22:49:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 22:49:29 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 22:49:31 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 22:49:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:49:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ca9988558a5eacce7c90cdc4e47bdbb211376da49463c155923430de39d4a`  
		Last Modified: Thu, 23 Jan 2020 22:49:55 GMT  
		Size: 88.4 KB (88392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf498a32c132740eb11d320a6bef7c1930ccbf579ab6215758fc79ea8a84bc4`  
		Last Modified: Thu, 23 Jan 2020 22:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5475460c54abc8555bf4d0cbd75e770a399cd70c60d4e0108a0a7b8290031c17`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:488a2de17ec852acfc64aaa85eda6f96d871735c6d4e81b7c623a708823f1618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0a04dece66804c096550d7b0f2d118b9fc71ba20a8286b2e2b01c10cc9d53b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_VERSION=1.6.0
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Thu, 23 Jan 2020 17:10:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Thu, 23 Jan 2020 17:10:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Jan 2020 17:10:07 GMT
VOLUME [/spiped]
# Thu, 23 Jan 2020 17:10:07 GMT
WORKDIR /spiped
# Thu, 23 Jan 2020 17:10:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bb1f437036a8001e843fa5970d110834f88eab3f52e0117394eb55dfd5717`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad352e7500492b9a55f564319ec4901c35391305ea2d03122f0b2b4d6e53c97`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6ef0b43b14cc42f0b136a8abbef558d32eb7b3e367fd97369ec774dc82090`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:a9f2d41c15a40c84435c70e5ef8cace5cee29cd1f84babe1ece1c40f4c2db8aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:94a496399350fa792c12e719637ec1b6288c9df7d1d958434b3bf6f1a4cb35a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7b9f24c6da4ff2db786e27df56dffad1979a1a1b3f8d30f090d43ac5026157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:15:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 06:15:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 06:15:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 06:15:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 06:15:40 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 06:15:40 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 06:15:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:15:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:15:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731399cccc6f318fc2161064db19deeaa2fbb915888b6bfb4f788393478b1793`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd449eddd5c8ce7f92d05d131ce66ac8ec39d6d022327729918564f50d41ec7c`  
		Last Modified: Sun, 02 Feb 2020 06:16:01 GMT  
		Size: 2.1 MB (2128004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc4057ac7a766f5ef045ce99563fa24f1a184dd5314c8c2278373e4e910b03`  
		Last Modified: Sun, 02 Feb 2020 06:16:03 GMT  
		Size: 7.0 MB (7027512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a5937d1f11dff98ab8deee7b992099bf6bc7c104bdb75997f4766ee01289e3`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24862150235a45dafb0089ae7493770b72db3c3d54c0fbf02d7d7540907797a9`  
		Last Modified: Sun, 02 Feb 2020 06:16:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:46c09863fe9de71ed17fe3429d98937b35cca01042ce95a7cfac14a4940e5940
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32143594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4854892b43b9226b0bfec04d10d05520d1c3169732ba4d2496373730e06d6c3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:28:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 18:28:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:28:16 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 18:28:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 18:29:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 18:29:04 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 18:29:04 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 18:29:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 18:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 18:29:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd3ed7c8c7f6527fcca82864bf95939d859f70dbd259e58c7b77f2cb9b78fb9`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37608bc89418e7e427b153b07e0f00846c35f85e931ec816c2ec38c9142aaf2a`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 1.8 MB (1839087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d56a8f81afe86e05571a145096d08791146a0620bdad3a6b7f770d1e46742a`  
		Last Modified: Sat, 01 Feb 2020 18:29:26 GMT  
		Size: 5.5 MB (5472626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9936f33ba62b478e8d90beb45179853a937da89dc8a77ac60274d13f21144963`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774801a174976d8412993bef93bcc4432be10e2db2842e1d568ac473c9317643`  
		Last Modified: Sat, 01 Feb 2020 18:29:24 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:740ad6efbf90726477deac506ce4164a29631a5ec5d250e48f524191dd95397e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29739793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71504de64d0ace9ede0f5de8448e4aad5e678a8538d54fd2b4586548219ff12f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:27:59 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 08:28:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 08:28:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 08:28:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 08:28:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 08:28:54 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 08:28:55 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 08:28:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:29:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cec23850f77792ec02c51a5c3d02d44ef577be63198b96c3d2d32f2e428abd1`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f287c58e653509527769eab1974b77bc7d6f5f0663686f24f171871a9b4d5`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 1.8 MB (1759406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012d5ec3a62094c0196d0f0f75875328f73bc5e10282349943f20ac1133a4bf`  
		Last Modified: Sun, 02 Feb 2020 08:29:29 GMT  
		Size: 5.3 MB (5279046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e5223531e65090bb4393cd1903cb614c531f1a4ce97dad6f506b9fd5d2c21`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05708d423c4906488d953a0fe15f13369c66cfd800315207045c3bde3c2e3717`  
		Last Modified: Sun, 02 Feb 2020 08:29:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b2e581ed96cd38f9c3feb006901f524f67d672f3c304950ad03b5ba5d85df4b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33759933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5208ab9badd9219190a61349c33a61c6abb0f0c5a9f85c111d8041b17d14ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 11:01:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 11:02:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:02:13 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 11:02:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 11:02:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 11:02:57 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 11:02:58 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 11:02:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 11:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 11:02:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce433f8fd0317821392c343b5116cf0526b6490a1016133e563f1f6c91d4e11`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef79c479a4e994c1a71e4f53a3aac700f92a97e49a59f81c3651ed3c0e139c7d`  
		Last Modified: Sun, 02 Feb 2020 11:03:20 GMT  
		Size: 2.0 MB (2007772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54caab845ffff5ee7f081cc3171aba5afdc35c073e36b4a85e13efcf745fa3f7`  
		Last Modified: Sun, 02 Feb 2020 11:03:22 GMT  
		Size: 5.9 MB (5899289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a866034f98905d2f1e9bc020a0fb9b076b92ae72b9ca92db777e18cb04949235`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe61640aba00e184e4ecf0094118dcac5ff70a4e7210c575880abc0076a66b2`  
		Last Modified: Sun, 02 Feb 2020 11:03:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:9b08de941dfabf18ab82637496dd834891465c7825cf3233a85f978770c48762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41504427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18dc26279c852de9a9c175279765969a744c699027eab9660eb2727c85fe124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:33:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 09:33:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 09:33:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 09:34:08 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 09:34:08 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 09:34:08 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 09:34:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b4b2d4ef7209a4b74a85b2268886f21ac7062f11a659fdb2aa6f0778a168b1`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ba6ade7bf16194e5e43284dac9428686f878f227f7f6f6bf775a5b4ac308b`  
		Last Modified: Sun, 02 Feb 2020 09:34:37 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f581d8f56da9341f96479173d238146066351b343ba87abc58e8c5fb2bad72`  
		Last Modified: Sun, 02 Feb 2020 09:34:43 GMT  
		Size: 11.6 MB (11622885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bff5f4bc56cbd458b29d3af1f8a43c3959a79d96399e9edb29952312da744`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd6758530d06a785788fe95501c1e5e54c659274c8b2e68be98bba7be1c8e4e`  
		Last Modified: Sun, 02 Feb 2020 09:34:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:2af640b2e5e945fc7a2bbfbb758f836c601e7de4736cc7a2c153e2b6f2341de1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aacf013b516fb925973edd0d5747ae594d30843d4a6e7b05dc75bee90541d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:59:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 02 Feb 2020 02:59:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:00:00 GMT
ENV SPIPED_VERSION=1.6.0
# Sun, 02 Feb 2020 03:00:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sun, 02 Feb 2020 03:00:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sun, 02 Feb 2020 03:01:48 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 02 Feb 2020 03:01:50 GMT
VOLUME [/spiped]
# Sun, 02 Feb 2020 03:01:54 GMT
WORKDIR /spiped
# Sun, 02 Feb 2020 03:01:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:02:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a590754624a36c689aa2f868ae093bd0d238306deee026950720a1cef27c3`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d8bb6be0d52570c63debf54f56ca533bf2dd6c63d7ce8608f252b603f2cd7`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 2.2 MB (2224858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee10f5eebb2434c30ad4544e59ecc613b84e9c385e27ae8e436cae5bb7fd5d2`  
		Last Modified: Sun, 02 Feb 2020 03:02:34 GMT  
		Size: 6.7 MB (6735278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef1fcf1f9bae2a0a129a9e502f40627dd016d7570d2ad986f6701448edf1660`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad008d8b0be1cb3825d2601908169faa054d1f30e0e4168421f0672c24b2079a`  
		Last Modified: Sun, 02 Feb 2020 03:02:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:4847e130e4505884571acd096a951f97c04043453c52945dd80eb985050af833
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33463886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52af50aad2f838fc10ccd8fd81eece8695e0daf0811b92c0ebad98de879ac18a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:21:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 01 Feb 2020 22:21:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_VERSION=1.6.0
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Sat, 01 Feb 2020 22:21:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Sat, 01 Feb 2020 22:21:36 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 01 Feb 2020 22:21:37 GMT
VOLUME [/spiped]
# Sat, 01 Feb 2020 22:21:37 GMT
WORKDIR /spiped
# Sat, 01 Feb 2020 22:21:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:21:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a991d51344d40c0dc65a4bbb295c13f9702296c25aaac1aef4d81bfc979b089`  
		Last Modified: Sat, 01 Feb 2020 22:21:51 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cde9e08e6e33966ecc6eee8880ae741ea240f38b9b7909c2a568a8e2dae10d`  
		Last Modified: Sat, 01 Feb 2020 22:21:56 GMT  
		Size: 1.8 MB (1821708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7642a6ebcfd2be1e13fc5075d371c0ed03f77d355a77755325555f6eb6ef8eb`  
		Last Modified: Sat, 01 Feb 2020 22:21:52 GMT  
		Size: 5.9 MB (5934595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33c4f7cbed3197ee9911e190eeb6e8fee8ed0d5ae49e1f2223d6bf93a9234e`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65e2452f41b088b369c8d479923a093961365f0f22a5e44f9c93fa2a67552ba`  
		Last Modified: Sat, 01 Feb 2020 22:22:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
