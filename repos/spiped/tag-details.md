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
$ docker pull spiped@sha256:3341f15907098e665e1e39a7fe67f8a08947d2a6a40f924585d5c703c7fd14e2
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
$ docker pull spiped@sha256:0c5fe169a548e2a94c540daf066dbd032630b7252660e0ecd7a7262621e84385
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59eca6f5480483b64dc79563f580834fc43fd1887ff36dca5293233839976352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:00:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 20:00:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 20:00:52 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 20:01:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 20:01:16 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 20:01:16 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 20:01:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 20:01:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:01:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390f34b79a1b94734def418ee1b77fa9f7e6b7864855301532b9938626c9579`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dab183e4d1aa7de59d6d3b044a3412243ecdadce47a2d96702f226af571217e`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 2.1 MB (2128057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7b31afb54f1cbc65e88e9084ce4e02db14bf6d253402e06872a303226dba77`  
		Last Modified: Wed, 26 Feb 2020 20:01:34 GMT  
		Size: 7.0 MB (7027538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f78340f290fcca0baf3e68dfa19d4040916e4987d74f8ea82a104ab0041d1b4`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26f710af9b85fb63be8dafb87182315392e08f33fc5f6029b475d676f80821`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:22708db4700044cc40629ef3d0132e65dc2a2c53ed30f557efdc2cde9d64a1d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32144294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153da17b7fb4a2df0866fcdb1658cb7310fccb97b65d6afee4e475a9c97b5c57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:30:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 04:30:30 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:30:30 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 04:30:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 04:30:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 04:31:33 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:31:42 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 04:31:44 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 04:31:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 04:31:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefbeddbda1bfbf1616744f38dc348943f324298d333f2b8c3558de8c9dc291`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2a0c75baa019bd5f2dd0846f446ae2c8bffec87698e82c25761aaf1cab5065`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.8 MB (1839104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5e08934b22040a5e598053f114c4364a441b0136ce740a3da39eb12d232ee`  
		Last Modified: Wed, 26 Feb 2020 04:32:09 GMT  
		Size: 5.5 MB (5472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fd5e13a49f16075834f990bec89ef5149e903af14c273a5af00db8ba1e4f7`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4550cfd82a5ee7240c85d580844209baccd056556ea3d30f2b7a803b375e00`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff8cdc2b76900c360fa78853a876c90cb60d40d6189721fd6440edbf98330e42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29740440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8f7d469ee7781d6741f036c6acdd382069be46a6bc0afbf965c7cb7240f873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 16:48:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 16:48:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:48:19 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 16:49:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 16:49:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 16:49:08 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 16:49:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:49:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff6a24a4fc649e54087f81871f0340c182dd5621e999612c894eddb1c23a2c6`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbcdd6271480b6052202176b3913a02e5aa2138403a2f4bf71bbb1942da17b3`  
		Last Modified: Wed, 26 Feb 2020 16:49:42 GMT  
		Size: 1.8 MB (1759383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740086b1bbe66205067ea279aa978c67880cf17811231656bc4fa01e5cec4565`  
		Last Modified: Wed, 26 Feb 2020 16:49:41 GMT  
		Size: 5.3 MB (5279075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cda810dd77a9db5ece3c96e17409ed7e7ac9d5d7ba7170be96239f1f9d25f`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873ee402dec91c7c8ad69dc2255a42ea15bf4d5685ff78e4843fda8b2a878aa`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:2045b20695df4a308887c27517b0322dd4346c917d64930ec7f475e6f42d6f70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23127b7b4048f79d0712142146ca1dac13e6f7e1447d989e8a9cac7bddee77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:26:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:26:13 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:26:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:26:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:26:57 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:26:58 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:26:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed69a865d08c299737373cdce47c8965793574b9ff0824aa64e10a6408a7a0f`  
		Last Modified: Wed, 26 Feb 2020 19:27:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7408f6432832bddbcc6a873062a16487fc77b8f81a0f0712a4a4d6e29d75926a`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 2.0 MB (2007825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b1c317b65863d53f82438d704518c869b157df900bc12823e0a26b3fc4c8f1`  
		Last Modified: Wed, 26 Feb 2020 19:27:18 GMT  
		Size: 5.9 MB (5899308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50411db9d236c261110100ce6f72493081c4d72e48b958be9025fd916278f1e2`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abcf881ec0ba905d35a64d37f591c9ee61d3c11d3b2850a9fbad546ef19afbf`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:2b3380572c777d30dc3c1df78ff3a532c31cf10d6697aa4cac4069356a0f16e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41505089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c3dbcd632dae8470e3fe9fd164ecaeb12f36ba4cef2d4882abbc9dca244068`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:33:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:33:40 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:33:41 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:34:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:34:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:34:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:34:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:34:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb39e2ebabb52d3a53b8f185dca6c0e86afd917f11cb005127fe42561332d67`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85219efcddbf6309ac25fa211217a0f409881166202a000741c82768e2398cc`  
		Last Modified: Wed, 26 Feb 2020 19:34:21 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a3242d878be2ea033f61cbfc1a7351d69cea664592603153633e6813a9b6f`  
		Last Modified: Wed, 26 Feb 2020 19:34:24 GMT  
		Size: 11.6 MB (11622908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee2e72356c1d3434c64075b0556588135d7214ba648211d57a1f9f67f6b967`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb8de6b637810b5100f73918b939d02e09fa36ae9336dc958ee09a16edb9bc`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c06423344c44b3d742686d3edd389a568a92e2fb50a8b8179a8a1ee69b3545
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010a4f97446ecf9df1cbf1bf0a27f73134a0e869fc8f9624d8b2a23d841f97ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 18:53:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:53:07 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 18:53:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 18:53:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 18:55:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 18:55:04 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 18:55:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 18:55:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:55:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 18:55:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfea20849fee248f74330af12c22433e92bbe7dab537da421edfcd2976601b87`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55407c0d0f18ea49b6657b3d13c844d211899153471b22d30c8a64da45c06794`  
		Last Modified: Wed, 26 Feb 2020 18:55:43 GMT  
		Size: 2.2 MB (2224830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2cea050271247b818081b57713dd5e687ca4752e2bc388597a214d4630fae3`  
		Last Modified: Wed, 26 Feb 2020 18:55:45 GMT  
		Size: 6.7 MB (6735303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa1eba0c0a3d25e79b17cc91014d8eba1f0221e9fe7066067eb5ead76bac08`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c9df31c76a744e37e149d31030486db709ea343608986846673f39e0a9fd15`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:6604a0c90cd36f63713c308d600d37c708070dff8f90483a62623ac468ceac99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33464540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f514f63bc05482a60a7e0f89dd05f9e95e69e655ae00ecadff4d5ffd2d5cd50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:48 GMT
ADD file:3396670211650b5d7c6e1f0ace1a72f1d1587f275baa682dfee6c7bf2603fb34 in / 
# Wed, 26 Feb 2020 00:42:50 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:58:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 07:58:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 07:59:18 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 07:59:18 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 07:59:19 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 07:59:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 07:59:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 07:59:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e25900e2a7f96a6326b79ec6dfdce1ac5461c7a961fb3752ec1770cd82b8d03c`  
		Last Modified: Wed, 26 Feb 2020 00:47:43 GMT  
		Size: 25.7 MB (25705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea8b61886f4f699c7f3022c2f79fd9edc5b87455b0400e1902ee2cff240003b`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813fd202d108b03f9751b80d328c05ba0a27826f140966910a13ab0d49ceda4c`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 1.8 MB (1821723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2133c8ba6ea7a2d5bb99b4dd9fedf11fd8c9aeef7c98d8981e0e81c425d40`  
		Last Modified: Wed, 26 Feb 2020 07:59:48 GMT  
		Size: 5.9 MB (5934684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25072a908f4a3ead826aa20e08dc8376f6c5e591c181f743943c5b4a7937bcd8`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40daa77c740c41873bcbf019def7b4c0f3fe41d390260d1e23be1d8a1ffb11b7`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:3341f15907098e665e1e39a7fe67f8a08947d2a6a40f924585d5c703c7fd14e2
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
$ docker pull spiped@sha256:0c5fe169a548e2a94c540daf066dbd032630b7252660e0ecd7a7262621e84385
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59eca6f5480483b64dc79563f580834fc43fd1887ff36dca5293233839976352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:00:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 20:00:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 20:00:52 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 20:01:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 20:01:16 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 20:01:16 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 20:01:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 20:01:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:01:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390f34b79a1b94734def418ee1b77fa9f7e6b7864855301532b9938626c9579`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dab183e4d1aa7de59d6d3b044a3412243ecdadce47a2d96702f226af571217e`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 2.1 MB (2128057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7b31afb54f1cbc65e88e9084ce4e02db14bf6d253402e06872a303226dba77`  
		Last Modified: Wed, 26 Feb 2020 20:01:34 GMT  
		Size: 7.0 MB (7027538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f78340f290fcca0baf3e68dfa19d4040916e4987d74f8ea82a104ab0041d1b4`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26f710af9b85fb63be8dafb87182315392e08f33fc5f6029b475d676f80821`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:22708db4700044cc40629ef3d0132e65dc2a2c53ed30f557efdc2cde9d64a1d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32144294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153da17b7fb4a2df0866fcdb1658cb7310fccb97b65d6afee4e475a9c97b5c57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:30:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 04:30:30 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:30:30 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 04:30:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 04:30:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 04:31:33 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:31:42 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 04:31:44 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 04:31:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 04:31:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefbeddbda1bfbf1616744f38dc348943f324298d333f2b8c3558de8c9dc291`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2a0c75baa019bd5f2dd0846f446ae2c8bffec87698e82c25761aaf1cab5065`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.8 MB (1839104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5e08934b22040a5e598053f114c4364a441b0136ce740a3da39eb12d232ee`  
		Last Modified: Wed, 26 Feb 2020 04:32:09 GMT  
		Size: 5.5 MB (5472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fd5e13a49f16075834f990bec89ef5149e903af14c273a5af00db8ba1e4f7`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4550cfd82a5ee7240c85d580844209baccd056556ea3d30f2b7a803b375e00`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff8cdc2b76900c360fa78853a876c90cb60d40d6189721fd6440edbf98330e42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29740440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8f7d469ee7781d6741f036c6acdd382069be46a6bc0afbf965c7cb7240f873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 16:48:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 16:48:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:48:19 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 16:49:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 16:49:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 16:49:08 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 16:49:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:49:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff6a24a4fc649e54087f81871f0340c182dd5621e999612c894eddb1c23a2c6`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbcdd6271480b6052202176b3913a02e5aa2138403a2f4bf71bbb1942da17b3`  
		Last Modified: Wed, 26 Feb 2020 16:49:42 GMT  
		Size: 1.8 MB (1759383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740086b1bbe66205067ea279aa978c67880cf17811231656bc4fa01e5cec4565`  
		Last Modified: Wed, 26 Feb 2020 16:49:41 GMT  
		Size: 5.3 MB (5279075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cda810dd77a9db5ece3c96e17409ed7e7ac9d5d7ba7170be96239f1f9d25f`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873ee402dec91c7c8ad69dc2255a42ea15bf4d5685ff78e4843fda8b2a878aa`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:2045b20695df4a308887c27517b0322dd4346c917d64930ec7f475e6f42d6f70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23127b7b4048f79d0712142146ca1dac13e6f7e1447d989e8a9cac7bddee77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:26:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:26:13 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:26:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:26:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:26:57 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:26:58 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:26:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed69a865d08c299737373cdce47c8965793574b9ff0824aa64e10a6408a7a0f`  
		Last Modified: Wed, 26 Feb 2020 19:27:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7408f6432832bddbcc6a873062a16487fc77b8f81a0f0712a4a4d6e29d75926a`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 2.0 MB (2007825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b1c317b65863d53f82438d704518c869b157df900bc12823e0a26b3fc4c8f1`  
		Last Modified: Wed, 26 Feb 2020 19:27:18 GMT  
		Size: 5.9 MB (5899308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50411db9d236c261110100ce6f72493081c4d72e48b958be9025fd916278f1e2`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abcf881ec0ba905d35a64d37f591c9ee61d3c11d3b2850a9fbad546ef19afbf`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:2b3380572c777d30dc3c1df78ff3a532c31cf10d6697aa4cac4069356a0f16e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41505089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c3dbcd632dae8470e3fe9fd164ecaeb12f36ba4cef2d4882abbc9dca244068`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:33:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:33:40 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:33:41 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:34:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:34:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:34:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:34:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:34:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb39e2ebabb52d3a53b8f185dca6c0e86afd917f11cb005127fe42561332d67`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85219efcddbf6309ac25fa211217a0f409881166202a000741c82768e2398cc`  
		Last Modified: Wed, 26 Feb 2020 19:34:21 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a3242d878be2ea033f61cbfc1a7351d69cea664592603153633e6813a9b6f`  
		Last Modified: Wed, 26 Feb 2020 19:34:24 GMT  
		Size: 11.6 MB (11622908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee2e72356c1d3434c64075b0556588135d7214ba648211d57a1f9f67f6b967`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb8de6b637810b5100f73918b939d02e09fa36ae9336dc958ee09a16edb9bc`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c06423344c44b3d742686d3edd389a568a92e2fb50a8b8179a8a1ee69b3545
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010a4f97446ecf9df1cbf1bf0a27f73134a0e869fc8f9624d8b2a23d841f97ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 18:53:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:53:07 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 18:53:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 18:53:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 18:55:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 18:55:04 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 18:55:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 18:55:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:55:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 18:55:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfea20849fee248f74330af12c22433e92bbe7dab537da421edfcd2976601b87`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55407c0d0f18ea49b6657b3d13c844d211899153471b22d30c8a64da45c06794`  
		Last Modified: Wed, 26 Feb 2020 18:55:43 GMT  
		Size: 2.2 MB (2224830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2cea050271247b818081b57713dd5e687ca4752e2bc388597a214d4630fae3`  
		Last Modified: Wed, 26 Feb 2020 18:55:45 GMT  
		Size: 6.7 MB (6735303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa1eba0c0a3d25e79b17cc91014d8eba1f0221e9fe7066067eb5ead76bac08`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c9df31c76a744e37e149d31030486db709ea343608986846673f39e0a9fd15`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:6604a0c90cd36f63713c308d600d37c708070dff8f90483a62623ac468ceac99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33464540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f514f63bc05482a60a7e0f89dd05f9e95e69e655ae00ecadff4d5ffd2d5cd50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:48 GMT
ADD file:3396670211650b5d7c6e1f0ace1a72f1d1587f275baa682dfee6c7bf2603fb34 in / 
# Wed, 26 Feb 2020 00:42:50 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:58:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 07:58:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 07:59:18 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 07:59:18 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 07:59:19 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 07:59:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 07:59:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 07:59:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e25900e2a7f96a6326b79ec6dfdce1ac5461c7a961fb3752ec1770cd82b8d03c`  
		Last Modified: Wed, 26 Feb 2020 00:47:43 GMT  
		Size: 25.7 MB (25705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea8b61886f4f699c7f3022c2f79fd9edc5b87455b0400e1902ee2cff240003b`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813fd202d108b03f9751b80d328c05ba0a27826f140966910a13ab0d49ceda4c`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 1.8 MB (1821723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2133c8ba6ea7a2d5bb99b4dd9fedf11fd8c9aeef7c98d8981e0e81c425d40`  
		Last Modified: Wed, 26 Feb 2020 07:59:48 GMT  
		Size: 5.9 MB (5934684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25072a908f4a3ead826aa20e08dc8376f6c5e591c181f743943c5b4a7937bcd8`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40daa77c740c41873bcbf019def7b4c0f3fe41d390260d1e23be1d8a1ffb11b7`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.0`

```console
$ docker pull spiped@sha256:3341f15907098e665e1e39a7fe67f8a08947d2a6a40f924585d5c703c7fd14e2
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
$ docker pull spiped@sha256:0c5fe169a548e2a94c540daf066dbd032630b7252660e0ecd7a7262621e84385
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59eca6f5480483b64dc79563f580834fc43fd1887ff36dca5293233839976352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:00:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 20:00:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 20:00:52 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 20:01:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 20:01:16 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 20:01:16 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 20:01:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 20:01:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:01:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390f34b79a1b94734def418ee1b77fa9f7e6b7864855301532b9938626c9579`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dab183e4d1aa7de59d6d3b044a3412243ecdadce47a2d96702f226af571217e`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 2.1 MB (2128057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7b31afb54f1cbc65e88e9084ce4e02db14bf6d253402e06872a303226dba77`  
		Last Modified: Wed, 26 Feb 2020 20:01:34 GMT  
		Size: 7.0 MB (7027538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f78340f290fcca0baf3e68dfa19d4040916e4987d74f8ea82a104ab0041d1b4`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26f710af9b85fb63be8dafb87182315392e08f33fc5f6029b475d676f80821`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v5

```console
$ docker pull spiped@sha256:22708db4700044cc40629ef3d0132e65dc2a2c53ed30f557efdc2cde9d64a1d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32144294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153da17b7fb4a2df0866fcdb1658cb7310fccb97b65d6afee4e475a9c97b5c57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:30:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 04:30:30 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:30:30 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 04:30:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 04:30:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 04:31:33 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:31:42 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 04:31:44 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 04:31:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 04:31:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefbeddbda1bfbf1616744f38dc348943f324298d333f2b8c3558de8c9dc291`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2a0c75baa019bd5f2dd0846f446ae2c8bffec87698e82c25761aaf1cab5065`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.8 MB (1839104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5e08934b22040a5e598053f114c4364a441b0136ce740a3da39eb12d232ee`  
		Last Modified: Wed, 26 Feb 2020 04:32:09 GMT  
		Size: 5.5 MB (5472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fd5e13a49f16075834f990bec89ef5149e903af14c273a5af00db8ba1e4f7`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4550cfd82a5ee7240c85d580844209baccd056556ea3d30f2b7a803b375e00`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff8cdc2b76900c360fa78853a876c90cb60d40d6189721fd6440edbf98330e42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29740440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8f7d469ee7781d6741f036c6acdd382069be46a6bc0afbf965c7cb7240f873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 16:48:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 16:48:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:48:19 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 16:49:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 16:49:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 16:49:08 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 16:49:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:49:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff6a24a4fc649e54087f81871f0340c182dd5621e999612c894eddb1c23a2c6`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbcdd6271480b6052202176b3913a02e5aa2138403a2f4bf71bbb1942da17b3`  
		Last Modified: Wed, 26 Feb 2020 16:49:42 GMT  
		Size: 1.8 MB (1759383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740086b1bbe66205067ea279aa978c67880cf17811231656bc4fa01e5cec4565`  
		Last Modified: Wed, 26 Feb 2020 16:49:41 GMT  
		Size: 5.3 MB (5279075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cda810dd77a9db5ece3c96e17409ed7e7ac9d5d7ba7170be96239f1f9d25f`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873ee402dec91c7c8ad69dc2255a42ea15bf4d5685ff78e4843fda8b2a878aa`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:2045b20695df4a308887c27517b0322dd4346c917d64930ec7f475e6f42d6f70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23127b7b4048f79d0712142146ca1dac13e6f7e1447d989e8a9cac7bddee77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:26:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:26:13 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:26:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:26:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:26:57 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:26:58 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:26:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed69a865d08c299737373cdce47c8965793574b9ff0824aa64e10a6408a7a0f`  
		Last Modified: Wed, 26 Feb 2020 19:27:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7408f6432832bddbcc6a873062a16487fc77b8f81a0f0712a4a4d6e29d75926a`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 2.0 MB (2007825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b1c317b65863d53f82438d704518c869b157df900bc12823e0a26b3fc4c8f1`  
		Last Modified: Wed, 26 Feb 2020 19:27:18 GMT  
		Size: 5.9 MB (5899308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50411db9d236c261110100ce6f72493081c4d72e48b958be9025fd916278f1e2`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abcf881ec0ba905d35a64d37f591c9ee61d3c11d3b2850a9fbad546ef19afbf`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; 386

```console
$ docker pull spiped@sha256:2b3380572c777d30dc3c1df78ff3a532c31cf10d6697aa4cac4069356a0f16e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41505089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c3dbcd632dae8470e3fe9fd164ecaeb12f36ba4cef2d4882abbc9dca244068`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:33:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:33:40 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:33:41 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:34:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:34:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:34:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:34:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:34:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb39e2ebabb52d3a53b8f185dca6c0e86afd917f11cb005127fe42561332d67`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85219efcddbf6309ac25fa211217a0f409881166202a000741c82768e2398cc`  
		Last Modified: Wed, 26 Feb 2020 19:34:21 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a3242d878be2ea033f61cbfc1a7351d69cea664592603153633e6813a9b6f`  
		Last Modified: Wed, 26 Feb 2020 19:34:24 GMT  
		Size: 11.6 MB (11622908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee2e72356c1d3434c64075b0556588135d7214ba648211d57a1f9f67f6b967`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb8de6b637810b5100f73918b939d02e09fa36ae9336dc958ee09a16edb9bc`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c06423344c44b3d742686d3edd389a568a92e2fb50a8b8179a8a1ee69b3545
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010a4f97446ecf9df1cbf1bf0a27f73134a0e869fc8f9624d8b2a23d841f97ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 18:53:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:53:07 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 18:53:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 18:53:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 18:55:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 18:55:04 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 18:55:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 18:55:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:55:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 18:55:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfea20849fee248f74330af12c22433e92bbe7dab537da421edfcd2976601b87`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55407c0d0f18ea49b6657b3d13c844d211899153471b22d30c8a64da45c06794`  
		Last Modified: Wed, 26 Feb 2020 18:55:43 GMT  
		Size: 2.2 MB (2224830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2cea050271247b818081b57713dd5e687ca4752e2bc388597a214d4630fae3`  
		Last Modified: Wed, 26 Feb 2020 18:55:45 GMT  
		Size: 6.7 MB (6735303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa1eba0c0a3d25e79b17cc91014d8eba1f0221e9fe7066067eb5ead76bac08`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c9df31c76a744e37e149d31030486db709ea343608986846673f39e0a9fd15`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.0` - linux; s390x

```console
$ docker pull spiped@sha256:6604a0c90cd36f63713c308d600d37c708070dff8f90483a62623ac468ceac99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33464540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f514f63bc05482a60a7e0f89dd05f9e95e69e655ae00ecadff4d5ffd2d5cd50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:48 GMT
ADD file:3396670211650b5d7c6e1f0ace1a72f1d1587f275baa682dfee6c7bf2603fb34 in / 
# Wed, 26 Feb 2020 00:42:50 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:58:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 07:58:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 07:59:18 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 07:59:18 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 07:59:19 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 07:59:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 07:59:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 07:59:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e25900e2a7f96a6326b79ec6dfdce1ac5461c7a961fb3752ec1770cd82b8d03c`  
		Last Modified: Wed, 26 Feb 2020 00:47:43 GMT  
		Size: 25.7 MB (25705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea8b61886f4f699c7f3022c2f79fd9edc5b87455b0400e1902ee2cff240003b`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813fd202d108b03f9751b80d328c05ba0a27826f140966910a13ab0d49ceda4c`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 1.8 MB (1821723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2133c8ba6ea7a2d5bb99b4dd9fedf11fd8c9aeef7c98d8981e0e81c425d40`  
		Last Modified: Wed, 26 Feb 2020 07:59:48 GMT  
		Size: 5.9 MB (5934684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25072a908f4a3ead826aa20e08dc8376f6c5e591c181f743943c5b4a7937bcd8`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40daa77c740c41873bcbf019def7b4c0f3fe41d390260d1e23be1d8a1ffb11b7`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:3341f15907098e665e1e39a7fe67f8a08947d2a6a40f924585d5c703c7fd14e2
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
$ docker pull spiped@sha256:0c5fe169a548e2a94c540daf066dbd032630b7252660e0ecd7a7262621e84385
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59eca6f5480483b64dc79563f580834fc43fd1887ff36dca5293233839976352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:00:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 20:00:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 20:00:52 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 20:00:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 20:01:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 20:01:16 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 20:01:16 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 20:01:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 20:01:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:01:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390f34b79a1b94734def418ee1b77fa9f7e6b7864855301532b9938626c9579`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dab183e4d1aa7de59d6d3b044a3412243ecdadce47a2d96702f226af571217e`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 2.1 MB (2128057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7b31afb54f1cbc65e88e9084ce4e02db14bf6d253402e06872a303226dba77`  
		Last Modified: Wed, 26 Feb 2020 20:01:34 GMT  
		Size: 7.0 MB (7027538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f78340f290fcca0baf3e68dfa19d4040916e4987d74f8ea82a104ab0041d1b4`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26f710af9b85fb63be8dafb87182315392e08f33fc5f6029b475d676f80821`  
		Last Modified: Wed, 26 Feb 2020 20:01:33 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:22708db4700044cc40629ef3d0132e65dc2a2c53ed30f557efdc2cde9d64a1d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32144294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153da17b7fb4a2df0866fcdb1658cb7310fccb97b65d6afee4e475a9c97b5c57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:30:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 04:30:30 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:30:30 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 04:30:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 04:30:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 04:31:33 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:31:42 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 04:31:44 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 04:31:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 04:31:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefbeddbda1bfbf1616744f38dc348943f324298d333f2b8c3558de8c9dc291`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2a0c75baa019bd5f2dd0846f446ae2c8bffec87698e82c25761aaf1cab5065`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 1.8 MB (1839104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af5e08934b22040a5e598053f114c4364a441b0136ce740a3da39eb12d232ee`  
		Last Modified: Wed, 26 Feb 2020 04:32:09 GMT  
		Size: 5.5 MB (5472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fd5e13a49f16075834f990bec89ef5149e903af14c273a5af00db8ba1e4f7`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4550cfd82a5ee7240c85d580844209baccd056556ea3d30f2b7a803b375e00`  
		Last Modified: Wed, 26 Feb 2020 04:32:06 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff8cdc2b76900c360fa78853a876c90cb60d40d6189721fd6440edbf98330e42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29740440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8f7d469ee7781d6741f036c6acdd382069be46a6bc0afbf965c7cb7240f873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 16:48:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 16:48:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:48:19 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 16:48:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 16:49:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 16:49:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 16:49:08 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 16:49:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:49:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff6a24a4fc649e54087f81871f0340c182dd5621e999612c894eddb1c23a2c6`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbcdd6271480b6052202176b3913a02e5aa2138403a2f4bf71bbb1942da17b3`  
		Last Modified: Wed, 26 Feb 2020 16:49:42 GMT  
		Size: 1.8 MB (1759383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740086b1bbe66205067ea279aa978c67880cf17811231656bc4fa01e5cec4565`  
		Last Modified: Wed, 26 Feb 2020 16:49:41 GMT  
		Size: 5.3 MB (5279075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cda810dd77a9db5ece3c96e17409ed7e7ac9d5d7ba7170be96239f1f9d25f`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873ee402dec91c7c8ad69dc2255a42ea15bf4d5685ff78e4843fda8b2a878aa`  
		Last Modified: Wed, 26 Feb 2020 16:49:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:2045b20695df4a308887c27517b0322dd4346c917d64930ec7f475e6f42d6f70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33760905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23127b7b4048f79d0712142146ca1dac13e6f7e1447d989e8a9cac7bddee77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:26:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:26:13 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:26:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:26:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:26:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:26:57 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:26:58 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:26:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed69a865d08c299737373cdce47c8965793574b9ff0824aa64e10a6408a7a0f`  
		Last Modified: Wed, 26 Feb 2020 19:27:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7408f6432832bddbcc6a873062a16487fc77b8f81a0f0712a4a4d6e29d75926a`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 2.0 MB (2007825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b1c317b65863d53f82438d704518c869b157df900bc12823e0a26b3fc4c8f1`  
		Last Modified: Wed, 26 Feb 2020 19:27:18 GMT  
		Size: 5.9 MB (5899308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50411db9d236c261110100ce6f72493081c4d72e48b958be9025fd916278f1e2`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abcf881ec0ba905d35a64d37f591c9ee61d3c11d3b2850a9fbad546ef19afbf`  
		Last Modified: Wed, 26 Feb 2020 19:27:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:2b3380572c777d30dc3c1df78ff3a532c31cf10d6697aa4cac4069356a0f16e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41505089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c3dbcd632dae8470e3fe9fd164ecaeb12f36ba4cef2d4882abbc9dca244068`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:33:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 19:33:40 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 19:33:40 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 19:33:41 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 19:34:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 19:34:06 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 19:34:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 19:34:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 19:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 19:34:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb39e2ebabb52d3a53b8f185dca6c0e86afd917f11cb005127fe42561332d67`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85219efcddbf6309ac25fa211217a0f409881166202a000741c82768e2398cc`  
		Last Modified: Wed, 26 Feb 2020 19:34:21 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a3242d878be2ea033f61cbfc1a7351d69cea664592603153633e6813a9b6f`  
		Last Modified: Wed, 26 Feb 2020 19:34:24 GMT  
		Size: 11.6 MB (11622908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee2e72356c1d3434c64075b0556588135d7214ba648211d57a1f9f67f6b967`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb8de6b637810b5100f73918b939d02e09fa36ae9336dc958ee09a16edb9bc`  
		Last Modified: Wed, 26 Feb 2020 19:34:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c06423344c44b3d742686d3edd389a568a92e2fb50a8b8179a8a1ee69b3545
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39480775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010a4f97446ecf9df1cbf1bf0a27f73134a0e869fc8f9624d8b2a23d841f97ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 18:53:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:53:07 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 18:53:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 18:53:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 18:55:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 18:55:04 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 18:55:06 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 18:55:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:55:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 18:55:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfea20849fee248f74330af12c22433e92bbe7dab537da421edfcd2976601b87`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55407c0d0f18ea49b6657b3d13c844d211899153471b22d30c8a64da45c06794`  
		Last Modified: Wed, 26 Feb 2020 18:55:43 GMT  
		Size: 2.2 MB (2224830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2cea050271247b818081b57713dd5e687ca4752e2bc388597a214d4630fae3`  
		Last Modified: Wed, 26 Feb 2020 18:55:45 GMT  
		Size: 6.7 MB (6735303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa1eba0c0a3d25e79b17cc91014d8eba1f0221e9fe7066067eb5ead76bac08`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c9df31c76a744e37e149d31030486db709ea343608986846673f39e0a9fd15`  
		Last Modified: Wed, 26 Feb 2020 18:55:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:6604a0c90cd36f63713c308d600d37c708070dff8f90483a62623ac468ceac99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33464540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f514f63bc05482a60a7e0f89dd05f9e95e69e655ae00ecadff4d5ffd2d5cd50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:48 GMT
ADD file:3396670211650b5d7c6e1f0ace1a72f1d1587f275baa682dfee6c7bf2603fb34 in / 
# Wed, 26 Feb 2020 00:42:50 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:58:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Feb 2020 07:58:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_VERSION=1.6.0
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.0.tgz
# Wed, 26 Feb 2020 07:58:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=e6f7f8f912172c3ad55638af8346ae7c4ecaa92aed6d3fb60f2bda4359cba1e4
# Wed, 26 Feb 2020 07:59:18 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 07:59:18 GMT
VOLUME [/spiped]
# Wed, 26 Feb 2020 07:59:19 GMT
WORKDIR /spiped
# Wed, 26 Feb 2020 07:59:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Feb 2020 07:59:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 07:59:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e25900e2a7f96a6326b79ec6dfdce1ac5461c7a961fb3752ec1770cd82b8d03c`  
		Last Modified: Wed, 26 Feb 2020 00:47:43 GMT  
		Size: 25.7 MB (25705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea8b61886f4f699c7f3022c2f79fd9edc5b87455b0400e1902ee2cff240003b`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813fd202d108b03f9751b80d328c05ba0a27826f140966910a13ab0d49ceda4c`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 1.8 MB (1821723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2133c8ba6ea7a2d5bb99b4dd9fedf11fd8c9aeef7c98d8981e0e81c425d40`  
		Last Modified: Wed, 26 Feb 2020 07:59:48 GMT  
		Size: 5.9 MB (5934684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25072a908f4a3ead826aa20e08dc8376f6c5e591c181f743943c5b4a7937bcd8`  
		Last Modified: Wed, 26 Feb 2020 07:59:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40daa77c740c41873bcbf019def7b4c0f3fe41d390260d1e23be1d8a1ffb11b7`  
		Last Modified: Wed, 26 Feb 2020 07:59:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
